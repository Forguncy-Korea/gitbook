# 지속적인 배포

포건시는 빌더를 열지 않고도 명령줄을 통해 직접 웹사이트 배포를 지원합니다. 사용자는 정기적으로 파일을 얻거나 프로젝트 개발에 공동 작업을 한 다음 이 기능을 사용하여 프로젝트를 서버에 자동으로 배포할 수 있습니다.

포건시는 "Forguncy.exe"와 동일한 레벨의 새로운 실행 파일인 "ForguncyConsole.exe"를 제공합니다.

* Forguncy Builder를 설치할 때 설치 디렉터리가 기본 디렉터리인 경우 이 파일의 경로는 다음과 같습니다: C:\Program Files\Forguncy _Version_ \Website\designerBin
* Forguncy Builder 설치 시 설치 디렉터리가 Custom Path인 경우, 이 파일의 경로는 "Custom Path\Forguncy _Version_ \Website\designerBin" 입니다.



## 지침&#x20;

기본 사용법은 다음과 같습니다.

명령줄 프로그램을 관리자권한으로 열고 다음 명령을 입력합니다.

```
cd C:\Program Files\Forguncy 10\Website\designerBin
ForguncyConsole /?
```

<figure><img src="../../../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

**ForguncyConsole.exe Action=PublishToServer /help** 명령을 사용하면 더 많은 매개변수 설명을 볼 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (138).png" alt=""><figcaption></figcaption></figure>

### 포건시 프로젝트 파일 배포  <a href="#fa-bu-huo-zi-ge-gong-cheng-wen-jian" id="fa-bu-huo-zi-ge-gong-cheng-wen-jian"></a>

지정된 배포 구성을 사용하여 이동식 유형 프로젝트 파일을 서버에 게시합니다. 공개된 소스파일은 포건시 프로젝트 파일입니다.

샘플 코드는 다음과 같습니다.



```
ForguncyConsole.exe Action=PublishToServer File=D:\Download\Teams\DocumentKuCun.fgko PublishConfigName=PublishSetting1 ServerPassword=123456  
```



매개변수 설명:

| 이름                | 설명                                                                       |
| ----------------- | ------------------------------------------------------------------------ |
| File              | 필수, 이동식 프로젝트 파일의 경로입니다. 지정한 파일이 없으면 오류가 표시됩니다.                           |
| PublishConfigName | 선택사항으로 게시 구성의 이름입니다.                                                     |
| ServerPassword    | 필수로 이동식 서버의 비밀번호입니다. 게시 구성은 비밀번호 설정을 저장하지 않으므로 서버의 비밀번호를 매개변수에 지정해야 합니다. |

### 포건시 프로젝트 파일 폴더 게시(권장) <a href="#fa-bu-huo-zi-ge-gong-cheng-wen-jian-wen-jian-jia-tui-jian" id="fa-bu-huo-zi-ge-gong-cheng-wen-jian-wen-jian-jia-tui-jian"></a>

지정된 게시 구성을 사용하여 공동 개발 프로젝트를 서버에 게시합니다. 지속적 통합의 릴리스 작업에는 이 방법을 사용하는 것이 좋습니다.

연속관리 구성에서 코드소스를 생성할 때 포건시 협업 프로젝트의 주소와 사용자 이름, 비밀번호, 기타 인증 정보를 입력해야 합니다. 지속적인 통합 도구는 협업 엔지니어링 콘텐츠를 자동으로 다운로드하고 업데이트합니다. 포건시는 프로젝트 콘텐츠가 위치한 폴더에 포건시의 내용을 서버에 게시하는 역할만 담당합니다. 지속적인 통합 도구의 소스 코드 변경 감지 기능을 사용하면 공동 프로젝트의 변경 사항을 감지한 후 릴리스 작업을 위해 이 명령줄 도구를 자동으로 실행할 수 있습니다.

**샘플 코드:**

```undefined
ForguncyConsole.exe Action=PublishToServer Folder=.\ PublishConfigName=PublishSetting1 ServerPassword=123456
```

**매개변수 설명:**

| 매개변수              | 설명                                                                                                           |
| ----------------- | ------------------------------------------------------------------------------------------------------------ |
| Folder            | <p>필수, 이동형 프로젝트 폴더는 일반적으로 지속적인 통합 도구인 TeamCity 또는 Jenkins와 같은 CI 도구로 관리됩니다.</p><p>지정한 폴더가 없으면 오류가 표시됩니다.</p> |
| PublishConfigName | 선택사항으로 게시 구성의 이름입니다.                                                                                         |
| ServerPassword    | 필수로 이동식 서버의 비밀번호입니다. 게시 구성은 비밀번호 설정을 저장하지 않으므로 서버의 비밀번호를 매개변수에 지정해야 합니다.                                     |

### 공동개발 프로젝트 공개 <a href="#fa-bu-huo-zi-ge-xie-zuo-kai-fa-xiang-mu" id="fa-bu-huo-zi-ge-xie-zuo-kai-fa-xiang-mu"></a>

지정된 게시 구성을 사용하여 공동 개발 프로젝트를 서버에 게시합니다. 협업창고 주소, 인증 사용자 이름, 비밀번호 등을 제공해야 합니다.

**샘플 코드:**

```bash
ForguncyConsole.exe Action=PublishToServer RepoUrl=http://xa-dd3-orrin22/Bonobo.Git.Server/OrrinTest.git RepoUserName=admin RepoPassword=admin PublishConfigName=PublishSetting1 ServerPassword=123456 ServerName=xa-dd3-orrin22 OverrideBuiltinDatabase=true
```

지정된 게시 구성을 사용하지 않고 이동형 공동 개발 프로젝트를 서버에 게시합니다.

**샘플 코드:**

```bash
ForguncyConsole.exe Action=PublishToServer RepoUrl=http://xa-dd3-orrin22/Bonobo.Git.Server/OrrinTest.git RepoUserName=admin RepoPassword=admin ServerName=xa-dd3-orrin22 UserName=Administrator ServerPassword=123456 AppName=Test1
```

| 매개변수              | 설명                                                                                                                                                                                         |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| RepoUrl           | 필수, 이동식 콜라보 프로젝트의 주소입니다.                                                                                                                                                                   |
| RepoBranchName    | 선택 사항이며 공동 프로젝트의 분기 이름이며 기본값은 master입니다.                                                                                                                                                   |
| RepoUserName      | 선택사항, 이동형 협업 프로젝트를 인증하는 데 사용되는 사용자 이름입니다. 현재 컴퓨터가 이미 인증된 경우(이전에 열린 공동 작업 프로젝트) 또는 저장소에 익명 액세스 권한이 있는 경우(예: GitHub의 공개 저장소) 이 매개변수는 필요하지 않습니다. 그렇지 않으면 저장소를 인증하기 위해 사용자 이름과 비밀번호를 지정해야 합니다. |
| RepoPassword      | 선택사항, 이동식 협업 프로젝트를 인증하는 데 사용되는 비밀번호입니다.                                                                                                                                                    |
| PublishConfigName | 선택사항으로 게시 구성의 이름입니다.                                                                                                                                                                       |
| ServerPassword    | 필수로 이동식 서버의 비밀번호입니다. 게시 구성은 비밀번호 설정을 저장하지 않으므로 서버의 비밀번호를 매개변수에 지정해야 합니다.                                                                                                                   |

### 기타 사용 가능한 매개변수 <a href="#qi-ta-ke-yong-can-shu" id="qi-ta-ke-yong-can-shu"></a>

명령줄에서 더 많은 매개변수와 값을 볼 수 있습니다. 게시 프로세스에 더 많은 설정 전달을 지원합니다. 이러한 매개변수의 기본값은 게시 대화상자의 기본 옵션과 동일하게 작동합니다.

<table><thead><tr><th>매개변수 </th><th width="311">설명 </th><th width="173">유형 </th><th>기본값</th></tr></thead><tbody><tr><td>ServerName</td><td>서버 호스트 이름 또는 IP 주소.</td><td>string</td><td>null</td></tr><tr><td>UserName</td><td>서버에 인증하는 데 사용되는 사용자 이름입니다.</td><td>string</td><td>administrator</td></tr><tr><td>SitePort</td><td>애플리케이션의 포트입니다.</td><td>string</td><td>null</td></tr><tr><td>AppName</td><td>애플리케이션의 이름입니다.</td><td>string</td><td>null</td></tr><tr><td>AppStartPage</td><td>애플리케이션의 기본 페이지입니다.</td><td>string</td><td>与应用程序设置相同</td></tr><tr><td>Https</td><td>애플리케이션에 SSL을 사용하십시오.</td><td>bool</td><td>false</td></tr><tr><td>PublishRolesToServer</td><td>빌더의 역할을 서버에 게시합니다.</td><td>bool</td><td>true</td></tr><tr><td>PublishUsersToServer</td><td>빌더의 사용자를 서버에 게시합니다.</td><td>bool</td><td>false</td></tr><tr><td>PublishOrganizationsToServer</td><td>빌더의 조직을 서버에 게시합니다.。</td><td>bool</td><td>false</td></tr><tr><td>OverrideBuiltinDatabase</td><td>서버단 내장 데이터베이스를 재정의합니다.</td><td>bool</td><td>false</td></tr><tr><td>OverrideProcessDatabaseToServer</td><td>서버단 프로세스 데이터베이스를 덮어씁니다.</td><td>bool</td><td>false</td></tr><tr><td>OverrideProcessFilesToServer</td><td>서버단 프로세스 디자인 파일을 재정의합니다.</td><td>bool</td><td>false</td></tr><tr><td>OverridePageAuthorityToServer</td><td>페이지 권한 및 셀 권한을 포함한 서버 권한을 재정의합니다.。</td><td>bool</td><td>false</td></tr><tr><td>OverrideServerScheduleTask</td><td>서버 예약 작업을 재정의합니다.</td><td>bool</td><td>false</td></tr><tr><td>OverrideServerGlobalProperty</td><td>전역 속성 설정을 재정의합니다.</td><td>bool</td><td>false</td></tr><tr><td>OverrideServerActiveReports</td><td>보고서</td><td>bool</td><td>false</td></tr></tbody></table>

### 반환 값 <a href="#fan-hui-zhi" id="fan-hui-zhi"></a>

게시 중에 오류가 발생하면 0이 아닌 값(오류 코드)이 콘솔에 반환됩니다. 콘솔 출력에서 ​​다음 오류 코드에 대한 자세한 이유를 확인할 수 있습니다. 여기에는 간단한 원인과 해결책만 나와 있습니다.

<table><thead><tr><th width="178">반환코드 </th><th>중요성 </th><th>해결 방법 </th></tr></thead><tbody><tr><td>0</td><td>성공</td><td><br></td></tr><tr><td>1000</td><td>누락된 작업 매개변수</td><td>작동 매개변수를 지정하십시오.</td></tr><tr><td>1001</td><td>잘못된 작업 값</td><td>올바른 작업 값을 지정하십시오.</td></tr><tr><td>1010</td><td>파일 매개변수 누락</td><td>파일 매개변수를 지정하십시오.</td></tr><tr><td>1011</td><td>지정한 파일이 존재하지 않습니다</td><td>기존 파일을 지정하십시오.</td></tr><tr><td>1012</td><td>폴더 매개변수 누락</td><td>폴더 매개변수를 지정하십시오.</td></tr><tr><td>1013</td><td>지정한 폴더가 존재하지 않습니다</td><td>기존 폴더를 지정하십시오</td></tr><tr><td>1020</td><td>이동형 문서에 PublishConfig가 없습니다.</td><td>기존 PublishConfig를 지정하세요.</td></tr><tr><td>1021</td><td>비밀번호 매개변수 누락</td><td>비밀번호 매개변수를 지정하세요.</td></tr><tr><td>1030</td><td>RepoUrl 매개변수가 누락되었습니다.</td><td>RepoUrl 매개변수를 지정하십시오.</td></tr><tr><td>2000</td><td>RepoUrl 매개변수로 지정된 프로젝트를 열지 못했습니다. 디자이너에게 직접 열어봐도 효과는 똑같습니다.</td><td>이동식 콜라보레이션 프로젝트가 유효한지 확인해주세요.</td></tr><tr><td>2001년</td><td>폴더 매개변수로 지정된 항목을 열지 못했습니다. 디자이너에게 직접 열어봐도 효과는 똑같습니다.</td><td>이동식 협업 프로젝트나 CI 구성이 유효한지 확인해주세요.</td></tr><tr><td>2002년</td><td>파일 매개변수로 지정된 프로젝트를 열지 못했습니다. 디자이너에게 직접 열어봐도 효과는 똑같습니다.</td><td>이동형 파일이 유효한지 확인해주세요.</td></tr><tr><td>2010</td><td>문서가 검사 오류로 생성되었습니다. 예를 들어 이동식 그리드 프로젝트에 잘못된 수식 참조가 있거나 테이블이 삭제되었습니다.</td><td>유형 그리드 디자이너에서 버그를 해결하십시오.</td></tr><tr><td>2011년</td><td>빌드 중 기타 예상치 못한 오류</td><td>디자이너에서 문서를 게시해 보고 어떤 일이 일어나는지 확인할 수 있습니다.</td></tr><tr><td>2012년</td><td>게시 설정을 확인하지 못했습니다. 예를 들어, 호스트 이름이 연결 가능하지 않거나 사용자 이름/비밀번호가 올바르지 않습니다.</td><td>게시 설정을 업데이트하세요.</td></tr><tr><td>2013년</td><td>게시하는 동안 예상치 못한 오류가 발생했습니다. 예를 들어 갑자기 네트워크 연결이 끊어지고 서버가 종료되는 경우입니다.</td><td>디자이너에서 문서를 게시해 보고 어떤 일이 일어나는지 확인할 수 있습니다.</td></tr></tbody></table>

### <br>
