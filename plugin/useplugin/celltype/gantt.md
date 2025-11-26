# 간트차트 (Gantt)

{% file src="../../../.gitbook/assets/ganttchart_7.105.fgko" %}

간트차트 플러그인을 이용하여 간트차트를 사용할 수 있습니다. 간트차트는 선 그래프로 가로축은 시간, 세로축은 진행 중인 프로젝트, 선은 해당 기간의 계획 및 실제 상황을 나타냅니다.&#x20;

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/Gantt.zip">Gantt.zip</a></td></tr><tr><td>v 9.0 </td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/Gantt.zip">Gantt.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/Gantt.zip">Gantt.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/Gantt.zip">Gantt.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/Gantt.zip">Gantt.zip</a></td></tr></tbody></table>

### 최소 구성만 사용하는 방법&#x20;

<figure><img src="../../../.gitbook/assets/image (515).png" alt=""><figcaption></figcaption></figure>

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3. 아래의 간트차트를 만드는데 필수사항인 필드를 가진 데이터 테이블을 생성합니다.

<table><thead><tr><th width="88"></th><th width="146">필드명 </th><th width="344">설명 </th><th>필드유형 </th></tr></thead><tbody><tr><td>1</td><td>ID </td><td>작업 고유 ID는 데이터베이스에서 자동으로 생성되는 기본 키여야 합니다.</td><td>int</td></tr><tr><td>2</td><td>Order</td><td>작업은 행마다 의미가 다르며 Level 필드를 함께 사용하여 작업을 상위 및 하위 수준과 구분하면 플러그인이 자동으로 업데이트합니다.</td><td>int</td></tr><tr><td>3</td><td>Level</td><td>작업 레벨, 최상위 레벨은 0입니다. 여러 루트 작업을 만들 수 없습니다. 예를 들어 2레벨  아래에 1레벨을 만들려고 하면 허용되지 않습니다.</td><td>int</td></tr><tr><td>4</td><td>Name</td><td>작업 명 </td><td>string</td></tr><tr><td>5</td><td>Depends</td><td>작업이 완료된 후(며칠) 이 작업을 시작합니다.</td><td>string</td></tr><tr><td>6</td><td>Start</td><td>작업 계획 시작 시간</td><td>OADATA</td></tr><tr><td>7</td><td>Duration</td><td>작업 계획 기간</td><td>int</td></tr><tr><td>8</td><td>Pre_work</td><td>사전 작업 </td><td>int</td></tr><tr><td>9</td><td>End</td><td>작업 계획 종료 시간 </td><td>OADATA</td></tr></tbody></table>

{% hint style="info" %}
* Name 필드 : 이름이 비어있으면 작업이 삭제되었음을 의미합니다. 따라서 새 작업을 만들거나 작업 이름을 공백으로 두고 삭제 버튼을 클릭하면 "삭제할 작업을 선택하십시오"라는 오류 메시지가 표시됩니다
{% endhint %}

4\. 3번에서 만든 데이터테이블을 연결한 리스트뷰를 페이지에 생성합니다.&#x20;

5\.  1) 리스트뷰를 선택한 후, 오른쪽 마우스 버튼 클릭 메뉴에서 "각 열에 이름 자동 생성"을 클릭합니다.

&#x20;        셀 영역을 선택하고, 셀 유형을 간트차트를 선택합니다.&#x20;

&#x20;    2\) 오른쪽 메뉴에서 "간트 차트 구성"을 클릭합니다.

&#x20;    3\) 간트차트구성 대화상자에서 아래와 같이 설정합니다.&#x20;

&#x20;         \* 리스트뷰 선택 : 4번에서 생성한 리스트뷰

&#x20;         \* 필수 값 : 3번에서 만든 필드와 연결&#x20;

<figure><img src="../../../.gitbook/assets/image (1625).png" alt=""><figcaption></figcaption></figure>

### 간트차트 툴바 설명

<figure><img src="../../../.gitbook/assets/image (1443).png" alt=""><figcaption></figcaption></figure>

![](<../../../.gitbook/assets/image (1780).png>): 현재 작업(task) 위에  작업 추가

![](<../../../.gitbook/assets/image (1860).png>): 현재 작업(task) 아래에 작업 추가&#x20;

![](<../../../.gitbook/assets/image (579).png>): 현재 작업 수준(Level) 줄이기 ,가장 높은 작업수준(Level)은 단일노드 (Leaf node)

![](<../../../.gitbook/assets/image (2008).png>): 현재 작업 수준 올리기

![](<../../../.gitbook/assets/image (1176).png>): 같은 수준(Level)에서 현재 작업을 위로 이동&#x20;

![](<../../../.gitbook/assets/image (1872).png>): 같은 수준(Level)에서 현재 작업을 아래로 이동&#x20;

![](<../../../.gitbook/assets/image (1651).png>):  현재 작업 삭제&#x20;

![](<../../../.gitbook/assets/image (622).png>) :  현재 작업의 서브작업 확장&#x20;

![](<../../../.gitbook/assets/image (2042).png>):  현재 작업의 서브작업 축소&#x20;

![](<../../../.gitbook/assets/image (1492).png>) : 시간 단위(월 → 주)를 줄이고 오른쪽 보기의 크기를 늘림&#x20;

![](<../../../.gitbook/assets/image (1684).png>) : 시간 단위(월 → 주)를 늘리고 오른쪽 보기의 크기를 줄임&#x20;

![](<../../../.gitbook/assets/image (649).png>):  오른쪽 그래프 화면으로 전체보기&#x20;

![](<../../../.gitbook/assets/image (688).png>): 왼쪽 편집 화면과 오른쪽 그래프 화면으로 나누기&#x20;

![](<../../../.gitbook/assets/image (1877).png>): 왼쪽 편집 화면으로 전체보기&#x20;

![](<../../../.gitbook/assets/image (2007).png>): 크리티컬 패스(critical path) 하이라이트

![](<../../../.gitbook/assets/image (859).png>): 작업 상태 색상 표시/표시안하기&#x20;

![](<../../../.gitbook/assets/image (1730).png>): 오른쪽 그래프의 표시 방식 전환: 계획만 표시, 계획 표시, 실제 표시.

&#x20;        (actualStart 및 actualEnd 컬럼을 설정하지 않으면 이 버튼이 나타나지 않습니다.)

![](<../../../.gitbook/assets/image (1644).png>): 저장 버튼, 테이블에 데이터를 저장

&#x20;        (데이터는 테이블에 제출하게 되며 테이블 테이블을 데이터베이스에 제출할지 여부는 사용자가 설정    합니다. 데이터 -> 데이터 제출 방법 -> 데이터 느슨한 바인딩 설정과 같은 테이블 설정에 주의하십시오. )

### 고급설정 사용방법&#x20;

<figure><img src="../../../.gitbook/assets/image (1585).png" alt=""><figcaption></figcaption></figure>

이 섹션에서 설명하는 구성은 선택사항입니다.&#x20;

1. 데이터 테이블에 아래 필드를 추가합니다.&#x20;

<table><thead><tr><th width="93"></th><th width="153">필드명 </th><th width="310">설명 </th><th>codeName</th></tr></thead><tbody><tr><td>1</td><td>CodeName</td><td>작업 코드, E.g. A1234.</td><td>string</td></tr><tr><td>2</td><td>Description</td><td>작업 설명 </td><td>string</td></tr><tr><td>3</td><td>Progress</td><td>작업 완료 진행률, 예. 100%</td><td>int</td></tr><tr><td>4</td><td>Assigs</td><td>작업에서 사용한 리소스의 최종 결과 텍스트</td><td>string</td></tr><tr><td>5</td><td>IsMilestone</td><td>작업 이정표 </td><td>boolean</td></tr><tr><td>6</td><td>Actual Start</td><td>(계획된) 시작 시간을 보완하는 작업의 실제 시작 시간</td><td>OADATA</td></tr><tr><td>7</td><td>Actual End</td><td>(계획된) 종료 시간에 대한 보충으로 작업의 실제 시작 시간</td><td>OADATA</td></tr><tr><td>8 </td><td>Assigns</td><td>담당자 </td><td>string </td></tr></tbody></table>

<figure><img src="../../../.gitbook/assets/image (403).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
* ActualStart : Null인 경우 그래프에 실제 정보가 그려지지 않습니다.&#x20;
* 페이지에 실제 기간, 실제 시작 시간,  실제 종료 시간의 세 열이 표시됩니다. 그러나 데이터베이스에는 실제 시작 시간과 실제 종료 시간이라는 두 개의 열만 저장됩니다. 'actualStart'와 'actualEnd' 두 열이 함께 전달되어야만 관련 정보가 페이지에 표시됩니다.
* 페이지에서 실제 시작 시간과 실제 종료 시간을 기준으로 데이터를 로드한 후 실제 지속 시간이 자동으로 계산됩니다. 이 세 값은 비어 있을 수 있습니다. 그 중 하나가 비어 있으면 그림의 오른쪽 부분에 작업의 실제 범례가 그려지지 않습니다. 그러나 세 값 중 두 값에 대한 데이터가 있는 경우 다른 두 값을 클릭하면 이 값이 다시 계산되고 작업의 실제 범례도 다시 그려집니다. 그리고 실제 시작 시간과 실제 종료 시간이 존재하는 한 실제 공사 기간이 계산되어 저장 및 다시 로드 후 실제 범례가 그려집니다.
*   실제 시작 시간, 실제 지속 시간 및 실제 종료 시간과 같은 실제 관련 정보는 설정을 위한 단 하나의 제한 조건이 있습니다. 즉, 실제 종료 시간은 실제 시작 시간보다 빠를 수 없습니다.

    .
{% endhint %}

2\. 추가 구성 제공&#x20;

<table><thead><tr><th width="79"></th><th>필드명 </th><th>설명 </th><th>필드타입</th></tr></thead><tbody><tr><td>1</td><td>Collapsed</td><td>하위 작업 축소 여부</td><td>boolean</td></tr><tr><td>2</td><td>Status</td><td>작업 상태</td><td>string</td></tr></tbody></table>

2-1. Collapsed 필드&#x20;

이 필드가 전달되면 이 필드의 접기 정보를 사용하여 각 작업의 하위 작업이 접혀 있는지 여부를 미세하게 제어합니다.

이 필드가 전달되지 않으면 고정 확장 수준의 번호가 컨트롤로 사용되며 이전 수준의 하위 작업이 0부터 균일하게 확장됩니다(-1은 축소 없음을 의미).

2-2. Status 필드&#x20;

다음 그림의 기본 데이터 식별 상태는 다른 식별을 구성할 수 있습니다.



| Status                                                                                                 | 의미          | 필드타입   |
| ------------------------------------------------------------------------------------------------------ | ----------- | ------ |
| ![](https://gcdn.grapecity.com.cn/data/attachment/forum/202011/28/233635tkg3zkk3klw7sfb3.png)Active    | 작업 활동 중     | string |
| ![](https://gcdn.grapecity.com.cn/data/attachment/forum/202011/28/233708aqaarcn45eeprspz.png)Completed | 작업 완료       | string |
| ![](https://gcdn.grapecity.com.cn/data/attachment/forum/202011/28/233832ciraxed55vu7auaa.png)Failed    | 작업 실패       | string |
| ![](https://gcdn.grapecity.com.cn/data/attachment/forum/202011/28/233810d5mlhwtt96px3dtw.png)Suspended | 작업이 일시 중단됨  | string |
| ![](https://gcdn.grapecity.com.cn/data/attachment/forum/202011/28/233540b4qq0d4dt4it09q6.png)Waiting   | 작업 대기 중     | string |

<figure><img src="../../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

3\. 다른 데이터 테이블 사용&#x20;

3.1 휴일 구성&#x20;

사용자는 휴일 테이블을 직접 관리하고 데이터 테이블과 해당 필드 이름을 선택합니다.



<table><thead><tr><th width="118.33333333333331">필드명 </th><th width="500">설명 </th><th>필드형식 </th></tr></thead><tbody><tr><td>Date</td><td>특정 날짜(고유)</td><td>OADATA</td></tr><tr><td>Is Holiday</td><td>날짜가 공휴일인지, 토요일과 일요일이 기본 공휴일인지 입력할 필요가 없습니다. 휴일 필드인지 여부: false인 경우 해당 날짜는 원래 토요일 또는 일요일이지만 작동 중임을 의미합니다. true인 경우 해당 날짜는 원래 근무일(월요일-금요일)이지만 꺼져 있음을 의미합니다.</td><td>Boolean</td></tr></tbody></table>

### 작업 명령 구성&#x20;

작업 명령을 설정하면 웹 페이지에 명령 열이 표시됩니다. 아이콘을 클릭하거나 행을 클릭하면 명령이 실행됩니다.

<figure><img src="../../../.gitbook/assets/image (658).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (1588).png" alt=""><figcaption></figcaption></figure>
