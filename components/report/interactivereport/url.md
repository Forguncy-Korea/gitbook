# URL 이동

보고서 요소에 대해 URL로 이동하도록 설정하면 미리 보기를 탭하여 이동할 수 있습니다.

이 섹션에서는 URL 이 효과를 구현하는 다양한 방법에 대해 설명합니다.

## 고정된 웹 사이트로 이동하기

URL을 웹 페이지 링크로 설정할 수 있으며 미리 볼 때 보고서 요소를 클릭하면 지정된 URL로 이동합니다.

예를 들어 새 보고서를 만들고, 텍스트 상자 구성 요소를 추가하고, 텍스트 "포건시  웹 사이트"를 입력합니다.

텍스트 상자 구성 요소를 선택하고 속성 설정 패널에서 드릴스루 옵션을 찾습니다. 드릴 유형을 URL로 이동으로 설정하고 URL을 포도 시티 웹 사이트의 웹 사이트 [https://www.grapecity.co.kr](https://www.grapecity.co.kr) 설정합니다.

![](<../../../.gitbook/assets/image (2163).png>)

보고서를 미리 보고 텍스트 상자 내용을 클릭하여 설정된 웹 페이지로 이동합니다.

![](<../../../.gitbook/assets/image (1415).png>)

## 표현식 동적 이동&#x20;

URL을 식으로 설정하여 식의 결과에 따라 URL을 동적으로 변경하여 지정된 여러 대상의 이동할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/65470911/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1634546503000\&api=v2) 다음 그림과 같이 데이터 테이블을 준비합니다.

![](<../../../.gitbook/assets/image (1800).png>)

![](https://help.grapecity.com.cn/download/thumbnails/65470911/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1634546503000\&api=v2)  새 보고서를 만듭니다.

![](https://help.grapecity.com.cn/download/thumbnails/65470911/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1634546502000\&api=v2)  테이블 구성 요소를 만들고, 필드 "세부사이트"를 바인딩하고, 두 번째 열에 "클릭"을 입력합니다. 테이블의 세 번째 열을 삭제하고 너비를 조정합니다.

![](<../../../.gitbook/assets/image (1437).png>)

![](https://help.grapecity.com.cn/download/thumbnails/65470911/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1634546502000\&api=v2)  점프를 설정합니다. \[클릭] 텍스트 상자를 선택하여 속성 설정 패널에서 \[작] 옵션을 찾습니다. 값 유형을 URL로 이동으로 설정합니다. 그런 다음 URL로 이동한 후 표현식을 선택합니다.![](https://help.grapecity.com.cn/download/thumbnails/65470911/image2021-3-23_13-48-5.png?version=1\&modificationDate=1634546502000\&api=v2)

![](<../../../.gitbook/assets/image (1296).png>)



![](https://help.grapecity.com.cn/download/thumbnails/65470911/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1634546502000\&api=v2)  표현식 편집기에 표현식(https://www.grapecity.co.kr/{세부사이트}) 을 입력하고 저장합니다.

![](<../../../.gitbook/assets/image (1034).png>)

![](https://help.grapecity.com.cn/download/thumbnails/65470911/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1634546502000\&api=v2)  보고서를 미리 봅니다. \[클릭]을 클릭하여  필드의 웹 페이지로 이동합니다.&#x20;

![](<../../../.gitbook/assets/image (1468).png>)
