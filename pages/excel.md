# Excel에서 가져오기

Excel 시트를 로드하고, Excel 내의 셀을 자동 인식하여 애플리케이션의 화면이 되는 필드나 리스트 뷰의 자동 생성, 각 페이지(등록, 리스트, 상세, 편집)의 자동 생성, 필요한 테이블 의 자동 작성을 합니다.

{% hint style="info" %}
기존 프로젝트에 Excel 시트에서 테이블을 추가하려면 E[xcel 파일에서 테이블 만들기](../database/setdata/excel.md)를 참조 하십시오 . 마찬가지로 페이지를 추가하려면 [Excel에서 페이지 만들기](../components/excel.md)를 참조하십시오.
{% endhint %}

1.  **파일 > 새로 만들기를 클릭한 다음 "Excel에서 가져오기"를 클릭합니다.**

    <figure><img src="../.gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>
2. Excel 파일을 엽니다.

<figure><img src="../.gitbook/assets/image (311).png" alt=""><figcaption></figcaption></figure>

3.  **입력 값을 삭제하고 다음을 클릭합니다.**

    이 화면은 가져온 Excel 시트에 데이터(입력 값)가 포함된 경우 해당 값을 삭제하는 단계입니다. 입력 값을 삭제하면 후속 단계에서 수행되는 입력 항목의 자동 감지 정확도가 향상됩니다.

<figure><img src="../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>

4.  **\[데이터 Excel 로드]를 클릭하여 입력 값이 포함된 Excel 파일을 선택하고 다음을 클릭합니다.**

    이 화면은 미리 Excel 파일에 입력된 값을 초기 데이터로 가져오는 단계입니다. 입력 값이 포함된 Excel 파일을 가져오면 다음 단계에서 수행하는 입력 항목의 자동 검색 정확도가 더욱 향상됩니다.

    입력 값이 포함된 Excel 시트를 가져오지 않으려면 다음 버튼을 클릭하여 이 단계를 건너뛸 수 있습니다.

<figure><img src="../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>

5. **자동 감지된 입력 항목을 적용하려면 "예"를 클릭합니다.**

<figure><img src="../.gitbook/assets/image (314).png" alt=""><figcaption></figcaption></figure>

6. **입력 항목을 설정 해제하고 \[다음]을 클릭합니다.**

입력 항목으로 설정된 셀은 파란색 배경에 흰색 문자로 항목 이름을 표시합니다. 항목 이름은 셀을 두 번 클릭하여 변경할 수 있습니다. 목록에 입력 항목이 있는 경우 전체 셀을 목록 보기 영역으로 설정합니다.

<figure><img src="../.gitbook/assets/image (315).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="274">항목 </th><th>설명 </th></tr></thead><tbody><tr><td>필드 추가 </td><td>선택한 셀을 사용자 입력 항목으로 설정합니다.</td></tr><tr><td>필드 제거 </td><td>입력 항목으로 설정된 셀을 해제합니다.</td></tr><tr><td>세부정보 테이블 추가 </td><td>선택한 셀 범위를 목록 보기 영역으로 설정합니다.</td></tr><tr><td>세부정보 테이블 제거 </td><td>리스트뷰 영역으로 설정된 셀 범위를 해제합니다.</td></tr><tr><td>자동탐색 </td><td>입력 항목을 자동으로 감지합니다.</td></tr></tbody></table>

7. **셀 유형을 설정하고 \[다음]을 클릭합니다.**

텍스트, 숫자 등 페이지의 셀유형에 맞게 설정합니다.

<figure><img src="../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>

콤보박스나 라디오 버튼을 사용하면 아래와 같이 항목을 설정할 수 있습니다.

<figure><img src="../.gitbook/assets/image (318).png" alt=""><figcaption></figcaption></figure>

8. **생성할 테이블을 설정하고 마침을 클릭합니다.**

생성할 테이블 이름을 지정할 수 있습니다.

테이블 생성과 동시에 다음 각 페이지를 자동으로 만들 수 있습니다.

<figure><img src="../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure>

| 항목      | 설명                 |
| ------- | ------------------ |
| 목록 페이지  | 테이블 데이터를 나열하는 페이지. |
| 세부 페이지  | 테이블 데이터를 나열하는 페이지. |
| 페이지 추가  | 테이블에 데이터를 등록하는 페이지 |
| 페이지 편집  | 테이블 데이터를 편집할 페이지   |

9. 테이블이 생성됩니다.&#x20;

<figure><img src="../.gitbook/assets/image (321).png" alt=""><figcaption></figcaption></figure>

10. **필요한 경우 테이블 이름, 필드 이름 및 필드의 데이터 형식을 변경합니다.**
