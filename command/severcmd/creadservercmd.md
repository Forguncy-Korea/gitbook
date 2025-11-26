# 서버단 명령 만들기

서버단 명령을 정의한 후에는 페이지에 계산 논리를 배치하는 대신 서버 쪽에서 실행됩니다. 이렇게 하면 동적 데이터 수집 및 계산의 논리를 더 잘 수행할 수 있습니다.



서버 명령 기능은 기본적으로 개체 관리자에 표시되지 않는 고급 기능입니다 .프로젝트 탐색기에 있는 ![](https://help.grapecity.com.cn/download/thumbnails/80946150/image2023-1-9_11-57-14.png?version=1\&modificationDate=1673923167000\&api=v2)버튼을  클릭하여 서버단 명령 앞의 확인란을 선택하고 "확인"을 클릭하면 개체 관리자에 서버 명령이 표시됩니다.



<figure><img src="../../.gitbook/assets/image (2125).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2135).png" alt=""><figcaption></figcaption></figure>

## 서버단 명령 만들기&#x20;

다음은 서버단 CSV 가져오기/내보내기 명령을 만드는 것과 같이 서버단 명령을 만드는 일반적인 단계를 보여줍니다.&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72357163/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092602000\&api=v2)  개체 관리자의 서버 쪽 명령 탭을 마우스 오른쪽 버튼을 클릭하고 서버 쪽 명령 만들기를 선택하여 서버단 명령 만들기 대화 상자를 나타납니다.

또는 폴더 만들기를 선택하여 폴더에 서버단 명령을 만듭니다.

![](<../../.gitbook/assets/image (735).png>)

리본 메뉴 모음에서 만들기를 클릭하고 서버 개체 영역에서 서버단 명령을 클릭하여 서버 명령 만들기 대화 상자를 팝업할 수도 있습니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357163/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092602000\&api=v2) 서버 명령의 일반 설정을 편집합니다. 설정 명령의 이름은 \[CSV 내보내기]입니다.

![](https://help.grapecity.com.cn/download/thumbnails/72357163/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092602000\&api=v2)  서버단 명령을 편집하는 명령입니다. \[명령 편집] 하이퍼링크를 클릭하고 서버 명령 편집 대화 상자를 표시하고 CSV 가져오기/내보내기 명령을 선택합니다.

CSV 내보내기를 선택하고, 데이터 테이블 및 CSV의 파일 경로를 선택합니다. 폴더는 이미 있는 폴더여야 하며 확장 ".csv"은 생략할 수 있습니다.

![](<../../.gitbook/assets/image (1935).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357163/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092602000\&api=v2) 서버단 명령을 만든 후 개체 관리자의 서버단 명령 레이블 아래에 표시됩니다.

서버 명령 앞에 있는 확장을 클릭하면 서버 명령을 관리하고 일반/파라미터/명령을 두 번 클릭하면 해당 탭이 직접 팝업되어 보고 수정할 수 있습니다.![](https://help.grapecity.com.cn/download/thumbnails/72357163/image2020-9-18_16-6-47.png?version=1\&modificationDate=1648092602000\&api=v2)

서버단 명령을 선택하고 마우스 오른쪽 버튼을 클릭하면 마우스 오른쪽 버튼 클릭 메뉴가 나타나고 이 쪽 명령을 사용하지 않도록 설정하거나 서버 쪽 명령을 복사하도록 선택할 수 있습니다.

![](<../../.gitbook/assets/image (1210).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357163/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092602000\&api=v2) 설정이 완료되면 이 서버단 명령을 호출할 수 있습니다.

예를 들어 페이지에서 셀 범위를 선택하고 버튼을 설정합니다. 버튼의 명령을 편집하고 "서버 명령 호출"으로 명령을 선택한 다음 서버단 명령 뒤에 있는 드롭다운을 클릭하고 드롭다운 목록에서 "CSV 내보내기"를 선택합니다.

![](<../../.gitbook/assets/image (1960).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72357163/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1648092602000\&api=v2) 설정이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다. 페이지를 실행합니다.페이지에서 \[CSV 내보내기]버튼을 클릭하면 설정된 지정된 경로 아래에 내보낸 CSV 파일이 표시됩니다.

![](<../../.gitbook/assets/image (1674).png>)

{% hint style="info" %}
서버단 명령을 만든 후 일반 탭 아래의 테스트 버튼을 클릭하여 페이지에서 호출하지 않고 빌더에서 직접 실행할 수 있습니다.

\[테스트] 버튼을 클릭하면  대화 상자가 표시됩니다. 이 서버단 명령을 실행하려면 사용자를 선택해야 합니다.

서버 명령에 파라미터가 있는 경우 서버 명령의 파라미터도 대화상자에 나열됩니다.

명령이 테스트되면 진행률 창이 표시됩니다. 실행이 완료되면 결과 대화 상자가 표시됩니다. 반환 코드 및 실행 로그가 대화 상자에 표시됩니다.
{% endhint %}

### 테스트 서버 명령 <a href="#ce-shi-fu-wu-duan-ming-ling" id="ce-shi-fu-wu-duan-ming-ling"></a>

서버 측 명령을 생성한 후 일반 탭에서 "테스트" 버튼을 클릭하면 서버 측 명령을 페이지에서 호출하지 않고 디자이너에서 직접 실행할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (233).png" alt=""><figcaption></figcaption></figure>

"테스트" 버튼을 클릭하면 다음 대화 상자가 나타납니다. 이 서버 명령을 실행하려면 사용자를 선택해야 하며 요청 시간 제한을 설정할 수 있습니다. 기본값은 100초입니다.

서버 측 명령을 테스트할 때 디자이너는 서버 측 명령을 실행하라는 요청을 서버에 보냅니다. 실행 시간이 요청 시간을 초과하면 요청 시간 초과 오류가 자주 발생합니다. 서버 명령이 완료 후 정보를 반환하도록 요청 시간 제한을 설정할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (234).png" alt=""><figcaption></figcaption></figure>

서버 명령에 매개변수가 있는 경우 서버 명령에 대한 매개변수도 대화 상자에 나열됩니다.

테스트가 명령되는 동안 진행 창이 표시됩니다. 실행이 완료되면 결과 대화 상자가 표시됩니다. 반환 코드와 실행 로그가 대화 상자에 표시됩니다.

클릭하면 ![](https://gccndocumentsitestorage.blob.core.chinacloudapi.cn/document-site-files/images/8ca07557-62b8-4219-8ddd-357e505dc985/80946150/image2023-1-31_17-50-17.png)로그 정보를 복사할 수 있습니다.

<figure><img src="../../.gitbook/assets/image (235).png" alt=""><figcaption></figcaption></figure>
