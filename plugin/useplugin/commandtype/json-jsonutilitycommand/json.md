# JSON 직렬화

JSON 직렬화 명령을 통해 JSON객체를 JSON 문자열로 변환할 수 있습니다.

### 사용 방법

아래 JSON 문자열을 직렬화 합니다.&#x20;

```
[{ name: '원빈', age: 37, major: '경제학', hobby: '코딩' },
{ name: '이나영', age: 31, major: '경영학', hobby: '디자인' },
{ name: 'curryyou', age: 21, major: '역사', hobby: '글쓰기' }]
```

1. 페이지에 "직렬화(Stringfy)"버튼과 여러줄 텍스트에 JSON 객체를 입력하고, 여러줄 텍스트에 결과값 (JSON 문자열)이 나올 수 있게 구성합니다.&#x20;

<figure><img src="../../../../.gitbook/assets/image (650).png" alt=""><figcaption></figcaption></figure>

&#x20; 2\. 버튼을 선택하고 명령편집을 아래와 같이 설정합니다.

&#x20;  \[JSON 직렬화 명령 설정하기]

* 명령선택 : JSON 직렬화 명령
* 객체 : =AB9
* 결과를 파라미터로 반환 : Json\_string

<figure><img src="../../../../.gitbook/assets/image (2202).png" alt=""><figcaption></figcaption></figure>

\[셀 속성과 내용 변경하기]

* 명령 선택: 셀 속성과 내용 변경하기
* 대상셀:=G21          속성 유형: 대상 셀에 설정 값을 입력            설정 값:=Json\_string

<figure><img src="../../../../.gitbook/assets/image (1871).png" alt=""><figcaption></figcaption></figure>



3\. 실행을 하고, 직렬화(Stringfy)버튼을 클릭하면 JSON 객체가 문자열로 나오는 것을 확인할 수 있습니다.

<figure><img src="../../../../.gitbook/assets/image (1180).png" alt=""><figcaption></figcaption></figure>
