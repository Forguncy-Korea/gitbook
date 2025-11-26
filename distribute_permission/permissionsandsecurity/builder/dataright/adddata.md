# 데이터 추가/생성 권한 편집

조건에 따라 사용자가 데이터를 만들 수 있는 권한이 있는지 여부를 제어합니다. 데이터 만들기 권한 항목 간의 설정 또는 관계, 즉 사용 권한 항목의 조건을 충족하면 데이터를 만들 수 있는 권한이 있으며 그렇지 않으면 사용 권한이 없습니다.

## 데이터 추가/생성 권한 만들기&#x20;

다음과 같이 데이터 테이블에 데이 만들기 권한을 설정하고 사용자 또는 역할이 데이터를 만들 수 있는 권한을 제어합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72356953/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092599000\&api=v2) 데이터 테이블을 열고 테이블 설정에서 데이터 추가/생성 권한 편집을 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (1966).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72356953/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092599000\&api=v2) 권한이 부여된 사용자를 설정합니다. 역할 열을 클릭하고 팝업 역할 목록에서 레코드 생성 권한을 부여하는 역할을 확인합니다. 예를 들어 "로그인 사용자"를 선택합니다.

<figure><img src="../../../../.gitbook/assets/image (1752).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80944501/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923143000\&api=v2)  행 조건 필터를 설정하면 조건을 충족하는 레코드가 필터링되어 인증된 사용자가 해당 작업을 수행할 수 있습니다.

조건 필터 열을 클릭하여 조건을 설정합니다. 팝업 조건 필터 대화 상자에서 조건을 설정합니다. 예를 들어 아래 그림과 같이 "주문 날짜가 2023/1/1보다 큼"으로 조건을 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (1965).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80944501/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923143000\&api=v2)  설정이 완료되면 페이지를 실행하고 사용자 유재석을 사용하여 로그인하고 로그인 한 후 새 데이터를 추가합니다.

* 주문 날짜가 2019/1/1보다 작으면 레코드 생성이 실패합니다.

![](<../../../../.gitbook/assets/image (366).png>)

주문 날짜가 2019/1/1보다 크면 레코드가 성공적으로 만들어집니다.
