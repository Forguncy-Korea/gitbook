# CSV 내보내기

서버단 명령을 이용하여 서버단에서 CSV 데이터를 내보낼 수 있습니다.&#x20;

다음은 서버 명령의  CSV가져오기/내보내 명령을 사용하여 서비단에서 CSV 데이터를 내보내는 방법에 대한 자세한 설명입니다.

​![](https://help.grapecity.com.cn/download/thumbnails/72357732/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092609000\&api=v2)개체 관리자의 서버단 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버단 명령 만들기를 선택하여 서버 명령 만들기 대화 상자를 나타납니다.또는 폴더 만들기를 선택하여 폴더에 서버 명령을 만듭니다.<br>

![](https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FVfAUDVhQBe0mgQr6F56l%2Fuploads%2Ft4FZ9qEVzybIdckBENz4%2Fimage.png?alt=media\&token=1d2bf4bb-c1ef-4616-84fc-6ae66ff2399f)

리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357846/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092611000\&api=v2)  서버 명령 관리자에서 \[새로 만들기]를 클릭하고 서버단 명령 편집 대화 상자를 표시하여 서버  명령에 대한 일반 설정을 편집합니다. 서버단 명령의 이름을 CSV 내보내기로 설정합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357846/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092611000\&api=v2)  서버단 명령을 편집하는 명령입니다. \[편집 명령] 하이퍼링크를 클릭하고 서버 명령 편집 대화 상자를 표시하고 서버 가져오기 내보내기 CSV 명령을 선택합니다. 명령 설정은 아래 표에 나와 있습니다.

<table><thead><tr><th width="268">설정</th><th>설명</th></tr></thead><tbody><tr><td>CSV 처리유형 </td><td>CSV 가져오기 작업을 선택하고 헤더 행을 가져올지 여부를 설정할 수 있습니다.</td></tr><tr><td>CSV파일 경로 </td><td>CSV 파일을 내보낼 경로를 설정합니다. "D:\CSV 가져오기\주문 목록 .csv"와 같은 파일의 전체 경로를 입력해야 하며 폴더는 이미 있는 폴더여야 하며 접미사 이름 ".csv"은 생략할 수 있습니다.</td></tr><tr><td>대상 테이블 </td><td>CSV를 가져올 테이블을 선택합니다.</td></tr><tr><td>열 연결 선택 </td><td>가져올 테이블을 선택하면 모든 테이블의 열이 자동으로 나열되고 필요에 따라 열을 추가하거나 삭제할 수도 있습니다.</td></tr><tr><td>쿼리조건 </td><td>내보낼 데이터의 조건인 쿼리 조건을 설정합니다. 필드가 "ID"로 설정된 경우 작업이 보다 크면 값이 3이고 ID가 3보다 큰 데이터를 CSV 파일로 내보냅니다.</td></tr><tr><td>상위제한 </td><td>표시/건너뛸 데이터 행 수를 설정합니다.</td></tr><tr><td>정렬 </td><td>데이터 정렬 규칙을 설정합니다.</td></tr><tr><td>기타설정 </td><td><p></p><p>CSV 가져오기 작업을 수행하는 경우 파일의 인코딩, 줄 구분 기호, 열 구분 기호, 텍스트 한정자, 파일 확장명, 가져온 CSV 파일의 인코딩, 행 구분 기호, 텍스트 구분 기호 및 파일 확장명을 가져오기 위해 여기에 설정된 것과 일치하도록 설정할 수 있습니다.</p><ul><li>인코딩: 가져올 파일의 인코딩을 설정합니다. UTF-8, GB2312, ASCII, 유니코드, Shift-JIS를 지원한다. 다른 웹 브라우저에서 지원하는 인코딩을 입력할 수도 있습니다.</li><li>행 구분 기호: "\r\n", "\r", "\n"을 지원합니다. 다른 문자를 줄 구분 기호로 설정할 수도 있습니다. 기본값은 \r\n입니다.</li><li>열 구분 기호: ""\t", "|", ”。 다른 문자를 설정할 수도 있습니다. 잘못된 문자를 열 구분 기호로 설정하면 열 구분 기호로 자동으로 사용됩니다. 기본값은 ""입니다.</li><li>텍스트 한정자: 시스템에서 문자열의 시작과 끝을 인식할 수 있는 텍스트 한정자를 지정합니다. 기본값은 ""입니다.</li><li>파일 확장자: 가져온 파일의 확장자입니다. 기본값은 .csv입니다.</li><li>날짜 데이터 자동 변환: 이 옵션을 선택하면 값이 날짜 데이터로 자동으로 변환됩니다. 이 옵션을 선</li></ul></td></tr></tbody></table>

![](<../../../../.gitbook/assets/image (1035).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357846/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092611000\&api=v2)  설정완료되면 서버 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼을 설정합니다. 버튼의 명령을 편집하고 "서버단 명령 호출"으로 명령을 선택한 다음 서버단 명령 뒤에 있는 드롭다운을 클릭하고 드롭다운 목록에서 "CSV 내보내기"를 선택합니다.

![](<../../../../.gitbook/assets/image (441).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357846/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092611000\&api=v2) 설정이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다. 페이지를 실행합니다.페이지에서 CSV 내보내기 버튼을 클릭하면 설정된 지정된 경로 아래에 내보낸 CSV 파일이 표시됩니다.
