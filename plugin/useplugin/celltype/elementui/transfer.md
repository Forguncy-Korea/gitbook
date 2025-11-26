# 전송

{% file src="../../../../.gitbook/assets/ElementUI_전송.fgko" %}

여러 선택 항목의 또 다른 UI입니다.

<figure><img src="../../../../.gitbook/assets/image (992).png" alt=""><figcaption></figcaption></figure>

특히 vue에 대한 기본 지식이 있는 개발자는 이 셀 유형에서 제공하는 몇 가지 인터페이스를 사용하여 자신만의 아이템 UI를 정의할 수 있습니다.

### 인터페이스

1. customRender(h, 옵션):
   1. 이 메소드는 커스텀 UI를 정의하는 곳입니다.
   2. 사용자는 자신의 UI를 사용자 지정하기 위해 "run javascript" 명령을 실행하여 이 메서드의 정의를 변경할 수 있습니다.
   3. 이 방법에서는 두 개의 매개변수가 허용됩니다.
      1. 매개변수 "h"는 vue 프레임워크의 렌더링 방법을 의미하며 가상 돔을 반환합니다.
      2. 매개변수 "옵션"은 전송에 의해 제공되며 전송 데이터 소스의 모든 단일 항목을 의미합니다.
   4. 이 메서드는 가상 돔을 반환해야 합니다.
2. 새로고침UI:
   1. 이 메서드는 사용자가 customRender를 변경한 후 필요한 전송 구성 요소를 다시 빌드하는 데 사용됩니다. vue는 렌더링이 변경되었음을 모르기 때문에 UI를 수동으로 새로 고쳐야 합니다.
3. getValueFromElement:
   1. 셀 유형 값 얻기

### 단계

* 페이지 로드 명령 편집
  1. "자바 스크립트 명령 실행"을 선택하십시오.
  2. 자바스크립트 수정
     1. 셀 유형을 전송할 셀 이름을 만드십시오.
     2. 해당 이름으로 전송 셀 유형 가져오기
     3. customRender 정의
     4. 전송의 customRender를 방금 정의한 것으로 바꿉니다.
     5. 새로 고침 UI
* 해킹 요소 스타일
  1. 셀 유형을 전송할 클래스 이름을 만드십시오.
  2. 클래스 스타일 편집 및 css 파일 업로드
* 제출할 맞춤 값을 얻는 방법
  1. getValueFromElement로 셀 유형 값 가져오기
  2. cellType.vue.data를 사용하여 전송 데이터 소스 가져오기
  3. 데이터 소스 및 셀 유형 값으로 자신의 값을 사용자 정의하십시오.



### 셀속성&#x20;

<figure><img src="../../../../.gitbook/assets/image (2205).png" alt=""><figcaption></figcaption></figure>

| 이름         | 설명                                                                                                                                                                                                                                             |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 명령 편집      | 값이 변경될 때 실행할 명령 구성                                                                                                                                                                                                                             |
| 기본값        | 기본값                                                                                                                                                                                                                                            |
| 바인딩 사용     | 항목이 데이터베이스에서 바인딩되는지 여부를 나타냅니다.                                                                                                                                                                                                                 |
| 항목 구성      | 디자인 타임에 바인딩 해제 항목 구성                                                                                                                                                                                                                           |
| 바인딩 항목 구성  | 구성 바인딩 항목. 구성 값/레이블 열, 필터, 정렬, 상단/오프셋 및 캐시 허용                                                                                                                                                                                                  |
| 왼쪽 제목      | <p><br><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196194/image2022-2-17_14-40-55.png?version=1&#x26;modificationDate=1645080055307&#x26;cacheVersion=1&#x26;api=v2&#x26;width=461&#x26;height=250" alt=""></p>     |
| 오른쪽 제목     | ![](https://grapecity.atlassian.net/wiki/download/thumbnails/2931196194/image2022-2-17_14-40-55.png?version=1\&modificationDate=1645080055307\&cacheVersion=1\&api=v2\&width=461\&height=250)                                                  |
| 대상 순서      | <ul><li>데이터 소스와 동일한 순서 유지</li><li>새 항목을 마지막에 삽입</li><li>새 항목을 처음에 삽입</li></ul>                                                                                                                                                                 |
| 필터링 가능     | <p><img src="https://grapecity.atlassian.net/wiki/download/thumbnails/2931196194/image2022-2-17_14-42-42.png?version=1&#x26;modificationDate=1645080162420&#x26;cacheVersion=1&#x26;api=v2&#x26;width=469&#x26;height=250" alt=""><br><br></p> |
| 필터 자리 표시자  | ![](https://grapecity.atlassian.net/wiki/download/thumbnails/2931196194/image2022-2-17_14-42-42.png?version=1\&modificationDate=1645080162420\&cacheVersion=1\&api=v2\&width=469\&height=250)                                                  |



### 관련 명령 빠른 생성&#x20;

| 이름          | 설명                                                                                                           |
| ----------- | ------------------------------------------------------------------------------------------------------------ |
| 연동 데이터 새로고침 | <p>바인딩 모드에서만 사용 가능<br> 바인딩이 변경되었지만 바인딩 항목이 데이터를 자동으로 다시 로드할 수 없는 경우 이 작업을 사용하면 바인딩 항목을 강제로 다시 로드할 수 있습니다</p> |
