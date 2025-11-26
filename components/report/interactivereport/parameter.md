# 매개변수를 이용한 보고서 이동

보고서는 보고서 이동 작업을 통해 대화형 데이터 프레젠테이션 및 분석을 가능하게 합니다. 예를 들어 기본 보고서에 요약된 데이터를 표시한 다음 마우스 클릭 한 번으로 더 자세한 데이터를 볼 수 있습니다.

다음 그림에서 기본 보고서는 장소별 물가내역이고 장소 클릭하면 해당 지역의 특정  물가 정보를 볼 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/65470864/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1634541524000\&api=v2) 기본 보고서를 만듭니다. RDL 보고서를 만들고 보고서 데이터 원본을 추가합니다.

기본 보고서 내용을 편집합니다. 다음 그림과 같이 차트 어셈블리 및 테이블릭스를 추가하여 데이터 바인딩을 수행하고 차트 제목을 수정합니다.

![](<../../../.gitbook/assets/image (1991).png>)

보고서 이름을 상위보고-하위보고서로 설정하는 등 기본 보고서를 저장합니다.

![](https://help.grapecity.com.cn/download/thumbnails/65470864/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1634541524000\&api=v2) 하위 보고서를 만듭니다. 기본 보고서가 하위 보고서로 드릴스루될 때 데이터 필터링을 구현하려면 하위 보고서에서 장소 변수 추가와 같은 보고서 매개 변수를 미리 설정해야 합니다.

![](<../../../.gitbook/assets/image (1316).png>)

다음 그림과 같이 차트 구성 요소 및 테이블 구성 요소를 추가하여 데이터 바인딩을 수행하고 차트 제목을 수정합니다.

차트와 테이블에 대한 필터를 설정합니다.

![](<../../../.gitbook/assets/image (2150).png>)

![](<../../../.gitbook/assets/image (1225).png>)

보고서를 미리 봅니다. 장소 통해 데이터를 필터링할 수 있는지 확인합니다.

보고서 이름을 보고서 드릴스루 하위 보고서로 설정하는 등의 하위 보고서를 저장합니다.

![](https://help.grapecity.com.cn/download/thumbnails/65470864/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1634541524000\&api=v2) 드릴 관계를 설정합니다. 기본 보고서를 열고 편집 상태로 이동하여 차트의 도면 영역을 선택합니다. 드릴스루 작업 섹션에서 드릴 유형을 보고서로 이동을 선택하고 점프 대상 보고서를 하위 보고서 드릴스루 하위 보고서로 지정합니다( 아래 그림 참조).

![](<../../../.gitbook/assets/image (1257).png>)

\[매개변수] 오른쪽에 있는 아이콘을 클릭하여 매개변수 리스트를 확장합니다.![](https://help.grapecity.com.cn/download/thumbnails/65470864/image2021-10-18_16-33-55.png?version=1\&modificationDate=1634546036000\&api=v2)

![](<../../../.gitbook/assets/image (1554).png>)

\[항목 추가]를 클릭한 후 \[장소]라는 매개 변수를 설정한 다음 매개 변수 뒤에 있는 설정 버튼을 클릭하여 다음 그림과 같이 매개 변수 값 데이터를 장소로 지정합니다.![](https://help.grapecity.com.cn/download/thumbnails/65470864/image2021-10-18_16-34-37.png?version=1\&modificationDate=1634546078000\&api=v2)

![](<../../../.gitbook/assets/image (1121).png>)

보고서가 미리 봅니다. 열 차트에서 막대를 클릭하면 보고서가 해당 지역의 세부 정보로 드릴스루되어 원하는 결과를 얻을 수 있습니다.

![](<../../../.gitbook/assets/image (1440).png>)

마찬가지로 테이블릭의 장소 및 물가 요약에 대해 동일한 보고서 드릴스루 동작이 추가됩니다.

![](<../../../.gitbook/assets/image (2279).png>)

![](<../../../.gitbook/assets/image (1380).png>)

![](https://help.grapecity.com.cn/download/thumbnails/65470864/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1634541524000\&api=v2) 보고서를 미리 보고 차트의 막대 또는 테이블릭스의 지역 또는 금액을 클릭하면 드릴스루됩니다.

{% hint style="info" %}
하위 보고서의 차트 제목을 표현식 "**{@판매 지역} 각 지방 판매 분석**"으로 변경하면 현재 필터링된 지역의 이름이 표시됩니다.&#x20;
{% endhint %}
