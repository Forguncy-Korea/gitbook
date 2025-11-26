# Cell 클래스

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364904/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 설명 <a href="#cell-lei-miao-shu" id="cell-lei-miao-shu"></a>

셀 개체입니다.

#### ![](https://help.grapecity.com.cn/download/thumbnails/72364904/blue%20block.png?version=1\&modificationDate=1648092722000\&api=v2) 메서드 <a href="#cell-lei-fang-fa" id="cell-lei-fang-fa"></a>



| 메서드                                       | 설명                                                                                                                                                       |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [bind](bind.md)                           | 선택한 셀에 하나 이상의 이벤트 처리기를 추가하고 이벤트가 발생할 때 실행되는 함수를 지정합니다.                                                                                                   |
| [disable](disable.md)                     | 셀을 사용하지 않도록 설정합니다. 셀이 비활성화되면 클릭할 수 없습니다.                                                                                                                 |
| [enable](enable.md)                       | 셀을 활성화합니다. 셀을 사용하지 않도록 설정하면 클릭할 수 없습니다.                                                                                                                  |
| [getActiveTabIndex](getactivetabindex.md) | <p>0부터 시작하는 현재 탭의 번호를 가져옵니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.<br></p>                                                                                         |
| [getContentPage](getcontentpage.md)       | <p>페이지 컨테이너의 자식 페이지 개체를 가져옵니다. 이 메서드는 셀 유형이 페이지 컨테이너인 경우에만 사용할 수 있습니다.<br></p>                                                                           |
| [getTabCount](gettabcount.md)             | <p>탭 수를 가져옵니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.<br></p>                                                                                                       |
| [getTabPage](gettabpage.md)               | <p>탭 컨테이너에서 자식 페이지 개체를 가져옵니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.<br></p>                                                                                        |
| [getValue](getvalue.md)                   | 지정된 셀의 값을 가져옵니다. 셀의 값을 가져온 후 명령과 같은 다른 곳에서 사용할 수 있습니다.                                                                                                   |
| [hasFocus](hasfocus.md)                   | <p>지정된 셀에 포커스가 있는지 여부를 가져옵니다. 페이지의 셀 중 하나가 포커스를 가져오는지 여부를 감지하는 데 사용할 수 있습니다. 반환 값은 true 또는 false, true: 셀은 포커스를 가져옵니다. false: 셀이 포커스를 가져오지 않습니다.<br></p> |
| [hide](hide.md)                           | 셀을 숨깁니다. 페이지에 지정된 셀을 숨기면 셀의 배경이 아닌 셀의 값, 유형 등만 숨길 수 있습니다. 쇼 방법과는 달리 실제 요구 사항에 따라 사용할 수 있습니다.                                                             |
| [setBackColor](setbackcolor.md)           | 지정된 셀에 배경색을 설정합니다.                                                                                                                                       |
| [setFocus](setfocus.md)                   | <p>지정된 셀에 포커스를 설정합니다. 일반적으로 셀은 마우스 클릭으로 요소를 선택하거나 탭 키를 통해 셀에 배치될 때 포커스를 받습니다. setFocus 메서드를 사용하면 지정된 셀에 직접 포커스를 부여할 수 있습니다.<br></p>                      |
| [setForeColor](setforecolor.md)           | 지정된 셀에 글꼴 색상을 설정합니다. setBackColor 메서드와 유사합니다.                                                                                                            |
| [setReadOnly](setreadonly.md)             | 셀의 읽기 전용 상태를 설정합니다.                                                                                                                                      |
| [setValue](setvalue.md)                   | 지정된 셀에 대한 값을 설정합니다.                                                                                                                                      |
| [showTab](showtab.md)                     | <p>표시되는 탭을 설정합니다. 예를 들어 첫 번째 탭이 기본적으로 표시되고 이 메서드를 사용하여 두 번째 탭을 표시할 수 있습니다. 이 메서드는 셀 유형이 탭인 경우에만 사용됩니다.<br></p>                                           |
| [show](show.md)                           | 셀을 표시합니다. 페이지의 숨겨진 셀을 표시하여 셀의 값, 유형 등을 표시합니다. hide 방법과는 달리 실제 요구 사항에 따라 사용할 수 있습니다.                                                                      |
| [unbind](unbind.md)                       | 선택한 요소에 대한 이벤트 처리기를 제거합니다. 이 메서드는 선택한 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.                                                                  |
| [unbindAll](unbindall.md)                 | 페이지의 모든 이벤트에 대한 바인딩을 제거합니다. 이 메서드는 페이지의 모든 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 실행을 종료할 수 있습니다.                                                             |
