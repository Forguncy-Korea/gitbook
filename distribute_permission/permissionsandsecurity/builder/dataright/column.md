# 열 권한

필드 권한은 사용자가 액세스할 수 있는 필드를 제어하는 열 권한입니다. 테이블에 필드 권한을 설정하면 다른 사용자가 다른 필드에 액세스하고 편집할 수 있는 다른 권한을 가질 수 있으므로 데이터 보호 역할을 할 수 있습니다.

필드 권한은 여러 권한 부여 항목 간의 관계인 권한 부여 항목 집합의 컬렉션으로, 권한 있는 프로젝트 중 하나의 조건을 충족하는 경우 적절한 권한이 있습니다.&#x20;

다른 사용자가 다른 필드에 대해 서로 다른 작업 권한을 가질 수 있도록 필드 권한을 설정하여 데이터 보호 효과를 얻을 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72356919/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092598000\&api=v2) 데이터 테이블을 열고 오른쪽 열 테이블 설정에서 열 권한 편집을 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (1406).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72356919/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092598000\&api=v2) 권한이 부여된 사용자를 설정합니다. 역할 열을 클릭하고 팝업 역할 목록에서 필드 권한을 부여하는 역할을 확인합니다. 예를 들어 "관리자"를 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (1888).png" alt=""><figcaption></figcaption></figure>



![](https://help.grapecity.com.cn/download/thumbnails/80944467/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923143000\&api=v2)  행 조건 필터를 설정하면 조건을 충족하는 레코드가 필터링되어 인증된 사용자가 해당 작업을 수행할 수 있습니다.

조건 필터 열을 클릭하여 조건을 설정합니다. 팝업 조건 필터 대화 상자에서 조건을 설정합니다. 예를 들어 아래 그림과 같이 두 번째 권한 제어의 조건을 "구매자는 로그인 사용자입니다"로 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (596).png" alt=""><figcaption></figcaption></figure>

필드 권한 열을 클릭하면 이 테이블의 모든 필드와 하위 테이블이 대화 상자에 나열되고 단일 필드와 하위 테이블의 작업 권한이 설정됩니다.

아래 그림과 같이 로그인한 사용자를 현재 사용자로 설정하면 모든 필드를 조회하고 편집할 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/80944467/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923143000\&api=v2)  볼 수 있는 모든 작업과 편집 가능한 모든 작업을 포함하여 허용되는 작업을 설정합니다. 필드 삭제는 필드 권한에서 허용되지 않습니다.

<figure><img src="../../../../.gitbook/assets/image (1978).png" alt=""><figcaption></figcaption></figure>

필드 권한 열을 클릭하면 이 테이블의 모든 필드와 하위 테이블이 대화 상자에 나열되고 단일 필드와 하위 테이블의 작업 권한이 설정됩니다.

아래 그림과 같이 로그인한 사용자를 현재 사용자로 설정하면 모든 필드를 조회하고 편집할 수 있습니다.

<figure><img src="../../../../.gitbook/assets/image (933).png" alt=""><figcaption></figcaption></figure>





![](https://help.grapecity.com.cn/download/thumbnails/72356919/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1648092598000\&api=v2) 설정이 완료되면 페이지를 실행하고 사용자 유재석 사용하여 로그인하면 관리자 역할이기 때문, 로그인하면 고객 이름 필드를 포함한 모든 주문 데이터를 볼 수 있습니다.

![](<../../../../.gitbook/assets/image (1815).png>)

조세호로 로그인하면 관리자 역할이 아니기 때문에 로그인 후 모든 주문을 볼 수 있지만 다른 고객의 주문 은 고객이름을 볼 수 없다.

![](<../../../../.gitbook/assets/image (1237).png>)

{% hint style="info" %}
뷰는 필드 권한을 설정할 수도 있지만 허용되는 작업은 모두 보거나 볼 수 있는 필드를 설정할지 여부만 설정할 수 있습니다.
{% endhint %}
