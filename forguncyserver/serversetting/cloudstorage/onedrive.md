# OneDrive 구성

서버관리자에서 OneDrive 클라우드 저장소 공급자를 업로드한 후 인증 설정 탭에서 인증 추가를 클릭하면 팝업되는 공급자 정보 편집 창에서 몇 가지 설정을 입력해야 합니다.&#x20;

그 중 클라이언트ID와 클라이언트 Secret은 OneDrive에서 얻어야 합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1137).png" alt=""><figcaption></figcaption></figure>

이 섹션에서는 OneDrive 클라우드 저장소 구성을 위한 인증 정보를 소개합니다.



### OneDrive 구성&#x20;

OneDrive 클라우드 저장소에 대한 인증 정보를 구성하려면 OneDrive에서 ClientId 및 ClientSecret 정보를 가져와야 합니다. 이 정보를 얻는 방법은 다음과 같습니다.

[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)  도메인 계정이 아닌 개인 계정으로 [https://portal.azure.com/#home](https://portal.azure.com/#home) 에 로그인합니다 .

[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)  Azure 서비스에서Azure Active Directory를 선택합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (327).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923286000\&api=v2)  왼쪽 메뉴에서\[추가>앱등록]을 클릭합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (670).png" alt=""><figcaption></figcaption></figure>

[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)  애플리케이션 등록 페이지에서 정보를 입력합니다.

지원되는 계정 유형 "개인 Microsoft 계정"을 포함하는 옵션을 선택하고 리디렉션 URL은 " _**AppBaseUrl**_ /UserService/CloudStorageProvider/OAuthCallback"입니다.

* 디자인 타임의 앱 리디렉션 URL은 http:// _localhost:PORT/_ Forguncy/CloudStorageProvider/OAuthCallback 입니다.
* 서버에 게시된 애플리케이션 리디렉션 URL은 http:// _localhost:PORT_/CloudStorageProvider/OAuthCallback 입니다.

설정이 완료되면 등록을 클릭합니다.

<figure><img src="../../../.gitbook/assets/image (2096).png" alt=""><figcaption></figcaption></figure>

서버관리자의 도메인 이름은 http://_localhost:22345/이며_ **도메인 이름은 일치해야 합니다.**

<figure><img src="../../../.gitbook/assets/image (2037).png" alt=""><figcaption></figcaption></figure>

[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)  앱 왼쪽 메뉴에서 "인증서 및 암호"를 클릭합니다.을 클릭한 다음 새 클라이언트 암호를 클릭하여 표시된 페이지에 클라이언트 암호를 추가합니다.

<figure><img src="../../../.gitbook/assets/image (1141).png" alt=""><figcaption></figcaption></figure>

추가 후 ClientSecret을 얻을 수 있습니다.

이 비밀번호는 생성된 직후에 볼 수 있는 값을 제외하고는 나중에 볼 수 없다는 점에 유의해야 합니다. 나중에 사용할 수 있도록 이 암호 값을 저장하려면 어딘가에 복사해야 합니다.

<figure><img src="../../../.gitbook/assets/image (2087).png" alt=""><figcaption></figcaption></figure>

[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)  애플리케이션 개요 페이지에서 ClientId를 얻을 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (1138).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A47.png?version=1\&modificationDate=1673923286000\&api=v2)  API 권한을 추가합니다. 왼쪽 메뉴에서 "API 권한"을 선택하고 "권한 추가"를 클릭하십시오.

<figure><img src="../../../.gitbook/assets/image (1168).png" alt=""><figcaption></figcaption></figure>

"마이크로소프트 그래프"를 선택합니다.

<figure><img src="../../../.gitbook/assets/image (1275).png" alt=""><figcaption></figcaption></figure>

위임된 권한을 선택합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1134).png" alt=""><figcaption></figcaption></figure>

권한 선택 검색 상자에 "File"을 입력하고 파일을 확장한 다음 Files.ReadWrite.All을 선택하고 권한 추가를 클릭합니다.

<figure><img src="../../../.gitbook/assets/image (1163).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A48.png?version=1\&modificationDate=1673923286000\&api=v2)  이 시점에서 OneDrive가 설정되었으므로 단계를 입력해야 합니다.[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)그리고[![](https://help.grapecity.com.cn/download/thumbnails/80953251/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1673923286000\&api=v2)](https://cloud.tencent.com/)인증 정보에서 얻은 클라이언트Id와 클라이언트Secret을 입력합니다.

<figure><img src="../../../.gitbook/assets/image (1702).png" alt=""><figcaption></figcaption></figure>

"로그인 및 저장"을 클릭하면 인증 설정 테이블에서 구성된 인증 정보를 볼 수 있으며 이 인증 정보를 편집하거나 삭제할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (1231).png" alt=""><figcaption></figcaption></figure>
