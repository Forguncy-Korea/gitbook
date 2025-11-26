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



### 로그인 모드&#x20;

로그인 모드에는 Office365 사용자 연동명령과, Office 365 통합인증 명령이 있습니다.&#x20;

* [Office365 사용자 연동 명령](/broken/pages/KGV23hc6OMBMxKUtuIoN) : Office365 계정으로만 로그인 할 수 있으며, 설정이 간단함&#x20;
* [Office365 통합인증 명령](office365/undefined.md) : Office 365 계정 또는 기본 제공 사용자로 로그인할 수 있으며, 설정이 복잡함&#x20;

### 사용방법&#x20;

1. 플러그을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3. Office 365 로그인은 서버명령에서만 사용되며, [Office365 통합인증 명령](office365/undefined.md)을 사용할 수 있다. 자세한 사항은 링크를 통해 확인할 수 있습니다. &#x20;
