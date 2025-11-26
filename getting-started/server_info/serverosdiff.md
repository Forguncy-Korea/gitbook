# Linux 용 Forguncy Server의 차이점과 주의점

Windows 버전의 Forguncy Server의 경우 설치 프로그램에 .NET 라인 타임이 포함되어 있지만 Linux 버전에는 포함되어 있지 않습니다. 이것은 리눅스의 경우에는 배포 유형에 따라 필요한 패키지가 다르기 때문입니다. 따라서 Linux용 Forguncy Server를 설치하려면 인터넷 연결이 필요합니다.

## 지원되지 않는 기능

다음 기능은 Linux 버전의 Forguncy Server에서 지원되지 않습니다.

* Windows 인증("Windows Active Directory용 인증 공급자" 포함)
* 동일한 포트 번호를 사용하여 여러 앱 배치
  * Windows 버전 Forguncy Server의 경우, 예를 들어 app1과 app2를 모두 80번 포트로 배치할 수 있지만, Linux 버전에서는 app1에서 80번 포트로 배치한 경우 app2는 80번 이외의 포트로 배치해야 합니다.
* 오프라인에서 앱 배치

## Windows 버전과 Linux 버전에서 다른 기능

*   PDF 내보내기 명령, Excel 내보내기(페이지) 명령(일반 명령 및 서버측 명령), Excel 내보내기(목록 보기) 명령

    * 그라디언트와 투명 설정(투명도)을 모두 사용하는 경우 Windows 버전과 Linux 버전에서는 색조가 약간 다를 수 있습니다.



## 기본적으로 설정된 경로

<table><thead><tr><th width="233">기능</th><th>Windows 버전 경로</th><th>Linux 버전의 경로</th></tr></thead><tbody><tr><td>자동 백업을 저장할 폴더</td><td>C:\Users\Public\Documents\ForguncyServerBackup</td><td>/opt/ForguncySites/ForguncyServerBackup</td></tr><tr><td>애플리케이션 배포 경로</td><td>C:\Users\Public\Documents\ForguncyServer</td><td>/opt/ForguncySites/ForguncyServer</td></tr><tr><td>감사 로그 저장 경로</td><td>C:\Windows\TEMP\</td><td>/var/log/ForguncyServer/</td></tr><tr><td>동시 연결 로그 저장 경로</td><td>%temp%\Forguncy\ForguncyConcurrencyAccessLog</td><td>/var/log/ForguncyServer/Forguncy/ForguncyConcurrencyAccessLog</td></tr></tbody></table>

## 글꼴 파일 설치

Forguncy는 다음 기능에서 Forguncy Server 환경의 글꼴 데이터를 사용합니다. Forguncy Builder는 Windows 환경에서 사용하기 때문에 Forguncy Server 환경도 Windows이면 개발시에 설정한 폰트가 서버 환경에도 존재하고 있는 경우가 대부분이지만, Linux의 경우에는 필요에 따라서 폰트를 설치해야 합니다. 일반적으로 글꼴에는 사용법에 따라 라이센스가 있습니다. 글꼴을 설치할 때 글꼴의 라이센스를 확인하십시오.

* PDF 내보내기 명령(일반 명령 및 서버단 명령)
* 보고서 내보내기 명령(일반 명령 및 서버단 명령)
* Excel 내보내기(페이지) 명령에서 문자가 이미지로 출력되는 부분(예: 버튼 셀)
* Excel 내보내기(목록 보기) 명령에서 문자가 이미지로 출력되는 부분(예: 버튼 셀)

다음은 폰트를 설치하는 절차의 예입니다.

1.  **글꼴을 설치할 디렉토리를 만듭니다.**

    **sudo mkdir -p /usr/share/fonts/opentype/noto**

    위의 "opentype" 이후의 경로는 임의의 것을 사용할 수 있습니다. 또는 디렉토리를 만들지 않고 "/usr/share/fonts/"를 사용할 수 있습니다.
2.  **설치할 글꼴 파일을 만든 디렉토리에 복제합니다.**

    **sudo cp -r \*.otf /usr/share/fonts/opentype/noto**
3.  **대상 디렉토리에 쓰기 권한을 설정합니다.**

    **sudo chmod 755 /usr/share/fonts/opentype/noto**
4.  **폰트 캐시를 업데이트합니다.**

    **sudo fc-cache -f -v**

    fc-cache 명령을 찾을 수 없으면 다음 절차에 따라 "fontconfig"를 설치하십시오.

    우분투의 경우 :

    **sudo apt install fontconfig**

    CentOS의 경우:

    **sudo yum install fontconfig**

## 자동으로 추가되는 방화벽 설정

Forguncy Server에 응용 프로그램이 배포되거나 Forguncy Server 서비스가 다시 시작되면 응용 프로그램에 필요한 포트 번호를 사용할 수 있도록 방화벽 설정이 Forguncy Server에 의해 자동으로 변경됩니다.

본 동작은, Windows판과 Linux판에서 공통의 동작입니다. 그러나 Linux 버전의 Forguncy Server의 경우 포트 개방은 일시적인 구성이므로 서버를 다시 시작할 때 사용할 수 없습니다. 영구 포트 개방이 필요한 경우 방화벽 포트 개방을 필요한 포트 번호에 대해 재구성하십시오.

Linux 버전의 Forguncy Server의 경우 다음 파일을 삭제하여 응용 프로그램을 게시할 때 방화벽의 자동 구성 동작을 비활성화할 수 있습니다.

/opt/ForguncyServer/WebSite/bin/Forguncy.FireWall.json

## 서버 관리 포털의 표시 언어 <a href="#i-heading---4" id="i-heading---4"></a>

Windows 버전의 경우 서버 관리 포털의 표시 언어는 Forguncy Server 서비스를 실행하는 사용자의 언어 설정에 따라 다릅니다. Linux 버전의 경우 서버 관리 포털은 OS 설정에 관계없이 항상 한국어로 표시됩니다.
