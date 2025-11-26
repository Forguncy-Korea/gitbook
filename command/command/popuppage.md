# 페이지 명령 - 팝업 페이지

팝업 페이지 명령을 사용하여 다른 작은 페이지를 페이지에 팝업하고 가운데에 표시하며 일반적으로 버튼, 하이퍼링크 등과 같은 셀 유형에 사용됩니다.

## 팝업 페이지 설정&#x20;

팝업 명령에서 앱의 페이지인 팝업 페이지를 설정해야 합니다.

### 페이지 선택

페이지를 선택하면 앱의 모든 페이지가 나열되고 페이지 중 하나가 선택되고 명령이 실행되면 페이지가 나타납니다.

* 내부 페이지: 내부 페이지의 이름을 입력하면 앱에서 페이지를 선택하는 것과 동일한 효과를 내어 내부 페이지가 직접 팝업됩니다.

<figure><img src="../../.gitbook/assets/image (2481).png" alt=""><figcaption></figcaption></figure>

* 셀에서 페이지 이름 값 선택     : 수식을 직접 입력하거나 페이지에서 셀을 선택하여 수식의 계산 또는 셀 값에 따라 해당 페이지를 팝업할 수 있습니다.

![](<../../.gitbook/assets/image (1787).png>)

실행 후 팝업 버튼을 클릭하면 "=B5" 수식의 계산 결과에 따라 주문 목록 페이지가 나타납니다.

![](<../../.gitbook/assets/image (2237).png>)

{% hint style="info" %}
페이지 이동 명령 뒤에 있는 명령은 실행되지 않습니다.&#x20;
{% endhint %}

### 고급 설정&#x20;

팝업 페이지 명령의 고급 설정은 페이지 이동 명령의 고급 설정과 동일합니다.



* [고급 설정 - 페이지 전송 값](movepage/pagevalue.md)
* [고급 설정 - 캐시를 제거](movepage/delcash.md)
* [고급 설정 -바인딩 된 데이터 설정을 로드](movepage/loadbounddatasetting.md)

**팝업 페이지를 닫은 후 실행되는 명령**

팝업 페이지가 닫힌 후 실행될 명령을 설정할 수 있습니다. 팝업 페이지 닫기 명령에 정의된 반환 결과 및 반환 값은 컨텍스트에서 얻을 수 있습니다. 자세한 내용은 [고급 설정](closepopuppage/advanced-settings.md)을 참조하세요 .

컨텍스트 변수에는 대상 페이지의 모든 팝업 페이지 닫기 명령의 반환 값이 나열됩니다.<br>

<figure><img src="../../.gitbook/assets/image (2482).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2484).png" alt=""><figcaption></figcaption></figure>



### 기타 설정&#x20;

기본적으로 팝업 페이지의 오른쪽 상단에 닫기 버튼이 있습니다.![](https://help.grapecity.com.cn/download/thumbnails/80941174/image2018-12-11_11-6-10.png?version=1\&modificationDate=1673923094000\&api=v2), 팝업 페이지를 닫으려면 닫기 버튼을 클릭하십시오.

닫기 버튼을 숨길 수도 있습니다. "파일->옵션->응용 프로그램 설정"을 선택하고 인터페이스 설정 영역 하단에서 아래 그림과 같이 "팝업 닫기 버튼 숨기기"를 체크합니다.

<figure><img src="../../.gitbook/assets/image (750).png" alt=""><figcaption></figcaption></figure>
