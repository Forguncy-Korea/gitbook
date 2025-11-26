# 트랜젝션 생성하기

데이터베이스 트랜잭션은 단일 데이터 테이블 작업 명령에서 수행되는 일련의 작업으로, 완전히 또는 전혀 수행되지 않습니다. 관련 작업 집합을 모두 성공하거나 모두 실패한 명령으로 결합하면 오류 복구를 단순화하고 응용 프로그램을 보다 안정적으로 만들 수 있습니다.

서버단 명령에서 트랜잭션 명령에 여러 데이터 테이블 작업 명령을 추가할 수 있으며, 어떤 이유로든 실행 중에 이러한 작업 중 하나가 실패하면 트랜잭션 명령이 중지되고 완료된 작업이 무효화됩니다.

서버 쪽에서 데이터 테이블 작업 명령을 실행하려면 데이터 정확성을 보장하기 위해 데이터 테이블 작업 명령을 트랜잭션 명령에 배치하는 것이 좋습니다.

다음은 서버 명령에서 트랜잭션 명령을 사용하는 방법에 대한 자세한 설명입니다.

​![](https://help.grapecity.com.cn/download/thumbnails/72357732/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092609000\&api=v2)개체 관리자의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버단 명령 만들기를 선택하여 서버 명령 만들기 대화 상자를 띄웁니다 .또는 폴더 만들기를 선택하여 폴더에 서버 명령을 만듭니다.​

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FVfAUDVhQBe0mgQr6F56l%2Fuploads%2Ft4FZ9qEVzybIdckBENz4%2Fimage.png?alt=media\&token=1d2bf4bb-c1ef-4616-84fc-6ae66ff2399f)

​리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357918/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092612000\&api=v2)  서버단 명령의 일반 설정을 편집합니다. 서버단 명령의 이름을 "트랜잭션"으로 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72358037/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092613000\&api=v2)  서버단 명령을 편집하는 명령입니다. \[명령편집] 하이퍼링크를 클릭하고 서버 명령 편집 대화 상자를 표시하고 트랜잭션 명령을 선택합니다.

고급 설정 표시를 클릭하여 격리 수준을 설정할 수 있습니다. 기본 수준을 사용하는 것이 좋습니다.

* 기본: 데이터베이스의 기본 격리 수준을 사용합니다.
* 커밋되지 않은 내용까지 읽기: 트랜잭션 중에 가변 데이터를 읽을 수는 없지만 수정할 수 있습니다(MySQL, SQLServer는 이 수준을 지원합니다).
* 커밋 내용 읽기: 트랜잭션 중에 가변 데이터를 읽고 수정할 수 있습니다(MySQL, Oracle, SQLServer에서 이 레벨을 지원).
* 반복 가능함으로 읽기: 트랜잭션 중에 가변 데이터를 읽을 수 있지만 수정할 수 없습니다. 트랜잭션 중에 새 데이터를 추가할 수 있습니다(MySQL, SQLServer는 이 수준을 지원합니다).
* 직렬화: 트랜잭션 중에 가변 데이터를 읽을 수 있지만 수정하거나 새 데이터를 추가할 수는 없습니다(SQLite, Oracle, MySQL, SQLServer는 이 레벨을 지원합니다).



![](<../../../.gitbook/assets/image (1019).png>)

그런 다음 트랜잭션 명령에 데이터 테이블 작업 명령을 추가해야 합니다.

![](<../../../.gitbook/assets/image (1128).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358037/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092613000\&api=v2)  서버단 명령이 생성되면이 서버단 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼을 설정합니다. 버튼의 명령을 편집하고 명령을 트랜잭션 명령으로 선택합니다.

![](<../../../.gitbook/assets/image (1374).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358037/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092613000\&api=v2)  설정이 완료되면 확인을 클릭하여 대화 상자를 닫고 페이지를 실행합니다，페이지에서 데이터 업데이트 버튼을 클릭하면 서버는 트랜잭션 명령의 데이터 테이블 작업 명령을 실행하여 데이터를 업데이트합니다.
