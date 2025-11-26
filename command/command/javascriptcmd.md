# 프로그래밍 명령 - JavaScript 명령

포건시는 표준 HTML5 프로그램을 생성하며, 개발 플랫폼으로서 JavaScript 프로그래밍 인터페이스를 제공합니다. 특별한 비즈니스 요구 사항이 있는 경우 제공된 프로그래밍 인터페이스를 사용하여 구현할 수 있습니다. JavaScript API는 JavaScript API 인덱스를 참조하십시오.

JavaScript 명령을 사용하여 설정된 JavaScript 코드를 실행할 수 있습니다.

![](<../../.gitbook/assets/image (1853).png>)

## JavaScript 명령&#x20;

JavaScript 명령의 오른쪽에는 포건시 Page 클래스와 CommandHelper 아래의 모든 JavaScript API가 나열됩니다. API 위로 마우스를 가져가면 API의 세부 정보와 사용 방법이 표시됩니다. API를 두 번 클릭하면 JavaScript 명령 텍스트 상자에 API가 삽입됩니다.

JavaScript 명령 설정에 대한 설명은 표에 나와 있습니다.

| 설정       | 설명                                                                                                                                                                      |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 열기       | Visual Studio와 같은 설정된 응용 프로그램을 사용하여 JavaScript 코드에 해당하는 JavaScript 파일을 열고 응용 프로그램이 설정되지 않은 경우 기본 프로그램을 사용하여 엽니다. 이 응용 프로그램에서 JavaScript 코드를 편집할 수 있으며 포건시가 자동으로 동기화됩니다. |
| 연결 프로그램  | JavaScript 코드를 여는 응용 프로그램을 설정합니다.                                                                                                                                       |

예를 들어 주문 목록 페이지의 쿼리 단추에 JavaScript 명령을 추가하고 JavaScript 코드를 다음과 같이 편집합니다.

```
var countcellValue=Forguncy.Page.getCell("count").getValue();
alert(countcellValue);
```

![](<../../.gitbook/assets/image (2100).png>)

실행 후 쿼리 버튼 클릭하면 대화 상자가 나타납니다.&#x20;

![](<../../.gitbook/assets/image (1192).png>)
