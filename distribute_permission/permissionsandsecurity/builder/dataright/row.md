# 행 권한

테이블에 행 권한을 설정하면 다른 사용자가 테이블의 데이터에 액세스, 편집 및 삭제할 수 있는 다른 권한이 있을 수 있으므로 데이터 보호 역할을 할 수 있습니다.

행 권한은 여러 권한 부여 항목 간의 관계인 권한 부여 항목 집합의 컬렉션으로, 권한 있는 항목의 조건을 충족하는 경우 적절한 권한이 있습니다.

서로 다른 사용자가 다른 사용 권한 작업 테이블의 데이터를 가질 수 있도록 다른 사용자에 대해 서로 다른 행 권한을 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72356890/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092598000\&api=v2) 데이터 테이블을 열고 오른쪽 열 테이블 설정에서 행 권한 설정을 선택하고, 권한편집을 클릭합니다.

<figure><img src="../../../../.gitbook/assets/image (1410).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72356890/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092598000\&api=v2) 권한이 부여된 사용자를 설정합니다. 팝업 역할 목록에서 행 권한을 부여하는 역할을 선택하려면 역할 열을 클릭하십시오. 예를 들어 "로그인 사용자"를 선택합니다.



<figure><img src="../../../../.gitbook/assets/image (1349).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80944438/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923142000\&api=v2)  행 조건 필터를 설정하면 조건을 충족하는 레코드가 필터링되어 인증된 사용자가 해당 작업을 수행할 수 있습니다.

조건 필터 열을 클릭하여 조건을 설정합니다. 팝업 조건 필터 대화 상자에서 조건을 설정합니다. 예를 들어 아래 그림과 같이 "모든데이터"로 조건을 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (921).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (1485).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80944438/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923142000\&api=v2)  보기, 편집 및 삭제를 포함하여 허용되는 작업을 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (1405).png" alt=""><figcaption></figcaption></figure>



![](https://help.grapecity.com.cn/download/thumbnails/80944438/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923142000\&api=v2)  데이터 테이블에 하위 테이블이 있는 경우![](https://help.grapecity.com.cn/download/thumbnails/80944438/image2023-2-23_14-47-12.png?version=1\&modificationDate=1677134832000\&api=v2), "기본 테이블 권한의 하위 테이블 설정 사용"을 선택하여 기본 테이블과 일치하는 하위 테이블의 권한 설정을 만들 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72356890/%E6%AD%A5%E9%AA%A47.png?version=1\&modificationDate=1648092598000\&api=v2) 설정이 완료되면 페이지를 실행하고 사용자 A  로그인하면 로그인 한 후 구매자가 A 인 주문만 볼 수 있으며 편집 및 삭제 작업을 수행 할 수 있습니다.

{% hint style="info" %}
뷰는 행 권한을 설정할 수도 있지만 허용되는 작업은 볼 수 있는지 여부만 설정할 수 있습니다.
{% endhint %}
