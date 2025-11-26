# 저장 프로시저 호출하기

저장 프로시저는 프로그램 가능한 함수의 집합으로 특정 기능을 완성하기 위한 SQL 문 집합으로 데이터베이스에 컴파일, 생성 및 저장됩니다. 사용자는 저장 프로시저의 이름을 지정하고 매개변수를 지정하여 호출하고 실행할 수 있습니다.

이동 가능한 유형은 서버 측에서 저장 프로시저 호출 명령의 사용을 지원합니다.

## 저장프로시저 호출 명령&#x20;

다음은 SQL Server를 호출하는 저장 프로시저를 예로 들어 서버 명령에서 저장 프로시저 호출 명령을 사용하는 방법을 설명합니다.

**단계**

![](https://help.grapecity.com.cn/download/thumbnails/72358307/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092617000\&api=v2)  다음 그림과 같이 저장 프로시저가 있는 SQLServer 데이터베이스에 연결합니다.

SQL Server 데이터베이스에 연결하는 방법에 대한 자세한 내용은 SQL Server에 연결을 참조 [하십시오](https://help.grapecity.com.cn/pages/viewpage.action?pageId=46172273) .

![](<../../../.gitbook/assets/image (1295).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358307/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092617000\&api=v2)  개체 관리자에서서버 명령 탭을 마우스 오른쪽 버튼으로 클릭하고 "서버 명령 생성"을 선택하면 서버 명령 편집 대화 상자가 나타나 서버 명령의 일반 설정을 편집할 수 있습니다. 서버 명령의 이름을 "저장 프로시저 호출"로 설정합니다.

**그림 2 일반 설정**

![](https://help.grapecity.com.cn/download/attachments/72358307/image2021-10-25_19-9-2.png?version=1\&modificationDate=1648092616000\&api=v2\&effects=border-simple,blur-border)

![](https://help.grapecity.com.cn/download/thumbnails/72358307/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092617000\&api=v2)  매개변수를 편집합니다. 다음 두 매개변수를 추가합니다.

**그림 3 매개변수 추가**

![](https://help.grapecity.com.cn/download/attachments/72358307/image2021-10-25_19-9-43.png?version=1\&modificationDate=1648092616000\&api=v2\&effects=border-simple,blur-border)

![](https://help.grapecity.com.cn/download/thumbnails/72358307/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092617000\&api=v2)  서버단 명령을 편집하는 명령입니다. "명령 편집" 하이퍼링크를 클릭하여 서버 명령 편집 대화 상자를 엽니다.

매개변수 설정 명령을 사용하여 세 개의 매개변수를 설정한 다음 저장 프로시저 호출 명령을 선택하십시오.

* 연결 문자열: 연결 문자열을 선택하고 연결 문자열이 없으면 "연결 문자열 관리"를 직접 클릭하여 연결할 수 있습니다. 드롭다운 버튼을 클릭하여 연결 문자열을 선택합니다.
* 프로시저 이름: 연결 문자열을 선택한 후 연결된 데이터베이스에 저장 프로시저가 있는 경우 저장 프로시저 이름 목록에 직접 표시됩니다. 드롭다운 버튼을 클릭하여 저장 프로시저를 선택합니다.
* 매개변수 목록: 매개변수를 설정합니다. 저장 프로시저에 매개변수가 있는 경우 저장 프로시저를 선택한 후 매개변수 목록에 매개변수가 나열되며 매개변수에 대한 입력 및 출력 값을 설정할 수 있습니다.
* 데이터 세트를 변수로 반환: 이 명령의 반환된 결과 데이터 집합을 변수 로 설정하여 저장 프로시저의 결과를 테이블에 표시합니다. Oracle 및 PostgreSQL은 이 설정을 지원하지 않습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72358307/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092617000\&api=v2)  설정이 완료되면 이 서버 측 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼으로 설정합니다. 버튼의 명령을 편집하고 "서버 명령 호출"로 명령을 선택한 다음 서버 명령 뒤의 드롭다운을 클릭하고 드롭다운 목록에서 "저장 프로시저 호출"의 서버 명령을 선택하고, 파리미터 이름과  값을 설정합니다.&#x20;

![](<../../../.gitbook/assets/image (429).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72358307/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1648092616000\&api=v2)  설정이 완료되면 확인을 클릭하여 대화 상자를 닫습니다. Name과 CountryCode를 입력하고 저장프로시저 호출 버튼을 클릭합니다.&#x20;

이 때 서버 명령어가 호출되고 매개변수가 설정되고 저장 프로시저 호출 명령어가 호출되어 저장 프로시저의 SQL 연산이 실행됩니다.

다음 그림과 같이 F12 키를 눌러 개발자 도구를 열고 "콘솔"을 클릭합니다.

