# 서버단에서 Excel 파일 내보내기&#x20;

서버 명령에서 서버 가져오기 및 Excel 내보내기 명령을 사용하여 서버에서 Excel 데이터를 내보낼 수 있습니다.

다음은 서버 측 명령에서 서버 측 Excel 데이터 가져오기 및 내보내기 명령을 사용하여 서버 측에서 Excel 데이터를 내보내는 방법에 대한 자세한 소개입니다.

**단계**

![](https://help.grapecity.com.cn/download/thumbnails/80959506/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1675999835000\&api=v2)  프로젝트 매니저에서 서버단명령의 레이블을 마우스 오른쪽 버튼으로 클릭하고 "서버단  명령 생성하기"를선택하면 서버 커맨드 생성 대화상자가 팝업된다.

또는 "폴더 만들기"를 선택하여 폴더에 서버 명령을 만듭니다.

![](https://help.grapecity.com.cn/download/thumbnails/80959506/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1675999835000\&api=v2)  서버 명령 관리자에서 "새로 만들기"를 클릭하면 서버 명령 편집 대화 상자가 팝업되어 서버 명령의 일반 설정을 편집합니다. 서버 명령의 이름을 "Excel 내보내기"로 설정합니다.

<figure><img src="../../../../.gitbook/assets/image (2107).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959506/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1675999835000\&api=v2)  서버 명령을 편집하는 명령입니다. "명령 편집" 하이퍼링크를 클릭하여 서버 명령 편집 대화 상자를 팝업하고 서버 가져오기 및 내보내기 Excel 명령을 선택합니다. 명령 설정은 아래 표를 참조하십시오.

| 설정        | 설명                                                                                                             |
| --------- | -------------------------------------------------------------------------------------------------------------- |
| Excel 작업  | Excel 내보내기 작업을 선택하고 헤더 행 내보내기/가져오기 여부를 설정할 수 있습니다.                                                             |
| 엑셀 파일 경로  | 내보낼 Excel 파일의 경로를 설정합니다 . 파일의 전체 경로는 "D:\export Excel \order list.xlsx " 와 같이 입력해야 하며 접미사 ".xlsx"는 생략할 수 있습니다. |
| 테이블 선택    | Excel 로 내보낼 테이블을 선택합니다 .                                                                                       |
| 열 선택      | 내보낼 테이블을 선택하면 모든 테이블의 열이 자동으로 나열되며 필요에 따라 열을 추가하거나 삭제할 수도 있습니다.                                                |
|  고급설정     | 내보낸 파일을 암호화, 암호화 비밀번호 설정: 내보낸 파일을 암호화하려면 다음 텍스트 상자에 암호화 비밀번호를 설정하세요. 비밀번호는 직접 설정하거나 매개변수로 설정할 수 있습니다.          |

<figure><img src="../../../../.gitbook/assets/image (2160).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959506/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1675999835000\&api=v2)  설정구성이 완료되면 서버 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 영역을 선택하고 버튼으로 설정합니다. 버튼의 명령을 편집하고 명령을 "서버단명령"으로 선택한 다음 서버 명령 옆에 있는 드롭다운 버튼을 클릭하고 드롭다운 목록에서 서버 명령 "Excel 내보내기"를 선택합니다

<figure><img src="../../../../.gitbook/assets/image (1683).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80959506/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1675999835000\&api=v2)  설정이 완료되면 확인을 클릭하여 대화 상자를 닫습니다. 페이지를 실행하고,페이지에서 "Excel내보내기" 버튼을 클릭하면 지정된 경로 아래에 내보낸 Excel 파일이 표시됩니다.

<figure><img src="../../../../.gitbook/assets/image (2166).png" alt=""><figcaption></figcaption></figure>
