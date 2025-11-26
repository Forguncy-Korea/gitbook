# 클라우드 스토리지

클라우드 스토리지 연계 기능을\
사용하면 외부 클라우드 스토리지 서비스와 Forguncy를 연동할 수 있습니다.



> 본 기능은 미리 이용하는 클라우드 스토리지의 계정을 설정하고, Forguncy Builder에서 설정하는 명령상에서 저장처 폴더를 설정하는 기능이며, 이용자가 이용하는 클라우드 스토리지나 저장처를 선택할 수 있는 것은 아닙니다.

{% file src="../../../.gitbook/assets/CloudStorageProvider (1).zip" %}

Forguncy가 지원하는 클라우드 스토리지 서비스는 다음과 같습니다.

* Google 드라이브
* OneDrive
* DropBox
* Box
* SharePoint

### 클라우드 저장소 업로드&#x20;

서버관리자에서 \[설정>클라우드 저장소 설정]을 선택하여 클라우드 저장소 설정 페이지로 들어갑니다.

업로드를 클릭하고 클라우드 저장소 공급자를 선택하고 업로드 후 인증 구성을 수행합니다.

<figure><img src="../../../.gitbook/assets/image (2518).png" alt=""><figcaption></figcaption></figure>

업로드가 완료되면 아래 목록에 공급자 이름, 버전 번호 및 의존성 버전 번호가 표시됩니다. ![](https://help.grapecity.com.cn/download/thumbnails/80953092/image2022-9-30_16-34-14.png?version=1\&modificationDate=1673923284000\&api=v2)버튼을   클릭하면 삭제할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (1541).png" alt=""><figcaption></figcaption></figure>



### 클라우드 인증 설정&#x20;

인증설정 탭을 클릭 한 후, \[인증 추가]버튼을 클릭하면 공급자 정보 편집창이 뜹니다.

공급자 정보 편집창에 정보를입력합니다.

<figure><img src="../../../.gitbook/assets/image (1140).png" alt=""><figcaption></figcaption></figure>

### 클라우드 스토리지 사용&#x20;

클라우드 스토리지를 구성한 후 스토리지 유형 설정에서 클라우드 스토리지를 선택할 수 있습니다.

예를 들어 관리 콘솔의 "설정-저장 경로"에서 최종 사용자가 업로드한 파일의 저장 유형을 클라우드 저장소로 설정합니다 .

<figure><img src="../../../.gitbook/assets/image (2285).png" alt=""><figcaption></figcaption></figure>

애플리케이션의 고급 설정에서 최종 사용자가 클라우드 스토리지에 업로드한 파일의 스토리지 유형을 설정합니다.

<figure><img src="../../../.gitbook/assets/image (1855).png" alt=""><figcaption></figcaption></figure>
