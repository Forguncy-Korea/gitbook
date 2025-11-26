# Https 배포

HTTPS(Hypertext Transfer Protocol over Secure Socket Layer)를 사용하면 서버 측 데이터가 해되는 것을 방지할 수 있습니다. HTTPS는 전문 인증 기관에서 배포한 서버 인증서가 필요합니다.

포건는 pfx/p12 인증서만 지원합니다. 인증서가 다른 유형인 경우 pfx/p12 인증서로 변환할 수 있습니다.



## Https 설정&#x20;

Https를 사용하기 전에 Https 설정이 필요합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72363120/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092696000\&api=v2) 관리 콘솔에서 설정->Https 인증서를 선택합니다.

![](<../../.gitbook/assets/image (744).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72363120/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092696000\&api=v2) Https 인증서의 쿼리 포트 영역에서 포트 번호를 입력하고 쿼리를 클릭하여 포트에 바인딩된 인증서 정보를 가져옵니다. 기본 포트 번호는 443입니다.

SSL 인증서 정보 영역에서 "인증서 해제"를 클릭하여 현재 포트에서 인증서를 제거합니다. 인증서 목록 보기를 클릭하여 목록 대화 상자를 열고 인증서를 선택한 후 바인딩을 클릭하여 인증서를 현재 포트에 바인딩합니다.

![](<../../.gitbook/assets/image (1262).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72363120/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092696000\&api=v2) 서버에 인증서를 업로드합니다.

로컬 컴퓨터에서 인증서 파일을 선택합니다. 인증서에 암호가 필요한 경우 암호를 입력합니다. 인증서 업로드를 클릭하여 서버에 인증서를 업로드합니다.

## Https 배포&#x20;

방법 1. 디자이너의 리본 메뉴 모음에서 배포-> 서버를 선택하고 게시 설정에서 다른 항목을 구성한 후 Https 보안 링크 사용을 선택합니다.

<figure><img src="../../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>

방법 2. 포건시 서버 설치 경로에서 "OfflinePublishTool .exe"을 찾아 두 번 클릭하여 게시 설정 창을 직접 열고 다른 항목을 구성한 후 "Https 웹 사이트로 게시"를 선택합니다.

<figure><img src="../../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>
