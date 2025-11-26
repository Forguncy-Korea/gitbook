# 루프 명령

서버단 명령에서 루프 명령을 사용하여 특정 루프 방식으로 하나 또는 하나의 하위 명령 집합을 반복할 수 있습니다.

## 루프 명령&#x20;

예를 들어 디자이너에는 주문 테이블이 있고 서버 쪽의 순환 명령을 사용하여 테이블 1에 주문 테이블의 데이터를 추가할 수 있는 테이블 1이 있습니다.

다음은 서버 명령에서 루프 명령을 사용하는 방법에 대한 자세한 설명입니다.

**절차를 따르십시오**

![](https://help.grapecity.com.cn/download/thumbnails/72358105/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092615000\&api=v2)  개체 관리자의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 \[서버단 명령 생성하기]를 선택하여 서버단 명령 만들기 대화 상자를 나타납니다.

또는 폴더 만들기를 선택하여 폴더에 서버 명령을 만듭니다.

![](<../../../.gitbook/assets/image (819).png>)

리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버단 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72358105/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092615000\&api=v2)  서버 명령의 일반 설정을 편집합니다. 서버 명령의 이름을 "루프 명령"으로 설정합니다.

![](<../../../.gitbook/assets/image (1810).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358105/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092615000\&api=v2) 서버 명령의 파라미터를 편집합니다. 배열 형식의 파라미터 "고객 주문 테이블"을 추가하고 두 개의 배열 항목을 추가합니다.

![](<../../../.gitbook/assets/image (2104).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358105/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092615000\&api=v2)  서버단 명령을 편집하는 명령입니다. \[명령 편집] 하이퍼링크를 클릭하고 서버단 명령 실 대화 상자를 표시하고 명령선택에서 "루프 명령 만들기"를 선택합니다.

* 반복 횟수 : 루프 수 또는 루프 배열을 지정할 수 있습니다.
* 반복 항목/배열 인덱스 파라미터 이름: 현재 루프 인덱스 값을 설정하는 변수 이름입니다.
* 반복 항목 / 배열 대상 객체 파라미터 이름 : 현재 루프 개체의 변수 이름을 설정합니다.

예를 들어 루프의 배열을 지정하고 클릭 하 고 팝업 대화 상자의 매개 변수 목록에서 고객 주문 테이블을 두 번 클릭 하 여 삽입 합니다.![](https://help.grapecity.com.cn/download/thumbnails/72358105/image2020-3-11_14-53-23.png?version=1\&modificationDate=1648092614000\&api=v2)

![](<../../../.gitbook/assets/image (1578).png>)

루프의 하위 명령을 "데이터 테이블 업데이트하기"로 선택하고 작업 유형은 추가되고 대상 테이블은 테이블 1입니다.

![](<../../../.gitbook/assets/image (1190).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358105/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1648092615000\&api=v2)  서버단 명령이 생성되면  서버단 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼으로 설정합니다. 버튼의 명령편집을 하 루프 명령으로 선택합니다.

파라미터 목록에서 파라미터를  "고객 주문 테이블"의 값을 설정합니다. 값 뒤에 있는 버튼 클릭하여 테이블에서 데이터 선택 대화 상자를 표시합니다. 테이블 이름과 범위를 선택하고 데이터 그룹에 대한 열 이름을 설정합니다. 페이지에서 테이블의 열 이름을 미리 설정해야 합니다.![](https://help.grapecity.com.cn/download/thumbnails/72358105/image2020-3-11_15-5-23.png?version=1\&modificationDate=1648092614000\&api=v2)

![](<../../../.gitbook/assets/image (1529).png>)

파라마터를 설정한 후 고급 설정에서 "연결 데이터를 최신 정보로 업데이트하기"를 선택합니다.

![](<../../../.gitbook/assets/image (1117).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358105/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092615000\&api=v2)  설정이 완료되면 확인을 클릭하여 대화 상자를 닫고 페이지를 실행합니다，페이지에서 데이터 추가 버튼을 클릭하면 서버는 반복 명령의 데이터 테이블 작업 명령을 실행하여 주문 테이블의 각 행에 대해 기록된 주문 번호와 고객 이름 필드 루프를 테이블 1에 추가합니다.

![](<../../../.gitbook/assets/image (2011).png>)
