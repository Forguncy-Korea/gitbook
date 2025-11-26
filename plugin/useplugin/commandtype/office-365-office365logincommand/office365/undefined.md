# 새로운 생성자 사용

1\. 먼저 포건시를 열고 새로운 프로젝트를 생성하십시오.

2\. 다음은 페이지를 하나 생성하겠습니다. 이 페이지는 로그인이 완료된 후 보여줄 페이지입니다. (페이지 구성에 대한 내용은 자세히 설명하지 않습니다. 잘 모르시면 따로 질문해 주세요.)

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846687_8253.png" alt=""><figcaption></figcaption></figure>

3\. 다음은 프로젝트 탐색기의 서버단 명령에 마우스 오른쪽 클릭한 후 새로운 서버단 명령 생성하기를 선택하십시오.

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846780_0609.png" alt=""><figcaption></figcaption></figure>

4\. 서버단 명령 생성을 시작하시고, 제목에 「Office 365-Single-Sign-On」, 권한은 「모두」, HTTP 메소드는 「GET」으로 지정해 주십시오.&#x20;

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/5db70dd0f77dfc40f7e8f6ea6b112c67_1644902195_0835.png" alt=""><figcaption></figcaption></figure>

본문의 처음에 설명드린 바와 같이 본 매뉴얼은 초보자들을 위한 매뉴얼이 아닙니다. 왜 이렇게 설정해야 하는 지에 대한 설명은 따로 드리지 않습니다.

5\. 다음은 「명령」 탭으로 이동하여 「명령 편집」을 클릭합니다.

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846857_6691.png" alt=""><figcaption></figcaption></figure>

6\. 명령 실행창이 나타나면 「Office365 통합인증」 을 찾아 선택합니다.

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846866_051.png" alt=""><figcaption></figcaption></figure>

7\. 「Office365 통합인증」 서버 명령 내에 필수 항목인 Client ID, Tenant ID, Client Secret을 입력합니다.&#x20;

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846906_9203.png" alt=""><figcaption></figcaption></figure>

8\. 이제 확인을 눌러 서버 명령을 저장합니다. 아래와 같이 나타나면 성공입니다.

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846921_0045.png" alt=""><figcaption></figcaption></figure>

9\. 자, 다음은 포건시의 프로젝트 탐색기 > 기본 제공 페이지 > 로그인 페이지로 이동합니다.

&#x20;

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846981_3094.png" alt=""><figcaption><p><br></p></figcaption></figure>

10\. 로그인 페이지에 수동으로 「Office 365 SSO」 로그인 버튼을 추가합니다.



<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644846994_1871.png" alt=""><figcaption></figcaption></figure>

버튼 생성 방법은 따로 설명하지 않습니다. 어떻게 생성하시는 지 모르시는 경우 게시판에 따로 질문을 올려 주세요.&#x20;

11\. 새로 생성한 버튼에 마우스 오른쪽을 클릭 후, 명령 편집을 선택합니다.

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644847014_5846.png" alt=""><figcaption></figcaption></figure>

12\. 명령 편집창이 나타나면 「페이지 이동 명령」을 선택한 후, 옵션을 「값」으로 선택합니다. 이후 아래 그림과 같이 앞서 작성한 서버단 기능을 호출하도록 지정합니다. 지정 방식은 ServerCommand/{서버단 명령 이름} 입니다. 이렇게 호출하면 작성한 서버단 명령을 API 형태로 호출할 수 있습니다.



<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/5db70dd0f77dfc40f7e8f6ea6b112c67_1644902340_9822.png" alt=""><figcaption></figcaption></figure>

13\. 이제 작성한 앱을 서버로 배포합니다.

<figure><img src="https://dev.grapecity.co.kr/data/editor/2202/b38ccd225d199fb490e7b67d143f734a_1644847114_5002.png" alt=""><figcaption></figcaption></figure>
