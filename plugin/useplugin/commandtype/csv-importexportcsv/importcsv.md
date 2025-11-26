# CSV 가져오기

CSV 가져오기/내보내기 명령 중 CSV 처리 방식을 CSV로 가져오기를 하면 CSV데이터를 리스트뷰에 가져올 수 있습니다.&#x20;

### 사용방법&#x20;

1. 페이지에 CSV 가져오기 버튼과, 제품테이블과 연결한 리스트뷰를 생성해줍니다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (386).png" alt=""><figcaption></figcaption></figure>

2\. CSV가져오기 버튼 명령을 아래와 같이 설정합니다.&#x20;

&#x20; \- 명령 선택 : CSV 가져오기와 내보내기&#x20;

&#x20; \- CSV 처리 명령 : 가져오기&#x20;

&#x20; \- 리스트뷰 이름 : 리스트뷰1&#x20;

&#x20; \- 불러오기 모드 : 추가&#x20;

&#x20;   불러오기 모드에는 아래와 같이 3개의 모드가 있습니다. 예제에서는 추가모드를 사용합니다.&#x20;

&#x20;    . 추가 : 대상 리스트뷰에 레코드 추가&#x20;

&#x20;    . 합치기 : 대상 리스트뷰에 지정된 레코드의 데이터를 병합&#x20;

&#x20;    . 교체 : 데이터를 덮어씀&#x20;

&#x20; \- 열 : D6    CSV 열 이름 : 제품명&#x20;

&#x20;    열 : K6    CSV 열 이름 : 가격&#x20;

<figure><img src="../../../../.gitbook/assets/image (656).png" alt=""><figcaption></figcaption></figure>

3\. 실행을 하고, CSV 가져오기 버튼을 클릭한 후 파일을 선택하면 리스트뷰에 해당 CSV파일이 가져와진 것을 확인할 수 있습니다.&#x20;

<figure><img src="../../../../.gitbook/assets/picture (1).gif" alt=""><figcaption></figcaption></figure>
