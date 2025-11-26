# 사용자 생성 (Office 365 계정으로 로그인)



아래 절차대로 진행하 사용자 생성을 할 수 있습니다.&#x20;

1. Azure 열기 : [https://portal.azure.com/#home](https://portal.azure.com/#home)

<figure><img src="../../../../.gitbook/assets/image (1902).png" alt=""><figcaption></figcaption></figure>

2\. Azure Active Directory로 이동&#x20;

<figure><img src="../../../../.gitbook/assets/image (856).png" alt=""><figcaption></figcaption></figure>

3\. 앱 등록을 선택합니다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (1660).png" alt=""><figcaption></figcaption></figure>

4\. 새 등록을 선택합니다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (1581).png" alt=""><figcaption></figcaption></figure>

5\. 애플리케이션 등록&#x20;

<figure><img src="../../../../.gitbook/assets/image (713).png" alt=""><figcaption></figcaption></figure>

&#x20;(1) 먼저, 앱 이름을 지정합니다.&#x20;

&#x20;(2) 다음은 "지원되는 계정 유형(Supported Account Types)"에서 아래 항목을 선택합니다.

&#x20;  \- 모든 조직 디렉터리의 계정(모든 Azure AD 디렉터리 - 다중 테넌트) 및 개인 Microsoft 계정(예: Skype, Xbox)

&#x20;  \- Accounts in any organizational directory (Any Azure AD directory - Multitenant) and personal Microsoft accounts (e.g. Skype, Xbox)

&#x20;(3) Redirect URI는 일단 아무 주소나 입력해 두세요. 나중에 변경해야 합니다. 이후에 다시 설명합니다.&#x20;



**6.** 등록하면 다음의 정보들이 화면에 표시됩니다. 아래 정보들을 메모장 등에 저장해 두십시오.

<figure><img src="../../../../.gitbook/assets/image (1045).png" alt=""><figcaption></figcaption></figure>

7\. Certificate & secrets을 선택하여 Client Secret을 가져옵니다.&#x20;

Azure는 한글판과 영문판의 아래 정보가 순서가 섞여 있으므로 한글과 영문을 아래와 같이 묶어 둡니다.&#x20;

&#x20;(1) 애플리케이션(클라이언트) ID - Application(Client) ID

&#x20;(2) 디렉터리(테넌트) ID - Directory(Tenant)ID

&#x20;(3) 개체 ID - Object ID

8\. 새 클라이언트 비밀. 비밀번호는 반드시 기억해 두세요. 그렇지 않으면 로그아웃 후 영구적으로 잃어버리게 됩니다.(이 경우 새로운 비밀번호를 생성할 수 있습니다.)



<figure><img src="../../../../.gitbook/assets/image (1012).png" alt=""><figcaption></figcaption></figure>

9\. 암호에 대한 설명과 사용 기간을 설정합니다.



<figure><img src="../../../../.gitbook/assets/image (1650).png" alt=""><figcaption></figcaption></figure>

10\. 비밀번호를 등록하면 아래와 같이 나타납니다.



<figure><img src="../../../../.gitbook/assets/image (2263).png" alt=""><figcaption></figcaption></figure>
