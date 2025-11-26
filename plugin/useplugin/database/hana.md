# Hana 데이터 베이스

Hana 데이터베이스 (SAP 데이터베이스)와의 원활한 통합을  통해 업무 효율성을 향상 시킬 수 있습니다.&#x20;

포건시와 SAP 간의 연결을 완성하기 위해 SAP 의 Hana 데이텁베이스에 연결합니다.&#x20;

Hana 데이터 베이스에 연결하려면 다음 조건을 충족해야 합니다.&#x20;

* PC의 Hana 클라이언트&#x20;
* 서버는 Hana데이터베이스를 실행하고 연결할 준비&#x20;



### 플러그인 다운로드

<table><thead><tr><th width="151">버전</th><th>다운로드</th></tr></thead><tbody><tr><td>V10 </td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/HanaDbWrapper.zip">HanaDBWrapper.zip</a></td></tr></tbody></table>



### PC에 Hana 클라이언트를 설치하는 방법&#x20;

1.  Hana 클라이언트 설치 프로그램을 다운로드 합니다. SAP Hana 사용자가 아닌 경우, 설치만 가능합니다.&#x20;

    <figure><img src="../../../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>


2. Hana 클라이언트는 JRE 버전 8 이상을 사용합니다. 설치하기 전에 버전 8이 있는지 확인하세요. [최신 Java LTS 무료 다운로드](https://www.oracle.com/java/technologies/downloads/) 에서 다운로드하거나 jre-8u381-windows-x64.exe 첨부 파일을 다운로드할 수도 있습니다.&#x20;
3.  하나 클라이언트를 설치합니다 . 다운로드한 파일의 압축을 풀고 실행 가능한 애플리케이션 hdbinst.exe 를 실행한 후 설치 경로를 선택하고 완료될 때까지 기다립니다.

    <figure><img src="../../../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>





### Hana 서버를 얻는 방법&#x20;

1. 하나 데이터베이스는 Linux 에서만 실행할 수 있습니다 . 로컬 Linux 가상 머신 에서 개발하려면 "Sap Hana Express Edition 2.0 sps06"을 사용합니다 . 이러한 서버는 다음 단계를 통해 얻을 수 있습니다. 다른 버전을 구할 수 있는 방법이 있다면 이를 따를 필요는 없습니다. 실행 중인 Hana 데이터베이스의 버전에 관계없이 LiveType은 Hana 클라이언트와 서버가 상호 호환되기 때문에 성공적으로 연결됩니다.
2. 시작하기 전에 VMWare 워크스테이션 소프트웨어 가 있는지 확인하십시오 . SAP는 Hana 데이터베이스가 있는 서버를 로컬 컴퓨터 HXEDownloadManager\_win.exe 로 가져오는 데 도움이 되는 ova 파일을 다운로드할 수 있는 다운로드 관리자를 제공합니다 .
3. 다운로드 관리자를 실행하고 " Server VM Only "를 선택하여 다운로드합니다. 불안정한 네트워크로 인해 이 다운로드 관리자를 제대로 실행하지 못할 수 있습니다. 다운로드 관리자를 성공적으로 열고 ova 파일을 다운로드할 때까지 닫았다가 반복해서 실행하세요.

<figure><img src="../../../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

4. VMWare를 사용하여 방금 다운로드한 ova 파일을 가져옵니다 .

<figure><img src="../../../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

5. 가져온 Linux 시스템은 SUSE 입니다 . 기본 사용자 이름과 비밀번호는 'hxeadm' 및 'HXEHana1' 입니다 . 그런 다음 시스템 비밀번호를 변경하고 데이터베이스 마스터 비밀번호를 설정한 후 다음 명령줄을 사용하여 Hana SUSE에 연결할 수 있는지 확인합니다.

<figure><img src="../../../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

6.  클라이언트와 서버가 있으면 Hana 에 연결할 수 있습니다 .포건시에서 Hana 에 대한 연결을 만듭니다 . 기본 포트는 39013 이고 호스트는 가상 머신의 IP 주소입니다 .

    <figure><img src="../../../.gitbook/assets/image (164).png" alt=""><figcaption></figcaption></figure>

    <figure><img src="../../../.gitbook/assets/image (165).png" alt=""><figcaption></figcaption></figure>

### Linux 서버 에서 HANA 연결

최종 사용자는 포건시를 통해 하나 데이터베이스에 접근하고, 포건시도 하나 의 클라이언트 이기 때문에 포건시 서버에도 데이터 드라이버를 설치해야 한다. Windows 시스템 에 Hana 클라이언트를 직접 설치할 수도 있지만, Linux 시스템에 클라이언트를 설치하는 경우에는 데이터 드라이버가 제공되지 않기 때문에 수동으로 데이터 드라이버를 다운로드하고 글로벌 환경을 가리키도록 설정해야 합니다. 다운로드한 데이터 드라이버.

* 다운로드 주소: [SAP 개발 도구](https://tools.hana.ondemand.com/#hanatools)

<figure><img src="../../../.gitbook/assets/image (166).png" alt=""><figcaption></figcaption></figure>

* tar.gz 파일 의 압축을 풀면 dotnetcore 라는 폴더가 있어야 합니다 .
*   전역 환경 설정: /etc/environment 파일로 이동하여 아래 코드를 추가하고 '/opt/hana/dotnetcore' 경로가 데이터 공급자가 있는 위치이며 ' 와 동일 할 필요는 없습니다. /opt/ hana/dotnetcore' , 그러나 폴더 에 libadonetHDB.so 및 Sap.Data.Hana.Core.v2.1.dll 이라는 두 개의 어셈블리가 포함되어 있는지 확인하십시오.

    <figure><img src="../../../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

이 플러그인을 선택하면 데이터베이스에 쉽게 연결할 수 있습니다. 플러그인을 선택하고 적절하게 구성하면 설계에서 데이터베이스에 직접 연결할 수 있습니다. 이러한 방식으로 데이터베이스의 테이블을 사용하여 테이블 데이터 소스 바인딩, 추가, 삭제, 수정, 쿼리 등의 작업을 수행할 수 있습니다. 이 기능의 도입으로 데이터 작업이 더욱 편리하고 효율적으로 이루어졌습니다.
