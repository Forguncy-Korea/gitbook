# 테이블 행 번호

테이블에 행 번호를 추가하는 것은 그룹화 기능에 해당하는 실제 비즈니스에서 일반적인 요구 사항이며 테이블 행 번호는 전역 행 번호와 그룹 내 행 번호를 정렬하는 두 가지 방법을 모두 지원합니다.

전역 행 번호는 1부터 증가하는 전체 테이블을 정렬하는 범위입니다. 그룹 내 행 번호는 그룹 내에서만 정렬되며 각 그룹은 1부터 시작합니다.

이 섹션에서는 전역 행 번호와 그룹 내 행 번호를 추가하는 단계를 각각 설명합니다.

## 전역 줄 번호 추가&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/64456059/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1633752177000\&api=v2) 새 테이블을 만듭니다.

먼저 테이블을 만들고 다음 그림과 같이 필드를 바인딩합니다.

![](<../../../.gitbook/assets/image (475).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64456059/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1633752177000\&api=v2) 새 열이 추가되었습니다.

맨 왼쪽에 열을 추가하고 머리글 행에 전역 행 번호를 입력합니다.

![](<../../../.gitbook/assets/image (1291).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64456059/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1633752177000\&api=v2) 표현식 편집기를 엽니다.

전역 행 번호 세부 정보 셀을 마우스 오른쪽 버튼 클릭하고 **표현식을 선택합니다**.

![](<../../../.gitbook/assets/image (448).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64456059/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1633752177000\&api=v2) 식을 추가합니다.

오른쪽에서  RowNumber를  검색하여 오른쪽 표현식에 추가한 다음 저장을 클릭합니다.

![](<../../../.gitbook/assets/image (1491).png>)

![](https://help.grapecity.com.cn/download/thumbnails/64456059/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1633752177000\&api=v2) 보고서를 미리 보고 행 번호 효과를 확인합니다.
