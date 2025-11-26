# 논리 명령 - 조건

조건 명령을 사용하면 If, Else If 및 Else를 사용하여 조건의 다른 분기를 구성하고, 조건 집합을 설정하고, 조건이 충족되면 하나 또는 하나의 명령 집합을 실행하는 조건에 따라 다른 명령을 설정할 수 있습니다. 그렇지 않은 경우 다른 명령 또는 명령 집합이 실행됩니다.

if 다중 분기 조건문: 여러 조건에 따라 여러 분기를 선택하여 적절한 명령을 실행할 수 있습니다.

구문: if... else if...... else if...... else if...... else......

## 조건부 분기를 추가/제거

조건 명령에서 조건 중 하나를 충족하는 경우 해당 명령을 실행하기 위해 여러 조건문을 추가할 수 있습니다.

### 조건문 추가

명령을 \[조건] 명령으로 선택한 후 아래 조건 상자에서 \[Else 추가] 또는 \[ElseIf 추가]를 선택합니다.

![](<../../../.gitbook/assets/image (2223).png>)

또는 \[조건식]을 마우스 오른쪽 버튼으로 클릭하고 \[ElseIf 추가] 또는 \[Else 추가]를 선택합니다.

### 조건문 삭제&#x20;

조건문 상자에서 삭제를 클릭하여 조건문 삭제합니다.

![](<../../../.gitbook/assets/image (554).png>)

또는 \[조건식] 에서 마우스 오른쪽 버튼을 클릭하고 삭제를 선택합니다.

## 조건문 설정&#x20;

\[If/Else/ElseIf \[조건문]]을 클릭하여 오른쪽에 조건식, 확인 대화 상자, JavaScript 조건의 세 페이지 탭이 있으며, 설정사항은 아래 표에 나와 있습니다.

![](<../../../.gitbook/assets/image (493).png>)

<table><thead><tr><th width="178.33333333333331">설정1</th><th width="193">설정2</th><th>설명 </th></tr></thead><tbody><tr><td>조건식 </td><td>관계 </td><td>조건을 이전 조건과 통과 및/또는 연결합니다.</td></tr><tr><td>조건식 </td><td>괄호 </td><td><p>조건을 괄호로 묶고 최대 4개의 괄호를 지정할 수 있습니다.</p><p>괄호를 사용하여 "(A 및 B) 또는 C) 및 D"와 같은 복잡한 식을 설정할 수 있습니다.</p></td></tr><tr><td>조건식 </td><td>열 </td><td><p></p><p>쿼리할 테이블의 필드를 선택합니다.</p><ul><li>데이터 소스: 데이터 테이블에서 필드를 선택합니다. 작성자, 생성 날짜, 마지막 업데이트 및 마지막 업데이트 날짜는 활자 그리드에 의해 자동으로 추가되며 이러한 필드를 선택할 수도 있습니다.</li><li>페이지 요소: 페이지에서 셀 유형을 선택합니다.</li><li>로그인한 사용자: 로그인한 사용자의 사용자 이름, 전체 이름, 메시지, 역할 또는 조직 상위 사용자를 선택합니다.</li></ul></td></tr><tr><td>조건식 </td><td>연산자 </td><td>필드 및 값과 같은 조건을 비교합니다(예: 같음, 보다 크거나 같음).</td></tr><tr><td>조건식 </td><td>값 </td><td><p></p><p>비교할 값, 수식 또는 특정 키워드를 입력합니다.직접 입력하거나 클릭할 수 있습니다<img src="https://help.grapecity.com.cn/download/thumbnails/72354226/8-1-10-7_3.png?version=1&#x26;modificationDate=1648092557000&#x26;api=v2" alt="">마우스를 사용하여 셀 범위를 지정합니다.</p><p>기본 제공 키워드는 다음과 같습니다.</p><ul><li>%Null%: 입력(empty)이 없고 정의가 없음을 나타냅니다.</li><li>%CurrentUer.UserName%: 로그인한 사용자의 사용자 이름을 나타냅니다.</li><li>%CurrentUer.FullName%: 로그인한 사용자의 전체 이름을 나타냅니다.</li><li>%CurrentUer.Email%: 로그인한 사용자의 이메일 주소를 나타냅니다.</li><li>%CurrentUer.Role%: 로그인한 사용자의 그룹을 나타냅니다.</li><li>%CurrentUser.OrganizationSuperior%: 로그인한 사용자의 조직 상위를 나타냅니다.                        </li></ul><p></p></td></tr><tr><td>확인 대화 상자 </td><td>아이콘</td><td>없음, 묻기, 정보, 오류 및 경고로 설정할 수 있는 확인 대화 상자의 아이콘입니다.</td></tr><tr><td>확인 대화 상자</td><td>확인 대화 상자 제목 </td><td>대화 상자의 제목을 확인하고 제목 텍스트를 사용자 지정할 수 있습니다.</td></tr><tr><td>확인 대화 상자</td><td>텍스트 확인 </td><td>대화 상자의 내용을 확인하고 확인 텍스트를 사용자 지정할 수 있습니다.</td></tr><tr><td>확인 대화 상자</td><td>[예] 버튼 텍스트 / [아니오] 버튼 텍스트 </td><td>예 및 아니요 단추의 표시 텍스트는 텍스트 내용을 사용자 지정할 수 있습니다.</td></tr><tr><td>JavaScript 조건 </td><td>열기</td><td>Visual Studio와 같은 설정 응용 프로그램을 사용하여 해당 JavaScript 파일을 열고 설정되지 않은 경우 기본 프로그램으로 엽니다. 이 응용 프로그램에서 JavaScript 코드를 편집할 수 있으며 활자 격자가 자동으로 동기화됩니다.</td></tr><tr><td>JavaScript 조건 </td><td>연결 프로그램 </td><td>JavaScript 코드를 여는 응용 프로그램을 설정합니다.</td></tr><tr><td>JavaScript 조건 </td><td><img src="https://help.grapecity.com.cn/download/thumbnails/72354226/Image%2047.png?version=1&#x26;modificationDate=1648092557000&#x26;api=v2" alt=""></td><td>브라우저에서 JavaScript API 도움말 문서를 엽니다.</td></tr></tbody></table>

## 명령 설정&#x20;

\[If/Else/ElseIf \[조건식]에서 \[명령없]]을 클릭하여 오른쪽에서 원하는 명령을 선택합니다.

![](<../../../.gitbook/assets/image (1837).png>)
