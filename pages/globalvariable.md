# 전역변수&#x20;

전역 변수는 포건시로 생성할 수 있으며, AppKey, AppSecret, 일부 토큰 등 애플리케이션 실행 중 장기간 저장해야 하는 값을 전역 변수에 저장할 수 있어 편리하다. 나중에 전화해서 관리할 수 있습니다.

전역 변수에 대한 참조를 생성, 삭제, 수정 및 찾을 수 있습니다.

전역 변수는 서버 측에서만 사용할 수 있습니다. 배포 후 관리 콘솔에서 변수 값을 변경할 수 있습니다.



리본의 메뉴바에서 "수식-전역변수"를 선택하면 전역변수 생성 대화상자가 나타납니다.

<figure><img src="../.gitbook/assets/image (1911).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (428).png" alt=""><figcaption></figcaption></figure>

전역 변수 생성 대화 상자에서 "새로 만들기"를 클릭하고 전역 변수의 이름과 값을 입력하며 값은 고정 값만 가능합니다 .

생성된 전역 변수에 대해 참조 삭제 및 찾기 등의 작업도 수행할 수 있습니다.&#x20;

<figure><img src="../.gitbook/assets/image (2297).png" alt=""><figcaption></figcaption></figure>

## 수식에서 전역 변수 사용&#x20;

서버 측 명령을 편집할 때 수식을 입력할 수 있는 모든 곳에서 전역 변수를 호출할 수 있으며 모든 전역 변수가 자동으로 나열됩니다.

사용시 "=전역변수 1"과 같이 수식을 직접 입력하거나![](https://help.grapecity.com.cn/download/thumbnails/80959800/image2023-2-16_16-44-32.png?version=1\&modificationDate=1676537072000\&api=v2), 팝업 대화 상자에서 변수를 선택하고 삽입을 두 번 클릭합니다.

<figure><img src="../.gitbook/assets/image (1909).png" alt=""><figcaption></figcaption></figure>

## **명령을 통해 전역 변수의 값을 편집** <a href="#id-di-shi-ba-zhang-quan-ju-bian-liang-4.-tong-guo-ming-ling-bian-ji-quan-ju-bian-liang-de-zhi" id="id-di-shi-ba-zhang-quan-ju-bian-liang-4.-tong-guo-ming-ling-bian-ji-quan-ju-bian-liang-de-zhi"></a>

전역 변수 설정 명령으로 전역 변수의 값을 편집할 수 있습니다.

서버 명령을 생성하고 명령을 "전역 변수 값  설정"으로 설정합니다. 이름 열의 드롭다운 버튼을 클릭하여 전역 변수를 선택한 후 새 값을 설정합니다.

설정이 완료된 후 이 명령어를 다시 호출하면 변수를 참조하는 모든 위치가 새로 고쳐집니다.

<figure><img src="../.gitbook/assets/image (1916).png" alt=""><figcaption></figcaption></figure>

## 서버 관리자에서 전역 변수 값 편집&#x20;

포건시서버관리자에 들어가 "앱목록"에서 응용 프로그램을 클릭하면 "전역 변수" 탭에서 응용 프로그램의 모든 전역 변수를 볼 수 있습니다.

여기에서 전역 변수의 값을 편집하고 편집 후 "설정 저장"을 클릭하면 이 변수를 참조하는 모든 위치가 새로 고쳐집니다.

<figure><img src="../.gitbook/assets/image (550).png" alt=""><figcaption></figcaption></figure>
