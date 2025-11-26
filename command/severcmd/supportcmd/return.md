# 반환 명령 생성하기

&#x20;서버 명령을 실행할 때 이상이 발생할 수 있습니다. 문제를 찾아 해결하는 데 도움이 되도록 서버 명령을 실행할 때 발생하는 비정상적인 정보를 페이지에 반환하려면 반환 명령을 사용하십시오.

반환정보 중 반환값이 0인 경우에만 서버 명령이 성공적으로 실행되었음을 의미하고, 그 외의 반환값은 실행에 실패했음을 의미한다.

서버 명령의 트랜잭션 명령이 실행되지 않으면 트랜잭션 명령이 롤백됩니다(즉, 명령이 중지되고 완료된 작업이 무효화됩니다).





### 반환 명령&#x20;

다음은 서버 명령어에서 반 명령어를 사용하는 방법을 자세히 소개한 것이다.

**1.** 개체 관리자에서 서버 명령 라벨을 마우스 오른쪽 버튼으로 클릭하고 "서버 명령 생성"을 선택하면 서버 명령 생성 대화 상자가 나타납니다.

또는 "폴더 만들기"를 선택하여 폴더에 서버 명령을 만듭니다.

2. 서버 명령의 일반 설정을 편집합니다. 서버 명령의 이름을 "주문 상태 업데이트"로 설정합니다.

<figure><img src="../../../.gitbook/assets/image (273).png" alt=""><figcaption></figcaption></figure>

**3.** 서버 명령의 명령을 편집합니다. "명령 편집" 하이퍼링크를 클릭하여 서버 명령 편집 대화 상자를 열고 조건부 명령을 선택하십시오.

1. 조건을 설정합니다. 조건 명령의 "If" 뒤를 클릭하고 ![](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/80946969/image2018-12-24_10-57-30.png)"조건식"을 선택한 다음 "새 조건"을 클릭하고 필드를 "%CurrentUser.Role%"로, 작업을 "Equals"로, 값을 "Manager"로 설정합니다.

<figure><img src="../../../.gitbook/assets/image (225).png" alt=""><figcaption></figcaption></figure>

2. 하위명령을 설정합니다.&#x20;

설정이 완료되면 확인을 클릭하세요.

<figure><img src="../../../.gitbook/assets/image (226).png" alt=""><figcaption></figcaption></figure>

3. 조건부 분기를 추가합니다. "다른 항목 추가"를 선택한 후,

&#x20;      하위   명령으로 "반환명령 생성하기" 명령을 아래와 같이 설정합니다.

<figure><img src="../../../.gitbook/assets/image (227).png" alt=""><figcaption></figcaption></figure>

**4.**  서버 명령어가 생성된 후 서버 명령어를 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하여 버튼으로 설정합니다.&#x20;

명령을 "서버단 명령 호출"을 선택 한 후, 서버단 명령은 우리가 만든 "주문 상태 업데이트"를 선택합니다.

반환 값을 받을 셀도 설정합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (228).png" alt=""><figcaption></figcaption></figure>

**5.** 설정이 완료되면 "확인"을 클릭하여 대화 상자를 닫고 페이지를 실행하세요.

* 역할이 manager인 사용자 김매니저로 로그인합니다. 페이지에서 "주문 상태 업데이트" 버튼을 클릭하면 서버가 데이터 테이블 작업 명령을 실행하여 주문 상태를 업데이트하고, ID가 1인 주문의 제품명을 "1"로 변경됩니다.

<figure><img src="../../../.gitbook/assets/image (230).png" alt=""><figcaption></figcaption></figure>

* 관리자 권한이 없는 계정으로 로그인 하고, 버튼을 클릭하면 데이터테이블 업데이트 명령이 실행되지 않습니다. 반환명령의 반환코드가 반환됩니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (231).png" alt=""><figcaption></figcaption></figure>
