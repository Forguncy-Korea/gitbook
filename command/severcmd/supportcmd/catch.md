# 예외처리 명령

서버단 명령에서 예외 catch 명령을 사용하여 지정된 상황에서 오류를 처리한 다음 오류 조건에 따라 다음 단계를 결정할 수 있습니다.

​![](https://help.grapecity.com.cn/download/thumbnails/72358198/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092616000\&api=v2)프로젝트 탐색기의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버단 명령 만들기를 선택하여 서버단 명령 만들기 대화 상자를 띄웁니다. <br>

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FzxNQdilex6YN3fZKZhGM%2Fuploads%2FM7ndQXFvMxRnTKlgee90%2Fimage.png?alt=media\&token=55d7054c-8e83-4df0-b9e6-4effaf72841e)

리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버단 명령 만들기 대화 상자를 팝업할 수도 있습니다.

서버단 명령을 편집하는 명령입니다. 명령 탭에서 \[명령편집] 하이퍼링크를 클릭하고 서버단 명령 실행 대화 상자를 표시하고 예외 처리 명령을 선택합니다.

![](<../../../.gitbook/assets/image (2050).png>)

예외 처리 명령을 선택하면 \[Try], \[Catch], \[Finally] 세 개의 하위 노드가 나타납니다. 각 노드는 명령 목록을 추가할 수 있습니다.

Catch 노드에서 Exception Code 및 Exception Message를 설정하고 다음 명령에서 파라미터로 사용할 수 있습니다.

<figure><img src="../../../.gitbook/assets/image (1477).png" alt=""><figcaption></figcaption></figure>

명령이 예외 없이 실행되면 오류 코드는 0이 됩니다. 오류 코드는 예외 또는 오류가 발생한 경우에만 0이 아닙니다.

* Try 노드 실행에 예외가 없는 경우 반환된 결과는 Try 노드에서 가져옵니다.
* Try 노드가 예외를 실행하는 경우 반환 결과는 Catch 노드에서 가져옵니다.
* Finally 노드는 명령만 실행하고 결과를 반환하지 않습니다.
