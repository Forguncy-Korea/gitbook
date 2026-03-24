# Office 365 로그인(Office365LoginCommand)

포건시 로그인의 종류는 크게 총 3가지로 볼 수 있습니다.&#x20;

1. Forguncy 인증 : 포건시 서버 자체에서 사용자 관리
2. Windows 인증 : Microsoft사의 Active Directory를 연동한 사용자 관리
3. 제3자 인증 : 네이버, 카카오, 구글, 페이스북 등 타사의 로그인을 연동한 사용자 관리

포건시로 앱을 만드는 개발자는 위 3가지 중 1가지를 택하여 사용자 로그인 방식으로 채택하실 수 있습니다.

위 방식들 중 Microsoft Office365를 이용한 인증은 2번이 아니라, 3번 방식을 사용합니다. 왜냐하면 Microsoft의 Office365는 Azure를 기반으로 하고 있고, 이는 Microsoft의 Cloud 서비스이기 때문에 언제든 열려 있는 서버이기 때문입니다.

해당 플러그인을 사용하기 위해서는 [Office 365 Client ID와 TenantID](office-365.md)가 필요합니다.&#x20;

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/Office365LoginCommand.zip">Office365LoginCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/Office365LoginCommand.zip">Office365LoginCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/Office365LoginCommand.zip">Office365LoginCommand.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/Office365LoginCommand.zip">Office365LoginCommand.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/Office365LoginCommand.zip">Office365LoginCommand.zip</a></td></tr></tbody></table>



### 보안 공급자 등록

1. 서버관리자에 로그인합니다.\
   Office 365 인증(Microsoft Entra ID)은 HTTPS를 통한 암호화된 통신이 필요하므로 Forguncy Builder의 디버깅 실행에서는 동작을 확인할 수 없습니다. HTTPS를 활성화하고 Forguncy Server에 애플리케이션을 게시해야 합니다.
2.  **\[타사] - \[업로드]을 클릭하여 다운로드한 ZIP 파일을 선택합니다.**<br>

    <figure><img src="../../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
3. **등록이 완료되면 다음과 같이 표시됩니다.**

<figure><img src="../../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

\[구성 추가]를 클릭합니다.  다음 그림과 같이 Office 365(Microsoft Entra ID) 인증을 사용하기 위해 설정이 필요한 항목이 표시됩니다. 다음 절차에서는 이러한 설정 값을 얻는 방법을 설명합니다.

<figure><img src="../../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
