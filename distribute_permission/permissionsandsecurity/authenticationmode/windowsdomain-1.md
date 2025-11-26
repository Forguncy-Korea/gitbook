# Windows Active Directory

Active Directory 의 사용자, 조직 단위 등 정보를 포건시 사용자, 역할, 조직의 정보로 사용할 수 있습니다.

조직의 조직 역할, 리더 설정은 지원하지 않습니다.&#x20;

**절차를 따르십시오**

![](https://help.grapecity.com.cn/download/thumbnails/78807434/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1663723761000\&api=v2)

{% file src="../../../.gitbook/assets/ADSecurityProvider.zip" %}

를 클릭하여 패키지를 다운로드합니다.

사용자 계정 관리 인터페이스의 타사 영역에서 업로드를 클릭하고 ADSecurityProvider .zip 파일을 선택합니다.

<figure><img src="../../../.gitbook/assets/image (1988).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (294).png" alt=""><figcaption></figcaption></figure>



![](https://help.grapecity.com.cn/download/thumbnails/78807434/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1663723761000\&api=v2)**AD Provider를 업로드** 하시면 좌측 기본 설정 메뉴 중 기타 설정 항목이 생성됩니다.

기타 설정의 내용은 내부의 서버 담당자 또는 보안 담당자에게 문의를 하여 내용을 작성 후 적용해주십시오.

<figure><img src="../../../.gitbook/assets/image (905).png" alt=""><figcaption></figcaption></figure>

* 동기화 간격(분): 포건시는 보안 공급자로부터 얻은 사용자 정보를 캐시합니다. 자동 동기화 간격 설정은 포건시가 최신 사용자 정보 데이터를 자동으로 동기화하는 시간을 나타냅니다. 기본값은 20분입니다.
* 사용자 속성: 포건시가 사용자 속성에서 가져오는 속성을 나타냅니다. 포건시는 사용자 이름, 사서함 정보를 가져오고 더 많은 사용자 속성을 가져오도록 설정할 수 있습니다.&#x20;
* 그룹 종류: Windows 도메인에는 distributionGroup, securityGroup의 두 가지 유형의 그룹이 있습니다. 이 설정을 통해 사용자는 포건시에서 가져올 사용자 그룹을 결정할 수 있습니다.
* 그룹 필터: 모든 사용자 그룹을 사용할 수 있음을 나타내기 위해 비워 두면 여러 그룹 이름이 쉼표로 구분된 포건시에서 사용하는 그룹 이름을 설정합니다.

해당 설정을 완료하시면 기본 설정 목록 아래에 유저 목록이 생성되며 MS Exchange 서버에서 설정한 대로 표시됩니다.&#x20;

포건시는 메모리에 사용자 정보 데이터를 캐시하고 사용자가 Windows 도메인을 업데이트하면 20분 이내에 최신 정보를 얻을 수 있습니다. 페이지에서 동기화를 클릭하여 사용자 정보 데이터를 업데이트하거나 설정 추가에서 자동 동기화 간격을 변경하여 최신 사용자 정보 데이터를 자동으로 가져올 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/80942475/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923114000\&api=v2) 외부 인증 제공자 명을 클릭하면 AD서버에 등록된 사용자, 역할, 조직을 확인할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (2376).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80942475/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923114000\&api=v2) 포건시빌더의 리본메뉴에서 \[보안>인증모드]를 클릭 한 후, “외부서비스 인증"선택합니다.

<figure><img src="../../../.gitbook/assets/image (2378).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80942475/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923114000\&api=v2)포건시 빌더에서  \[배포>서버배포]를  클릭하여 배포를 합니다.

<figure><img src="../../../.gitbook/assets/image (2379).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80942475/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1673923114000\&api=v2)서버관리자의   \[앱목록]에서 배포한 앱에서 하단에 "통합"에서 ADSecurityProvider를 선택합니다.

<figure><img src="../../../.gitbook/assets/image (2377).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80942475/%E6%AD%A5%E9%AA%A47.png?version=1\&modificationDate=1673923114000\&api=v2) \[앱목록>모든앱목록]에서 배포한 앱을 재시작합니다.

<figure><img src="../../../.gitbook/assets/image (2380).png" alt=""><figcaption></figcaption></figure>
