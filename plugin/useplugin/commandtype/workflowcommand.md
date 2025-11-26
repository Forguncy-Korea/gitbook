# 워크플로우 명령 (WorkflowCommand)

워크플로우 명령을 통해 워크플로우를 전송할 수 있으므로 전체 프로세스를 보다 정밀하게 제어할 수 있습니다. 워크플로우 명령 플러그인에는 워크플로우 명령 및 워크플로우 처리명령이 포함됩니다.

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr><tr><td>v 6. 0</td><td> <a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6_Plugin_20200903/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr><tr><td>v 5. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V5_Plugin_20191115/WorkflowCommand.zip">WorkflowCommand.zip</a></td></tr></tbody></table>

## 사용방법

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.

### 워크플로우 명령&#x20;

프로세스 바 셀 유형을 사용하여 워크플로우를 전환하기 전에 사용자는 프로세스 바 셀에서 "제출"을 클릭하여 다음 플로우로 들어갑니다. 워크플로우 명령을 통해 하나의 제출을 완료할 수 있습니다.&#x20;

명령창에서 "워크플로우 명령"을 선택하고 아래와 같이 설정합니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (400).png" alt=""><figcaption></figcaption></figure>



<table><thead><tr><th width="256">설정 </th><th>설명 </th></tr></thead><tbody><tr><td>대상 테이블 이름 </td><td>워크플로를 시작할 테이블을 선택합니다.</td></tr><tr><td>다음 상태</td><td>워크플로에 정의된 상태입니다.</td></tr><tr><td>담당자 할당 </td><td>다음 상태를 책임지는 사람.담당자가 여러 명인 경우 영문 쉼표로 구분하고, 담당자가 사용자 관리에 없을 경우 명령어 수행 시 오류가 발생합니다.</td></tr><tr><td>작업명 </td><td>기록 정보에서 볼 수 있는 작업의 이름입니다.</td></tr><tr><td>메모 </td><td>비고는 이력 정보에서 볼 수 있습니다.</td></tr></tbody></table>

### 워크플로우 처리 명령&#x20;

리스트뷰에 처리해야 하는 레코드가 여러 개인 경우 워크플로우 처리 명령을 사용하여 레코드를 일괄 처리할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (725).png" alt=""><figcaption></figcaption></figure>



| 설정           | 설명                                                                     |
| ------------ | ---------------------------------------------------------------------- |
| ListView 이름  | 리스트뷰 이름을 선택합니다                                                         |
| ListView 행   | 처리할 레코드를 설정하거나 모든 행을 선택하거나 행을 선택합니다.                                   |
| 작업명          | 선택한 레코드에 대해 수행할 작업의 이름을 설정합니다.                                         |
| 메모           | 메모를 직접 입력하거나 페이지에서 셀 범위를 선택하여 셀의 값을 메모로 가져올 수 있습니다. 메모는 기록에서 볼 수 있습니다. |
