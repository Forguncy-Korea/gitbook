# 워크플로우 설정&#x20;

{% file src="../../.gitbook/assets/workflowsample.fgko" %}

워크플로우의 설정에 대해 설명합니다. 워크플로우는 원래 상태, 대상 상태, 작업 및 담당자를 포함하는 여러 하위 프로세스로 구성됩니다.&#x20;

## 워크플로우 설정하기&#x20;

아래 절차대로 진행하세요.&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/56529783/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1611021585000\&api=v2) 데이터 테이블을 열고 테이블 설정에서 \[워크플로우 편집]을 클릭하여 워크플로우 설정 인터페이스로 이동합니다.&#x20;

<figure><img src="../../.gitbook/assets/image (1659).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56529783/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1611021585000\&api=v2) 워크플로우 활성화를 선택하여 워크플로우를 설정합니다. 테이블의 각 레코드에 대해 이 워크플로우가 처리됩니다.

<figure><img src="../../.gitbook/assets/image (1458).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56529783/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1611021585000\&api=v2) 워크플로우에 나타날 수 있는 모든 상태를 설정합니다. 이러한 "상태"는 프로세스의 각 단계에서 "원래상태" 및 "대상 상태"에 사용됩니다.

상태를 늘리거나 삭제하려면 +"-를 클릭할 수 있으며, 상태 이름은 자유롭게 정의할 수 있으며 순서는 위쪽 및 아래쪽 화살표를 클릭하여 변경할 수 있습니다.

첫 번째 상태는 레코드의 초기 상태에 사용되며 다른 상태는 순서를 사용자 지정할 수 있습니다. 상태 수도 변경할 수 있지만 원래 상태와 대상 상태를 모두 포함해야 합니다.

<figure><img src="../../.gitbook/assets/image (377).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56529783/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1611021585000\&api=v2) 워크플로우의 프로세스를  설정합니다. 이는 워크플로우의 비즈니스 처리 단계입니다. 일반 및 승인 프로세스를 추가할 수 있습니다.

목록에서 단계 행을 선택하여 단계의 정의, 즉 단계의 원래 상태, 작업, 조건, 대상 상태 및 담당자를 수정합니다. +와 -를 클릭하여 단계를 늘리거나 제거합니다.

<figure><img src="../../.gitbook/assets/image (1454).png" alt=""><figcaption></figcaption></figure>

* 일반 프로세스: 일반 프로세스에서 비즈니스는 설정된 고정 프로세스를 따라 단계적으로 진행해야 하지만 경우에 따라 승인자가 동일한 레코드를 여러 번 승인해야 합니다. 예를 들어, 신청서는 프로젝트 관리자-부서 관리자-일반 관리자의 순서로 승인되어야 하며, 프로젝트 관리자가 제출한 신청서의 경우 이 절차에 따라 신청서를 제출하고 승인해야 합니다. 부서 관리자가 제출한 요청인 경우 승인을 위해 일반 관리자에게 전달하기 전에 두 번 제출하고 승인해야 합니다. 이 경우 승인 프로세스를 사용하여 프로세스를 간소화할 수 있습니다.
* 승인 프로세스: 프로세스에 승인을 위해 여러 역할이 필요한 경우 여러 단계를 추가하는 일반 프로세스 대신 승인 프로세스를 설정할 수 있습니다. 승인 프로세스 중에 신청자의 역할이 승인 프로세스에 있는 경우 해당 사람이 제출한 응용 프로그램은 다음 승인 단계로 직접 전송됩니다. 연속된 두 개 이상의 승인 링크의 승인자가 동일한 경우 한 번만 승인하면 다음 승인 단계로 이동할 수 있습니다. 예를 들어, 신청서는 프로젝트 관리자-부서 관리자-일반 관리자의 순서로 승인되어야 하며, 프로젝트 관리자가 제출한 경우 제출 후 부서 관리자의 승인을 받아야 합니다. 부서 관리자가 제출한 신청서의 경우, 제출 후 일반 관리자의 승인을 위해 직접 입력됩니다. 프로젝트 관리자와 부서 관리자가 동일한 사람인 경우 일반 직원이 제출한 신청서는 부서 관리자의 승인을 한 번만 거치면 일반 관리자의 승인을 받을 수 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/56529783/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1611021585000\&api=v2)워크플로우를 설정하면  테이블에 상태,할당 정보가 추가됩니다. 해당 정보를 리스트뷰에 사용할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (1227).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/56527354/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1611021554000\&api=v2)설정이 완료되면 \[확인] 버튼을 클릭합니다. 페이지에서 프로세스 바를 설정합니다. 프로세스 바에 대한 자세한 내용은 [프로세스 바를](../../components/celltype/processbar.md) 참조하십시오.

페이지에서 셀 범위를 선택하고 셀 유형을 프로세스 바로 설정합니다. 프로세스 표시줄에는 현재 작업 레코드의 상태, 현재 소유자 정보 및 현재 사용자가 수행할 수 있는 작업이 표시됩니다.

현재 사용자가 작업 버튼 클릭하면 현재 레코드가 다음 상태로 전환되고 워크플로우는 프로세스에 설정된 단계를 따릅니다.
