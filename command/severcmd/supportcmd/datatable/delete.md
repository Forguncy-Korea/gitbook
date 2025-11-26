# 데이블 테이블 데이터 삭제하기

서버단 명령의 데이터 테이블 작업 명령에서 삭제에 대한 작업 유형을 설정하고 대상 테이블에서 지정된 레코드를 삭제할 수 있습니다.

다음은 서버단 명령의 데이터 테이블 작업 명령에서 삭제 시 작업 유형을 선택하는 작업에 대해 설명합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357696/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092609000\&api=v2)  개체 관리자의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버단 명령 만들기를 선택하여 서버단 명령 만들기 대화 상자를 나타납니다.

또는 폴더 만들기를 선택하여 폴더에 서버단 명령을 만듭니다.

![](<../../../../.gitbook/assets/image (1575).png>)

리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357696/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092609000\&api=v2)  서버 명령의 일반 설정을 편집합니다. 서버단 명령의 이름을 "데이터 삭제"로 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357696/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092609000\&api=v2)  서버단 명령을 편집하는 명령입니다. \[명령편집] 하이퍼링크를 클릭하고 서버 명령 편집 대화 상자를 표시하고 데이터 테이블 편집하는 명령을 선택합니다.

* 작업 유형: 작업 유형을 삭제로 선택합니다.
* 대상 테이블: \[고객주문테이블]과 같이 데이터를 삭제할 데이터 테이블을 선택합니다.
* 업데이트 조건: 필드 "ID", "같음", 값 "3", 즉 ID가 3인 데이터 삭제와 같이 삭제된 레코드에 대한 조건을 설정합니다.

![](<../../../../.gitbook/assets/image (1556).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357696/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092609000\&api=v2)  설정이 완료되면 이 서버단 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼으로 설정합니다. 버튼의 명령을 편집하고 "서버단 명령 호출"으로 명령을 선택한 다음 서버단 명령 뒤에 있는 드롭다운을 클릭하고 드롭다운 목록에서 "데이터 삭제"를 선택합니다.

![](<../../../../.gitbook/assets/image (1865).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357696/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092609000\&api=v2)  서버단 명령을 선택한 후 고급 설정 표시를 클릭하고 호출이 성공한 후 데이터 다시 로드를 선택하여 서버가 데이터 테이블 업데이트 명령을 호출하면 페이지가 데이터를 다시 로드하고 업데이트된 데이터를 표시합니다.

![](<../../../../.gitbook/assets/image (442).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357696/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1648092609000\&api=v2)  설정이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다. 페이지를 실행합니다.페이지에서 데이터 삭제 단추를 클릭하면 데이터 테이블의 데이터가 서버 측에서 삭제됩니다.

ID 3의 레코드가 삭제된 것을 볼 수 있습니다.

