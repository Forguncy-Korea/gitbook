# TeamCity 구성

TeamCity Professional 2023.05 버전을 기반으로 TeamCity를 구성하는 방법을 소개합니다.

TeamCity의 VCS 기능을 사용해야 하는 경우 Git도 설치해야 합니다.

TeamCity를 설치하고 TeamCity 서버 서비스와 TeamCity 에이전트 서비스를 구성하여 관리 권한이 있는 일반 사용자로 실행되도록 합니다(시스템 권한을 사용하지 않음).

1.  TeamCity에 들어가서 "프로젝트 생성"을 클릭하여 프로젝트를 생성하세요.

    <br>

    "수동"을 선택하고 프로젝트 정보 "이름"과 "프로젝트 ID"를 입력한 후 "만들기"를 클릭합니다.

    <br>

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.643ba7.png" alt=""><figcaption></figcaption></figure>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.110e0b.png" alt=""><figcaption></figcaption></figure>
2.  새 빌드 구성을 추가하려면 "빌드 구성 만들기"를 클릭하세요.



    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.1c1b5c.png" alt=""><figcaption></figcaption></figure>

    "수동"을 선택하고 프로젝트 정보 "이름"과 "빌드 구성 ID"를 입력한 후 "만들기"를 클릭합니다.

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.133bac.png" alt=""><figcaption></figcaption></figure>
3.  VCS를 구성합니다.

    <br>

    구성이 완료되면 "만들기"를 클릭하십시오.

    <figure><img src="../../../.gitbook/assets/image (139).png" alt=""><figcaption></figcaption></figure>

    구성이 완료되면 "만들기"를 클릭하십시오.

    | Type of VCS           | Git을 선택해야 합니다.                                   |
    | --------------------- | ------------------------------------------------ |
    | VCS root name         | 고유한 VCS 루트 이름을 입력합니다.                            |
    | VCS root ID           | VCS 루트 이름을 입력하면 VCS 루트 ID가 자동으로 생성됩니다.           |
    | Fetch URL             | 협업 프로젝트의 URL 주소를 입력하세요.                          |
    | Default branch        | 지점명을 입력하세요.                                      |
    | Authentication method | 인증 방법을 설정하고 저장소에 인증이 필요하지 않은 경우 선택적으로 익명을 선택합니다. |
4.  빌드 단계를 구성합니다.

    ① “Build Steps” 선택 후, “Add Build Step”을 클릭하세요.



    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.568036.png" alt=""><figcaption></figcaption></figure>

    ② “명령줄”을 선택합니다.

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.7b91aa.png" alt=""><figcaption></figcaption></figure>



    ![](https://www.grapecity.com.cn/solutions/huozige/help/docs/v10.0/publishapp/CI\&CD/ConfigTeamcity)③ 빌드 명령어 입력 후 페이지 하단의 “저장” 버튼을 클릭합니다.

    ![영상](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.bdcf74.png)
5.  프로젝트 홈페이지로 돌아가서 빌드 프로젝트를 실행하세요.



    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.800a0e.png" alt=""><figcaption></figcaption></figure>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.9f6c6d.png" alt=""><figcaption></figcaption></figure>

### <br>
