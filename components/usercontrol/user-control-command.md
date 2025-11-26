# 사용자정의컨트롤 명령

사용자정의컨트롤은 생성 명령을 지원합니다. 구성 요소 명령은 구성 요소의 공개 명령이며 구성 요소 내에서 또는 다른 페이지의 명령에서 호출할 수 있습니다.



### 구성요소 생성 명령 <a href="#chuang-jian-zu-jian-ming-ling" id="chuang-jian-zu-jian-ming-ling"></a>

사용자컨트롤 선택하고 마우스 오른쪽 버튼을 클릭한 후 오른쪽 클릭 메뉴에서 "명령 생성"을 선택하면 명령 생성을 위한 대화상자가 나타납니다.

<figure><img src="../../.gitbook/assets/image (257).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (261).png" alt=""><figcaption></figcaption></figure>

| 설정   | 설명                        |
| ---- | ------------------------- |
| 일반   | 구성요소 명령의 이름과 설명을 설정합니다.   |
| 매개변수 | 구성요소 명령의 매개변수를 설정합니다.     |
| 반환 값 | 구성 요소 명령의 반환 값을 설정합니다.    |
| 주문하다 | 구성요소 명령에서 실행되는 명령을 설정합니다. |

예를 들어 구성요소 명령을 "열 옵션 명령"으로 설정하는 경우 편집 명령은 다음과 같습니다.

<figure><img src="../../.gitbook/assets/image (262).png" alt=""><figcaption></figcaption></figure>

### 사용자 컨트롤 내에서 사용자컨트롤 명령 사용&#x20;

사용자 컨트롤내부에서 사용하는 경우 "컴포넌트 호출 명령"을 사용해야 합니다. 명령을 선택한 후 컴포넌트 명령에 매개변수와 반환 값이 있으면 명령 아래에 표시됩니다.

<figure><img src="../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

페이지에서 컴포넌트 컨테이너 셀을 설정합니다. 페이지를 실행한 후 "열 옵션" 버튼을 클릭하면 컴포넌트 명령이 호출되고 열 옵션 대화 상자가 나타나며 사용 가능한 열을 선택할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (264).png" alt=""><figcaption></figcaption></figure>

### 구성 요소 외부에서 구성 요소 명령 사용 <a href="#zai-zu-jian-wai-bu-shi-yong-zu-jian-ming-ling" id="zai-zu-jian-wai-bu-shi-yong-zu-jian-ming-ling"></a>

컴포넌트 외부에서 사용하는 경우에는 오퍼레이션 셀 명령을 사용하여 컴포넌트 셀을 선택하고 해당 오퍼레이션에 대해 "구성요소 명령 호출"을 선택한 후 컴포넌트 명령에 매개변수와 반환 값이 있는 경우 표시됩니다.&#x20;

<figure><img src="../../.gitbook/assets/image (265).png" alt=""><figcaption></figcaption></figure>
