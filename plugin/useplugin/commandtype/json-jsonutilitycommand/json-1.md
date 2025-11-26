# JSON 역직렬화

JSON 역직렬화 명령을 사용하면 JSON 문자열을 JSON 객체로 변환할 수 있습니다.

### 사용 방법&#x20;

아래 JSON 문자열을 역직렬화 합니다.&#x20;

```
{"employee": [{ "first_name": "Katie",  "last_name": "Rodgers"}, 
{"first_name": "Naomi",  "last_name": "Green"}]}
```

1. 아래 그림과 같이 페이지 및 데이터 테이블을 생성합니다.&#x20;

* 데이터테이블 생성 :&#x20;

| 필드명       | 필드타입  |
| --------- | ----- |
| firstname | Text  |
| lastname  | Text  |

* 페이지 구성&#x20;

&#x20;    . 셀 영역을 지정한 후 셀 유형을 여러줄 텍스트  지정하고 해당 셀 이름 result로 설정

&#x20;    . 위의 데이터테이블을 연결한 리스트뷰 생성&#x20;

&#x20;    . JSON 직렬화 버튼 생성&#x20;

<figure><img src="../../../../.gitbook/assets/image (1289).png" alt=""><figcaption></figcaption></figure>

2\. "JSON 직렬화" 버튼의 명령을 생성합니다.&#x20;

2-1. JSON 역직렬화 명령을 아래와 같이 설정합니다.&#x20;

* 명령 선택 : JSON 역직렬화
* JSON 문자열 : result
* 결과를 파라미터로 반환 : res

<figure><img src="../../../../.gitbook/assets/image (597).png" alt=""><figcaption></figcaption></figure>

2-2. 루프 명령을 아래와 같이 설정합니다.&#x20;

* 명령 선택 : 루프 명령 만들기
* 반복횟수 선택&#x20;

&#x20;     \- 개수 혹은 배열 : res.employee

&#x20;     \- 반복항목/배열 대상 객체 파라미터 이름 : Item

<figure><img src="../../../../.gitbook/assets/image (616).png" alt=""><figcaption></figcaption></figure>

루프 명령 만들기의 하위 명령명령명 데이터 테이블 업데이트 명령을 아래와 같이 설정합니다.&#x20;

* 명령 선택 : 데이터 테이블 업데이트하기&#x20;
* 업데이트 형식 : 추가
* 열 : firstname    값 : =Item.first\_name
* 열 : lastname     값:  =Item.last\_name

<figure><img src="../../../../.gitbook/assets/image (689).png" alt=""><figcaption></figcaption></figure>

3\. 실행을 하여 여러줄 텍스트 박스에 아 JSON 문자열을 입력하고,  JSON 직렬화 버튼을 클릭하면 리스트뷰에 필드들이 저장되는 것을 확인할 수 있습니다.&#x20;

```
{"employee": [{ "first_name": "Katie",  "last_name": "Rodgers"}, 
{"first_name": "Naomi",  "last_name": "Green"}]}
```

<figure><img src="../../../../.gitbook/assets/image (1267).png" alt=""><figcaption></figcaption></figure>
