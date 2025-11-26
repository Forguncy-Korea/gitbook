# 조건명령

서버단 명령에서 조건부 명령을 사용하여 조건에 따라 다른 명령을 설정하고, If, ElseIf 및 Else를 사용하여 다른 조건 분기를 구성하고, 조건 집합을 설정하고, 조건이 충족되면 하나 또는 하나의 명령 집합을 실행할 수 있습니다. 그렇지 않은 경우 다른 명령 또는 명령 집합이 실행됩니다.

​![](https://help.grapecity.com.cn/download/thumbnails/72357732/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092609000\&api=v2)개체 관리자의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버단 명령 만들기를 선택하여 서버 명령 만들기 대화 상자를 나타납니다.또는 폴더 만들기를 선택하여 폴더에 서버 명령을 만듭니다.​

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FVfAUDVhQBe0mgQr6F56l%2Fuploads%2Ft4FZ9qEVzybIdckBENz4%2Fimage.png?alt=media\&token=1d2bf4bb-c1ef-4616-84fc-6ae66ff2399f)

​리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357918/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092612000\&api=v2)  서버 명령의 일반 설정을 편집합니다. 서버 쪽 명령의 이름을 "주문상태 업데이터"로 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357918/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092612000\&api=v2)  서버 쪽 명령을 편집하는 명령입니다. \[편집 명령] 하이퍼링크를 클릭하여 서버 명령 편집 대화 상자를 표시하고 조건부 명령을 선택합니다.

1\. 조건을 설정합니다. \[If 조건식]을 클릭하고 오른쪽에 조건 표현식을 설정하고 \[새 조건]을 클릭하고 필드를 \[%CurrentUser.Role%]로 설정하고 \[같음]으로 설정하고 \[관리자]를 입력합니다.

![](<../../../.gitbook/assets/image (379).png>)

2\. 명령을 설정합니다. \[If 조건식]에서 \[명령없음]을 클릭하고 오른쪽의 \[선택 명령] 콤보 상자에서 \[데이터 테이블 작업]을 선택합니다. 유형은 \[업데이트]입니다.

설정이 완료되면 확인을 클릭합니다.

![](<../../../.gitbook/assets/image (1347).png>)



3\. 조건부 분기를 추가합니다. \[Else 추가]를 선택합니다.

![](<../../../.gitbook/assets/image (908).png>)

4\. "Else"에서 "조건"을 클릭하고 오른쪽의 "선택 명령"콤보 상자에서 명령 "반환 명령 생성하기"를 선택하고 반환 코드 및 반환 정보를 설정합니다.

설정이 완료되면 확인을 클릭하여 창을 닫습니다.

![](<../../../.gitbook/assets/image (884).png>)



![](https://help.grapecity.com.cn/download/thumbnails/72357918/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092612000\&api=v2)  서버 명령이 생성되면이 서버 쪽 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼으로 설정합니다. 버튼의 명령을 편집하고 "서버단 명령 호출"으로 명령을 선택한 다음 서버단 명령 후 드롭다운을 클릭하고 드롭다운 목록에서 "주문 상태 업데이트"를 선택합니다.

반환 코드를 설정하고 페이지에 지정된 셀에 정보를 반환하고 "연결 데이터를 최신 정보로 업데이트하기"를 선택합니다.

![](<../../../.gitbook/assets/image (1645).png>)



![](https://help.grapecity.com.cn/download/thumbnails/72357918/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092612000\&api=v2) 설정이 완료되면 확인을 클릭하여 대화 상자를 닫고 페이지를 실행합니다.

* 유재석으로 로그인을 사용하여, 유재석의 역할은 관리자입니다.페이지에서 주문 상태 업데이트 버튼을 클릭하면 서비스 쪽에서 데이터 테이블 작업 명령을 실행하여 주문 상태를 업데이트하고 ID가 1인 주문상태는 업데이트됩니다.&#x20;
* Administrator로 로그인을 사용하여, Administrator은 관리자 역할의 사용자가 아니다, 주문 상태 업데이트 버튼을 클릭, 서버는 주문 상태를 업데이트하기 위해 데이터 테이블 작업 명령을 수행하지 않습니다,하지만 반환 명령을 실행, 페이지에 반환 코드 및 반환 정보를 표시합니다.

![](<../../../.gitbook/assets/image (2098).png>)

*
