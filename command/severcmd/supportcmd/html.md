# 페이지를 HTML로 내보내기

서버단 명령에서 페이지를 HTML로 내보내기 명령을 사용하여 페이지를 HTML 문자열로 변환하고 결과를 변수에 저장할 수 있습니다. 그런 다음 결과 변수를 메일 보내기 명령의 내용으로 사용하여 페이지 콘텐츠를 메시지 내용으로 보낼 수 있습니다.

## 페이지를 HTML로 내보내기&#x20;

다음은 서버 명령에서  "페이지를 HTML로 내보내기 명령"을 설정하는 방법을 자세히 설명합니다.

**절차를 따르십시오**

​![](https://help.grapecity.com.cn/download/thumbnails/72358198/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092616000\&api=v2)프로젝트 탐색기의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버단 명령 만들기를 선택하여 서버단 명령 만들기 대화 상자를 띄웁니다. <br>

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FzxNQdilex6YN3fZKZhGM%2Fuploads%2FM7ndQXFvMxRnTKlgee90%2Fimage.png?alt=media\&token=55d7054c-8e83-4df0-b9e6-4effaf72841e)

리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72358353/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092617000\&api=v2)  서버 명령의 일반 설정을 편집합니다. 설정 명령의 이름은 \[페이지를 HTML로 내보내기]입니다.

![](https://help.grapecity.com.cn/download/thumbnails/72358353/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092617000\&api=v2)  서버 쪽 명령을 편집하는 명령입니다. \[명령 편집] 하이퍼링크를 클릭하고 서버 명령 편집 대화 상자를 표시하고 페이지를 HTML 명령으로 내보내기를 선택합니다.

* 페이지 내보내기: 앱에서 페이지를 선택하여 HTML로 내보냅니다.
* 결과를 저장할 파라미터 이름 : 다음 명령에서 사용할 수 있는 변수에 결과를 저장합니다.&#x20;

![](<../../../.gitbook/assets/image (454).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358353/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092617000\&api=v2) 페이지를 HTML 명령으로 내보낸 후 "메일 내용 편집"을 선택하고 페이지를 HTML 명령으로 내보내는 변수 "고객주문"페이지를 선택하는 메일 보내기 명령을 추가합니다. 추가 설정은 [알림 명령 -메일 보내기 명령](../../command/sendmailcmd.md)을 참조 하세요.

![](<../../../.gitbook/assets/image (1546).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358353/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092617000\&api=v2)  설정완료되면 이 서버단 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼을 설정합니다. 버튼 명령을 편집하고 "서버단 명령 호출"으로 명령을 선택한 다음 서버 쪽 명령 뒤에 있는 드롭다운 버튼을 클릭하고 드롭다운 목록에서 "Html로 페이지 보내기"를 선택합니다.

![](<../../../.gitbook/assets/image (1621).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358353/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092617000\&api=v2) 설정이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다. 페이지를 실행합니다.페이지에서 페이지를 메일전송 버튼을 클릭하면 지정된 페이지가 HTML 문자열로 변환되고 페이지 내용이 지정된 전자 메일 주소로 메시지 내용으로 전송됩니다.

![](<../../../.gitbook/assets/image (1812).png>)
