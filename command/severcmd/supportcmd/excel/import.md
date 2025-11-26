# 서버에서 Excel 파일 가져오기

서버 명령에서 서버 가져오기 및 Excel 내보내기 명령을 사용하여 서버에서 Excel 데이터를 가져올 수 있습니다.

다음은 서버단 명령에서 서버에서  Excel파일을사가져오는방법에 대한 자세한 소개입니다.



![](https://help.grapecity.com.cn/download/thumbnails/80959472/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1675999591000\&api=v2)  프로젝트탐색기에서   서버 커맨드의 레이블을 마우스 오른쪽 버튼으로 클릭하고 "서버단 명령생성하기"을 선택하면 서버 커맨드 생성 대화상자가 팝업된다.

또는 "폴더 만들기"를 선택하여 폴더에 서버 명령을 만듭니다.

<figure><img src="../../../../.gitbook/assets/image (1084).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959472/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1675999591000\&api=v2)  서버 명령에 대한 일반 설정을 편집합니다. 서버 명령의 이름을 "Excel 가져오기"로 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959472/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1675999591000\&api=v2)  서버 명령을 편집하는 명령입니다. "명령 편집" 하이퍼링크를 클릭하여 서버 명령 편집 대화 상자를 팝업하고 서버 가져오기 및 내보내기 Excel 명령을 선택합니다. 명령의 설정 및 설명은 아래 표를 참조하십시오.

<table><thead><tr><th width="298">설정 </th><th>설명 </th></tr></thead><tbody><tr><td>Excel 작업 </td><td>Excel 가져오기 작업을 선택 하고 헤더 행 내보내기/가져오기 여부를 설정할 수 있습니다.</td></tr><tr><td>엑셀 파일 경로</td><td>가져올 Excel 파일의 경로를 설정합니다 . "D:\export Excel\order list.xlsx"와 같이 파일의 전체 경로를 입력해야 하며 폴더는 기존 폴더여야 하며 접미사 ".xlsx"는 생략할 수 있습니다 .</td></tr><tr><td>가져온 Excel 시트 이름</td><td><p>엑셀에 여러 개의 워크시트가 있는 경우 가져올 워크시트를 선택할 수 있으며, 비워 두면 기본적으로 엑셀의 첫 번째 워크시트를 가져옵니다.</p><ul><li>인덱스 사용이 체크되지 않은 경우 가져올 Excel 워크시트의 이름을 입력합니다.</li><li>인덱스 사용 체크 시 불러온 엑셀 워크시트의 인덱스를 입력하면 인덱스가 1부터 시작됩니다.</li></ul><p></p></td></tr><tr><td>건너뛰는 행 수 </td><td>Excel의 처음 몇 행에 회사 이름 등 잘못된 데이터가 포함된 경우 건너뛴 행 수를 설정할 수 있습니다. 가져올 때 건너뛴 행 옆의 행부터 시작하는 Excel 열 이름을 기준으로 데이터를 가져옵니다.</td></tr><tr><td>테이블 선택 </td><td>Excel 로 가져올 테이블을 선택합니다 .</td></tr><tr><td>가져오기 모드 </td><td><p>작업을 Excel 로 가져오는 경우 가져오기 모드를 추가, 병합 및 바꾸기로 설정할 수 있습니다.</p><ul><li>추가: 원본 데이터를 기준으로 Excel 에서 데이터를 추가합니다.</li><li>병합: 새 데이터를 추가하고 참조 행의 데이터를 업데이트하며 기존 데이터를 삭제하지 않습니다.</li><li>바꾸기: 쿼리된 모든 데이터를 삭제하고 새 데이터를 추가합니다.</li></ul></td></tr><tr><td>열 선택</td><td>가져올 테이블을 선택 하면 모든 테이블의 열이 자동으로 나열되며 필요에 따라 열을 추가하거나 삭제할 수도 있습니다.</td></tr><tr><td>고급 설정</td><td><p>파일 비밀번호 가져오기: 비밀번호가 설정된 Excel 파일 가져오기를 지원합니다. 런타임 시 비밀번호가 설정된 Excel 파일을 가져올 때 사용자에게 비밀번호를 입력하라는 메시지가 표시됩니다.</p><p>참고: 가져온 파일에 설정된 비밀번호는 255자를 초과할 수 없습니다. 그렇지 않으면 올바른 비밀번호를 입력하더라도 잘못된 비밀번호가 프롬프트됩니다.</p></td></tr></tbody></table>

<figure><img src="../../../../.gitbook/assets/image (2177).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959472/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1675999591000\&api=v2)  설정구성이 완료되면 서버 명령을 호출할 수 있습니다.

페이지에서 셀 범위를 선택하여 버튼으로 설정합니다. 버튼의 명령을 편집하고 명령을 "서버단명령호출" 을선택한 다음 서버 명령 옆에 있는 드롭다운을 클릭하고 드롭다운 목록에서 서버 명령 "Excel 가져오기"를 선택한 다음 "고급 설정 표시"를 클릭합니다. "연결  데이터를 최신 정보로 업데이트하기" 선택하          면 서버가 Excel 가져오기 명령을 호출한 후 페이지가 데이터를 다시 로드하고 Excel 파일을 가져온 후 데이터를 표시합니다.

<figure><img src="../../../../.gitbook/assets/image (2176).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959472/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1675999591000\&api=v2)  설정이 완료되면 확인을 클릭하여 대화 상자를 닫습니다. 페이지를 실행하고,페이지에서 "Excel 가져오기" 버튼을 클릭하면 지정된 경로의 Excel 파일을 가져옵니다.

<figure><img src="../../../../.gitbook/assets/image (2106).png" alt=""><figcaption></figcaption></figure>
