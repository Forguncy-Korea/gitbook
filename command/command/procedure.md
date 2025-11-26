# 저장 프로시저  호출하기

저장 프로시저(Stored Procedure)는 특정 기능을 완성하기 위한 SQL문의 집합인 프로그래밍 가능한 함수 집합으로, 컴파일, 생성, 데이터베이스에 저장되며, 사용자는 저장 프로시저의 이름을 지정하고 매개변수를 부여하여 호출하고 실행할 수 있다.

<figure><img src="../../.gitbook/assets/image (2383).png" alt=""><figcaption></figcaption></figure>



## 저장 프로시저 호출하기 명령&#x20;

저장 프로시저 호출 명령을 사용할 때 연결된 데이터베이스에 매개 변수가 없는 저장 프로시저이거나 매개 변수가 있는 저장 프로시저일 수 있는 저장 프로시저가 이미 있는지 확인해야 합니다.

그렇지 않은 경우 저장 프로시저를 만들어야 합니다.

다음은 Mysql의 저장 프로시저 호출을 예로 들어 저장 프로시저 호출 명령의 사용법을 설명합니다.

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1673923107000\&api=v2)  아래 그림과 같이 이미 저장 프로시저가 있는 Mysql 데이터베이스에 연결합니다.

Mysql데이터베이스 연결에 대한 특정 작업은 [Mysql에 연결](../../database/externaldb/mysql-mariadb.md)을 참조하세요 .

<figure><img src="../../.gitbook/assets/image (2385).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1673923107000\&api=v2)  셀 범위를 선택하여 버튼으로 설정하고 명령을 "저장 프로시저 호출 명령"으로 편집합니다.

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1673923107000\&api=v2)  저장 프로시저 호출 명령을 설정합니다.

연결 문자열을 선택하고, 연결 문자열이 없으면 "연결 대화상자열기"를 클릭하여 직접 연결할 수 있습니다. 드롭다운 버튼을 클릭하고 연결 문자열을 선택합니다.

<figure><img src="../../.gitbook/assets/image (2386).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1673923107000\&api=v2)  연결 문자열을 선택한 후 연결된 데이터베이스에 저장 프로시저가 있으면 저장 프로시저 이름 목록에 바로 표시됩니다.

드롭다운 버튼을 클릭하고 저장 프로시저를 선택합니다.

<figure><img src="../../.gitbook/assets/image (2387).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1673923107000\&api=v2)  매개변수 설정. 저장 프로시저에 매개변수가 있는 경우 저장 프로시저를 선택하면 해당 매개변수가 매개변수 목록에 나열되며, 입력 값과 출력 값에 대한 셀을 설정할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (2388).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1673923107000\&api=v2) 데이터 세트를 변수로 반환합니다. 명령의 반환 결과 데이터 세트를 변수로 설정하여 저장 프로시저의 결과를 테이블에 표시합니다.

Oracle 및 PostgreSQL은 이 설정을 지원하지 않습니다.

<figure><img src="../../.gitbook/assets/image (2389).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A48.png?version=1\&modificationDate=1673923107000\&api=v2)  역할 권한. 이 저장 프로시저에 대한 명령을 실행할 수 있는 역할을 설정합니다.

<figure><img src="../../.gitbook/assets/image (2390).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/80941923/%E6%AD%A5%E9%AA%A49.png?version=1\&modificationDate=1673923107000\&api=v2)  설정이 완료되면 페이지를 실행합니다.  제품, 가격  값을 입력한 후 "프로시저" 버튼을 클릭합니다.

이때 저장 프로시저가 호출되고 저장 프로시저 내의 SQL 작업이 실행됩니다.&#x20;

<figure><img src="../../.gitbook/assets/image (2391).png" alt=""><figcaption></figcaption></figure>
