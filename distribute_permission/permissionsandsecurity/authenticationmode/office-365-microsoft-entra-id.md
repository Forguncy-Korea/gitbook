# Office 365 (Microsoft Entra ID)

#### 다운로드 링크&#x20;

{% file src="../../../.gitbook/assets/Office365SecurityProviderNew.zip" %}

포건시 로그인의 종류는 크게 총 3가지로 볼 수 있습니다.&#x20;

1. Forguncy 인증 : 포건시 서버 자체에서 사용자 관리
2. Windows 인증 : Microsoft사의 Active Directory를 연동한 사용자 관리
3. 제3자 인증 : 네이버, 카카오, 구글, 페이스북 등 타사의 로그인을 연동한 사용자 관리

포건시로 앱을 만드는 개발자는 위 3가지 중 1가지를 택하여 사용자 로그인 방식으로 채택하실 수 있습니다.

위 방식들 중 Microsoft Office365를 이용한 인증은 2번이 아니라, 3번 방식을 사용합니다. 왜냐하면 Microsoft의 Office365는 Azure를 기반으로 하고 있고, 이는 Microsoft의 Cloud 서비스이기 때문에 언제든 열려 있는 서버이기 때문입니다.

#### 보안 공급자 등록 <a href="#undefined-1" id="undefined-1"></a>

1. 서버관리자에 로그인합니다. Office 365 인증(Microsoft Entra ID)은 HTTPS를 통한 암호화된 통신이 필요하므로 Forguncy Builder의 디버깅 실행에서는 동작을 확인할 수 없습니다. HTTPS를 활성화하고 Forguncy Server에 애플리케이션을 게시해야 합니다.
2.  \[타사] - \[업로드]을 클릭하여 다운로드한 ZIP 파일을 선택합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2618).png" alt=""><figcaption></figcaption></figure>
3.  등록이 완료되면 다음과 같이 표시됩니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2619).png" alt=""><figcaption></figcaption></figure>
4.  \[구성 추가]를 클릭합니다. 다음 그림과 같이 Office 365(Microsoft Entra ID) 인증을 사용하기 위해 설정이 필요한 항목이 표시됩니다. 다음 절차에서는 이러한 설정 값을 얻는 방법을 설명합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2620).png" alt=""><figcaption></figcaption></figure>



### 필요한 Microsoft Entra ID 설정 및 설정 값 확인

1.  Azure 포털의 왼쪽 메뉴에서 Entra ID > 앱 등록을 클릭합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2621).png" alt=""><figcaption></figcaption></figure>
2.  상단에 새로 만들기를 클릭합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2622).png" alt=""><figcaption></figcaption></figure>
3.  앱이름을    입력하고 등록버튼을 클릭합니다.   <br>

    <figure><img src="../../../.gitbook/assets/image (2623).png" alt=""><figcaption></figcaption></figure>
4.  만든 앱의 왼쪽 메뉴에서 인증서 및 암호를 클린한 후, 새 클라이언트 암호를 클릭합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2625).png" alt=""><figcaption></figcaption></figure>
5.  암호에 대한 설명과 사용 기간을 설정합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2626).png" alt=""><figcaption></figcaption></figure>
6. 비밀번호를 등록하면 아래와 같이 나타납니다.

<figure><img src="../../../.gitbook/assets/image (2627).png" alt=""><figcaption></figcaption></figure>

7.  Forguncy의 Office 365( Microsoft Entra ID ) 인증 공급자에서 기타 설정 페이지의 클라이언트 비밀에 클립보드에 복사한 값을 입력합니다<br>

    <figure><img src="../../../.gitbook/assets/image (2628).png" alt=""><figcaption></figcaption></figure>
8.  만든 앱의 왼쪽 메뉴에서 API 권한을 클릭합니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2629).png" alt=""><figcaption></figcaption></figure>
9.  작성한 앱의 개요 페이지를 표시하고 애플리케이션(클라이언트) ID와 디렉터리(테넌트) ID 의 두 값이 표시되는지 확인합니다 .<br>

    <figure><img src="../../../.gitbook/assets/image (2630).png" alt=""><figcaption></figcaption></figure>
10. 이전 단계에서 확인한 응용 프로그램(클라이언트) ID와 디렉터리(테넌트) ID의 두 값을 복사하고 Forguncy의 Office 365( Microsoft Entra ID ) 인증 공급자의 기타 설정 페이지에 있는 응용 프로그램(클라이언트) ID 및 디렉터리(테넌트) ID를 각각 입력합니다. 사용자 이름으로 사용할 필드를 ID 또는 사용자 주체 이름에서 선택합니다. 기본값은 'ID'입니다. \[확인] 버튼을 클릭하여 설정을 저장합니다 .<br>

    <figure><img src="../../../.gitbook/assets/image (2631).png" alt=""><figcaption></figcaption></figure>

### 리디렉션 URI 설정

1. 만든 앱의 개요 페이지를 표시하고 리디렉션 URI 추가를 클릭합니다.

<figure><img src="../../../.gitbook/assets/image (2632).png" alt=""><figcaption></figcaption></figure>

2. 플랫폼 추가를 클릭합니다.
3. 웹을 클릭합니다.\
   ![](<../../../.gitbook/assets/image (2633).png>)
4.  **\[리디렉션 URI]에 대상 응용 프로그램의 URL에 "/signin-oidc"를 붙인 문자열을 설정하고 \[구성] 버튼을 클릭합니다.**

    여러 Forguncy 응용 프로그램에서 본 인증 공급자의 인증을 사용하는 경우 각 리디렉션 URL을 추가합니다. 하나의 Microsoft Entra ID 앱에 대해 여러 리디렉션 URL을 설정할 수 있습니다.
5.  **대상 응용 프로그램에 액세스하는 데 도메인 이름을 사용하는 경우 Forguncy 서버관리자에서 도메인 이름을 설정하고 설정 저장 버튼을 클릭합니다.**

    호스트 이름이나 IP 주소를 사용하여 액세스하는 응용 프로그램의 경우 이 설정은 필요하지 않습니다.<br>

    <figure><img src="../../../.gitbook/assets/image (2634).png" alt=""><figcaption></figcaption></figure>

