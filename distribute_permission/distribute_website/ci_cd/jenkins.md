# Jenkins 구성

Jenkins 버전 2.401.3을 기반으로 Jenkins를 구성하는 방법을 소개합니다. Jenkins를 사용하여 Git Warehouse를 관리하는 경우 먼저 Git을 설치해야 합니다.

Jenkins를 설치한 후 서비스 계정을 관리자 권한이 있는 일반 사용자로 설정합니다.

1.  Jenkins를 입력하고 "새 작업"을 클릭하여 새 작업을 만듭니다.

    ![영상](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.a98396.png)<br>

    작업 이름을 입력한 후 "자유 스타일 소프트웨어 프로젝트 빌드"를 선택하고 "확인"을 클릭합니다.

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.855022.png" alt=""><figcaption></figcaption></figure>
2.  Git을 구성합니다. 프로젝트 파일의 URL 주소를 입력하고 "추가"를 클릭한 ![영상](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.0465d4.png)후 "Jenkins"를 선택합니다.<br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.3b5ce8.png" alt=""><figcaption></figcaption></figure>
3.  Git 저장소의 사용자 이름과 비밀번호를 입력한 후 "저장"을 클릭하세요.

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.83af62.png" alt=""><figcaption></figcaption></figure>
4.  "자격 증명"을 선택하십시오.

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.7db958.png" alt=""><figcaption></figcaption></figure>
5.  지점을 선택하세요.

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.6ee67f.png" alt=""><figcaption></figcaption></figure>
6.  빌드 단계를 추가하고 "Windows 배치 명령 실행"을 선택합니다.

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.ebfeac.png" alt=""><figcaption></figcaption></figure>
7.  빌드 명령을 입력한 후 저장 버튼을 클릭합니다.

    <br>

    <figure><img src="https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.a2f77d.png" alt=""><figcaption></figcaption></figure>
8.  지금 빌드를 클릭하여 프로젝트를 실행합니다.

    ![영상](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/image.968df0.png)
