# 기존 사용자 정보 연동



1. **Office 365 Single Sign On** 서버 명령을 아래와 같 만듭니다.&#x20;

&#x20;    \- 모든 역할의 접근 허용 : 모두&#x20;

&#x20;    \- HTTP 메소드 : GET&#x20;

<figure><img src="../../../../../.gitbook/assets/image (929).png" alt=""><figcaption></figcaption></figure>

2\. 아래와 같이 명령을 설정합니다.&#x20;

* ClientID, TenantID 및 Client Secret을 입력합니다. ([ClientID, TenantID 및 Client Secret 생성법](../office-365.md) 참고하세요) &#x20;
* 로그인 모드는 기존 사용자 정보 연동을 선택합니다.&#x20;
* 기존 사용자 페이지 이름 연동 : 포건시에 해당 페이지를 만들어야 합니다.&#x20;
* 속성에 ID 저장 &#x20;

<figure><img src="../../../../../.gitbook/assets/image (1774).png" alt=""><figcaption></figcaption></figure>

3\.  아래와 같이 버튼을 만들고 "명령 편집"을 클릭합니다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (2272).png" alt=""><figcaption></figcaption></figure>

4\. 명령 창에서 아래와 같이 설정합니다.&#x20;

&#x20;   \- 명령 선택 : 페이지 이동 명령 만들기&#x20;

&#x20;   \- 값 선택 : 1 번에서 생성한 명령 값을 넣어줍니다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (2080).png" alt=""><figcaption></figcaption></figure>

5\. 서버에서 해당 사용자 정의 속성을 설정합니다.&#x20;

<figure><img src="../../../../../.gitbook/assets/image (1127).png" alt=""><figcaption></figcaption></figure>

6\. 기존 사용자 페이지 이름 연동을 합니다.&#x20;

&#x20;  6-1. Office 365 서버에 사용자 바인딩 만들기 명령

&#x20;    a. 일반 : 역할 권한을 익명으로 설정&#x20;

<figure><img src="../../../../../.gitbook/assets/image (897).png" alt=""><figcaption></figcaption></figure>

&#x20;  b. 파라미터 : 토큰, userName 및 암호(userName 및 암호는 신원 확인에 사용됨)



<figure><img src="../../../../../.gitbook/assets/image (2088).png" alt=""><figcaption></figcaption></figure>

&#x20;  c. 명령 : 파라미 설정&#x20;

<figure><img src="../../../../../.gitbook/assets/image (2152).png" alt=""><figcaption></figcaption></figure>

&#x20;6-2. 사용자 등록 및 바인딩이 필요한 경우 사용자 추가 서버단 명령을 설정해야 합니다.&#x20;

&#x20; a. 일반 : 역할 권한을 익명으로 설정&#x20;

<figure><img src="../../../../../.gitbook/assets/image (1490).png" alt=""><figcaption></figcaption></figure>

&#x20; b. 파라미터 : 필수 파라미터 설정 (기존 사용자 페이지와 연동 필요 )

<figure><img src="../../../../../.gitbook/assets/image (1373).png" alt=""><figcaption></figcaption></figure>

&#x20;c. 명령 : 파라미터 설정&#x20;

<figure><img src="../../../../../.gitbook/assets/image (2273).png" alt=""><figcaption></figcaption></figure>

6-3. 계정 바인딩 페이지, 익명 액세스로 설정됨 (이미 계정 있음)

&#x20;      a. **Token** : 페이지가 Office 365 Single Sign on 명령에 설정된 RelativeUserPageName인 경우 GETURLQUERYVALUE("Office365UserToken") 함수를 통해 토큰을 얻을 수 있습니다.

<figure><img src="../../../../../.gitbook/assets/image (2124).png" alt=""><figcaption></figcaption></figure>

사용자를 Office 365 서버에 바인딩 명령 호출

<figure><img src="../../../../../.gitbook/assets/image (512).png" alt=""><figcaption></figcaption></figure>

6-4. 페이지 등록 및 바인딩 , 익명 액세스(계정 없음)로 설정

&#x20;a. **Token** : 페이지가 Office 365 Single Sign on 명령에 설정된 RelativeUserPageName인 경우 GETURLQUERYVALUE("Office365UserToken") 함수를 통해 토큰을 얻을 수 있습니다.

&#x20;b. 사용자 추가 및 Office 365 서버에 사용자 바인딩 명령을 호출합니다.
