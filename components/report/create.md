# 보고서 만들기

포건시에서 보고서를 만드는 방법을 설명합니다.

보고서 기능은 기본적으로 프로젝트  탐색기에 표시되지 않는 고급 기능입니다 . 보고서 앞의 확인란을 선택하고 "확인"을 클릭하여 개체 관리자에 보고서 개체를 표시합니다.

<figure><img src="../../.gitbook/assets/image (620).png" alt=""><figcaption></figcaption></figure>



### 보고서 작성&#x20;

보고서를 만들려면 먼저 보고서를 만드는 데 사용할 데이터 테이블을 준비해야 합니다.

![](https://help.grapecity.com.cn/download/thumbnails/56535984/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1614840355000\&api=v2) 보고서를 만듭니다. 개체 관리자의 보고서 탭에서 마우스 오른쪽 버튼을 클릭하거나 새로운보고서생성 또는 RDL 보고서 생성을 선택합니다.

또는 폴더 만들기를 선택하여 폴더에서 페이지 보고서를 만들거나 RDL 보고서를 만듭니다.

![](<../../.gitbook/assets/image (2192).png>)

리본 메뉴 모음에서 만들기를 클릭하고 보고서 영역에서 페이지 보고서 또는 RDL 보고서를 클릭할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/56535984/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1614841911000\&api=v2) 데이터 원본을 만듭니다. 보고서를 선택하고 마우스 오른쪽 버튼을 클릭한 다음 마우스 오른쪽 버튼 클릭 메뉴에서 데이터 소스 추가를 선택하여 보고서 데이터 원본 편집 대화 상자를 표시합니다.

![](<../../.gitbook/assets/image (402).png>)



![](https://help.grapecity.com.cn/download/thumbnails/56535984/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1614842570000\&api=v2) 데이터 원본을 편집합니다.

* 이름: 데이터 원본의 이름입니다.
* 테이블: 데이터의 출처 데이터 테이블을 선택합니다.
* 데이터 소스 파라미터 편집: 추가된 데이터 소스 파라미터는 쿼리 조건, 쿼리 행 수 등에서 사용할 수 있습니다.
* 선택: 데이터 테이블을 선택하면 기본적으로 데이터 테이블의 모든 필드가 선택 목록에 자동으로 추가됩니다. 필요에 따라 열을 추가하거나 제거할 수 있습니다.
* 쿼리: 데이터 테이블의 데이터에 대한 쿼리 조건을 설정합니다.
* 상위 제한: 데이터 테이블의 데이터에 대한 쿼리 행 수를 설정합니다.
* 정렬: 데이터 테이블의 데이터에 대한 데이터 정렬을 설정합니다.

![](<../../.gitbook/assets/image (2228).png>)

![](https://help.grapecity.com.cn/download/thumbnails/56535984/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1614846094000\&api=v2) 보고서를 편집합니다.<br>

(1) 구성 요소 요소를 추가합니다.

머리글을 추가합니다. 보고서-> 머리글 추가를 클릭합니다.

![](<../../.gitbook/assets/image (1821).png>)

테이블을 보고서 본문 영역으로 드래그합니다.

![](<../../.gitbook/assets/image (2071).png>)

마지막 열의 셀을 마우스 오른쪽 버튼을 클릭하고 팝업 메뉴에서 세로막대 -> 더보기 선택하고 숫자를 4로 조정하고 4 열을 추가한 다음 오른쪽에 열 삽입을 클릭하면 4개의 열이 삽입됩니다.

![](<../../.gitbook/assets/image (1358).png>)

(2) 바인딩 데이터. 표의 두 번째 행에 있는 셀을 선택하고 셀 내의 오른쪽을 클릭하여 바인딩할 데이터 원본의 필드를 선택합니다. 데이터 바인딩은 헤더 헤더와 바닥글 요약을 자동으로 채웁니다.![](https://help.grapecity.com.cn/download/thumbnails/50014533/image2018-6-13_15-46-27.png?version=1\&modificationDate=1591667990000\&api=v2)

![](<../../.gitbook/assets/image (2062).png>)

(3) 외관 최적화. 전체 테이블을 선택하여 보고서 본문 테두리로 확장합니다.

오른쪽의 속성 설정 패널에서 다음 그림과 같이 선택한 테이블 설정 테마 색상 스타일을 지정합니다.

![](<../../.gitbook/assets/image (1080).png>)

디자이너 메뉴 모음의 미리 보기 버튼을 클릭하여 보고서를 미리 봅니다.

![](<../../.gitbook/assets/image (1543).png>)

![](https://help.grapecity.com.cn/download/thumbnails/56535984/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1614849577000\&api=v2) 보고서 권한을 편집합니다. 보고서를 선택하고 마우스 오른쪽 버튼을 클릭한 다음 오른쪽 메뉴에서 보고서 권한 편집을 선택합니다. 팝업 대화 상자에서 보고서를 보고 내보낼 수 있는 역할을 선택합니다.

![](<../../.gitbook/assets/image (1816).png>)

![](https://help.grapecity.com.cn/download/thumbnails/56535984/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1614849926000\&api=v2) 보고서를 표시합니다.&#x20;

![](<../../.gitbook/assets/image (721).png>)

![](<../../.gitbook/assets/image (747).png>)

