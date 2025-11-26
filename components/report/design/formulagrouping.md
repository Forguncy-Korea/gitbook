# 식 그룹화

일반적으로 테이블에 그룹화를 추가한 후 데이터를 그룹화하여 표시할 수 있습니다. 예를 들어 그룹 바인딩은 판매 지역이며 각 지역은 하나의 그룹에 해당합니다.

그러나 필요한 그룹화 조건은 다음 그림과 같이 주문 날짜의 월로 데이터를 그룹화하는 등 데이터베이스에 직접 존재하지 않지만 데이터베이스에는 주문 날짜가 저장됩니다.

이렇게 하려면 그룹화할 때 식을 사용하여 그룹화해야 합니다.

## 식 그룹화&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/64455871/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1633694861000\&api=v2) 새 테이블을 만듭니다.

새 보고서를 만들고 데이터 원본을 추가합니다. 테이블 구성 요소를 추가하고, 데이터 필드를 바인딩하고, 테이블을 적절하게 확장합니다.&#x20;

![](<../../../.gitbook/assets/image (1817).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64455871/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1633694861000\&api=v2) 그룹화를 추가합니다.

테이블의 셀을 클릭하여 테이블에 테이블 그룹화 창이 표시되도록 한 다음 주문 날짜를 테이블 그룹화 창으로 드래그하면 테이블에 그룹화가 나타납니다.

![](<../../../.gitbook/assets/image (2077).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64455871/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1633694861000\&api=v2) 사용정 그룹화 식입니다.

\[테이블 그룹화] 창에서 \[양식 1\_주문 날짜 1]을 클릭하여 속성 설정 패널의 그룹화 조건 표현식을 **{Month(주문 날짜)}**&#xB85C; 변경합니다.

함수 Month의 사용법은 Year/Quarter/Month/Day 함수 예제 -연도 분기 월일 가져오기를 참조하십시오.

보시다시피 그룹화 조건은 실제로 식이며 그룹화 필드를 바인딩할 때 자동으로 생성됩니다. 그룹화 조건은 여기에서 사용정 편집되며 데이터는 편집된 식에 따라 그룹화할 수 있습니다.

![](<../../../.gitbook/assets/image (345).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64455871/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1633694861000\&api=v2)그룹 헤더 표현식을 수정합니다.

그룹 헤더 셀 표현식을 "{Month(주문 일자)}월"로 조정하여 그룹 헤더가 "1월, 2월, 3월"로 표시되도록 합니다.

![](<../../../.gitbook/assets/image (1886).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64455871/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1633694861000\&api=v2) 보고서를 미리 봅니다.

표시되는 데이터는 월별로 그룹화되어 표시됩니다.

![](<../../../.gitbook/assets/image (638).png>)
