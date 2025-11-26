# 사용자 컨트롤 만들기

포건시에서는 재사용 가능한 UI 구성 요소 생성을 지원하여 복잡한 응용 프로그램의 유지 관리성을 향상시킵니다. 사용자 컨트롤을 생성하고, 수정하면  해당 사용자 컨트롤이 적용된 모든 곳에 바로 반영되어 자동으로 업데이트됩니다.&#x20;

사용자 컨트롤은 기본적으로 프로젝트 탐색기에 나타나지 않는 고급기능이다.&#x20;

프로젝트 탐색기의 ![](https://help.grapecity.com.cn/download/thumbnails/80947595/image2023-1-9_11-57-14.png?version=1\&modificationDate=1673923189000\&api=v2) 버튼을 클릭하여, 개체 선택 창에서 "사용자 컨트롤" 에 체크를 하면 프로젝트 탐색기에 사용자 컨트롤이 표시됩니다.&#x20;

<figure><img src="../../.gitbook/assets/image (1808).png" alt=""><figcaption></figcaption></figure>

## 사용자 컨트롤 생성&#x20;

다음은 간단한 검색창 사용자 컨트롤 생성을 예로 들어 사용방법을 설명하겠습니다.&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1673923189000\&api=v2)  프로젝트탐색기에서 사용자컨트롤을 마우스 오른쪽 버튼으로 클릭하고 "사용자 정의 컨트롤만들기"를 선택하면 사용자  컨트롤 페이지가 자동으로 생성됩니다. 페이지는 기본적으로 3행 3열이며 행 높이와 열 너비는 모두 범위입니다.&#x20;

또는 "폴더 만들기"를 선택하여 폴더에 구성 요소를 만듭니다.

<figure><img src="../../.gitbook/assets/image (413).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1673923189000\&api=v2)  사용자 정의  컨트롤  만들기   페이지를  편집합니다. 사용자 정의  컨트롤  만들기   페이지에서의 작업은 일반 페이지에서의 작업과 유사하며 일반 페이지와 마찬가지로 사용자 정의  컨트롤  만들기   페이지를 디자인할 수 있습니다.

예를 들어 사용자 정의  컨트롤  만들기   페이지는 다음과 같습니다.

<figure><img src="../../.gitbook/assets/image (854).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923189000\&api=v2)  (선택 사항) 속성 및 이벤트를 설정합니다.&#x20;

<figure><img src="../../.gitbook/assets/image (497).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923189000\&api=v2)  (선택 사항) 바인딩 속성입니다. 셀과 구성 요소 속성 값 또는 구성 요소 컨테이너 셀 값 간의 양방향 바인딩 설정, 즉 셀 값이 변경되면 구성 요소 속성 값 또는 구성 요소 컨테이너 셀 값 구성 요소 속성 또는 구성 요소 컨테이너의 값이 동기적으로 변경되면 셀 값이 변경되면 셀 값도 동기적으로 변경됩니다.

컴포넌트에서 셀을 선택하고 셀 설정의 "속성 바인딩"에서 바인딩할 속성을 선택합니다. 속성은 기본적으로 바인딩되지 않으며 셀 값 또는 생성된 구성 요소 속성을 바인딩하도록 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1577).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923189000\&api=v2)  (선택 사항) 사용자  컨트롤  명령을 설정합니다. 사용자  컨트롤  명령에는 구성 요소 속성 설정 및 구성 요소 명령 트리거가 포함됩니다. 자세한 내용은 사용자 정의명령 을 참조하십시오 .

트리거 구성 요소 명령은 구성 요소 이벤트에 설정된 명령이 적용되도록 구성 요소에서 설정해야 합니다.

구성 요소를 선택하고 해당 명령을 "사용자 정의 컨트롤 명령 호출"으로 편집하고 생성된 구성 요소 이벤트를 명령 이름으로 선택합니다.

<figure><img src="../../.gitbook/assets/image (1223).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1673923189000\&api=v2)  일반 페이지에서 셀 영역을 선택하고 컴포넌트를 셀 영역으로 드래그하면 자동으로 컴포넌트 컨테이너가 생성됩니다.

<figure><img src="../../.gitbook/assets/image (1804).png" alt=""><figcaption></figcaption></figure>

또는 셀 영역을 선택한 후 해당 셀 유형을 사용자 정의 컨트롤로설정한 후 오른쪽 셀 설정에서 컴사용자 정의 컨트롤  이름을 선택합니다.

<figure><img src="../../.gitbook/assets/image (1926).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A47.png?version=1\&modificationDate=1673923189000\&api=v2)  이벤트 명령을 편집합니다. 사용자 정의 컨트롤을선택하고 셀 설정에서 "쿼리 만들기"명령을 클릭한 다음 명령 창에서 명령을 편집합니다.

<figure><img src="../../.gitbook/assets/image (1222).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80947595/%E6%AD%A5%E9%AA%A48.png?version=1\&modificationDate=1673923189000\&api=v2)  페이지를 실행합니다. 사용자 정의 컨트롤의 텍스트 상자에   end\_mon을 입력한 후 검색 버튼을 클릭하여 주문을 검색합니다.

<figure><img src="../../.gitbook/assets/image (907).png" alt=""><figcaption></figcaption></figure>
