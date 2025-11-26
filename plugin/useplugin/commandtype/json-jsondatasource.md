# JSON 데이터소스 가져오기(JSONDataSource)

JSON 데이터 소스 가져오기 명령은 JSON의 내용을 리스트뷰나 셀로 추출할 수 있는 플러그인입니다.&#x20;

### 플러그인 다운로드&#x20;

버전에 맞는 플러그인을 다운로드 합니다.

<table><thead><tr><th width="139">버전 </th><th>다운로드 링크 </th></tr></thead><tbody><tr><td>v10.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V10_Plugin/JsonDataSource.zip">JsonDataSource.zip</a></td></tr><tr><td>v 9.0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V9_Plugin/JsonDataSource.zip">JsonDataSource.zip</a></td></tr><tr><td>v 7. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7.1_Plugin_20211223/JsonDataSource.zip">JsonDataSource.zip</a></td></tr><tr><td>v 7. 0</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V7_Plugin_20210722/JsonDataSource.zip">JsonDataSource.zip</a></td></tr><tr><td>v 6. 1</td><td><a href="https://forguncy-korea.github.io/attached_files/Plugin_Files/V6.1_Plugin_20201111/JsonDataSource.zip">JsonDataSource.zip</a></td></tr></tbody></table>



### 사용 방법&#x20;

1. 플러그인을 다운로드합니다.
2. Forguncy Builder에서 설치하고 Forguncy Builder를 다시 실행합니다.
3. 데이터 테이블을 아래와 같이 만들어줍니다.&#x20;

| 필드명            | 필드속성  |
| -------------- | ----- |
| name           | Text  |
| age            | Text  |
| secretIdentity | Text  |
| powers         | Text  |

&#x20; 4\. 페이지에 여러줄 텍스트 셀유형, 3번에서 만든 데이터 테이블을 연결한 리스트뷰와&#x20;

&#x20;   버튼을 만듭니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (2266).png" alt=""><figcaption></figcaption></figure>

&#x20; 5\. 명령창에 "JSON 데이터를 셀로 가져오기" 또 "JSON 데이터를 리스트뷰로 가져오기"를 선택합니다.

* JSON 데이터를 셀로 가져오기&#x20;

<figure><img src="../../../.gitbook/assets/image (1370).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (2045).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="270">항목 </th><th>설명 </th></tr></thead><tbody><tr><td>JSON 데이터 소스 </td><td>JSON  데이터 소스가 있는 셀 </td></tr><tr><td>JSON 설정 예제 </td><td>JSON 설정 예제를 입력하면  JSON 경로 및 목표 셀의 속성 이름에 속성이 나타남 </td></tr><tr><td>JSON 경로 </td><td>JSON 경로 </td></tr><tr><td>속성 이름 </td><td>JSON 속성 경로 </td></tr><tr><td>셀 </td><td>속성 경로가 입력될 셀 </td></tr></tbody></table>

* JSON 데이터를 리스트뷰로 가져오기&#x20;

<figure><img src="../../../.gitbook/assets/image (1699).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="270">항목 </th><th>설명 </th></tr></thead><tbody><tr><td>JSON 데이터 소스 </td><td>JSON  데이터 소스가 있는 셀 </td></tr><tr><td>JSON 설정 예제 </td><td>JSON 설정 예제를 입력하면  JSON 경로 및 목표 셀의 속성 이름에 속성이 나타남 </td></tr><tr><td>JSON 경로 </td><td>JSON 경로 </td></tr><tr><td>리스트뷰 </td><td>JSON 데이터를 가져올 리스트뷰 </td></tr><tr><td>속성 이름</td><td>JSON 속성 경로 </td></tr><tr><td>셀 </td><td>속성 경로가 입력될 리스트뷰의 셀 </td></tr></tbody></table>

6\. 실행을 하고 여러줄 텍스트에 아래 코드를 입력합니다.&#x20;

```
{
  "squadName": "Super hero squad",
  "homeTown": "Metro City",
  "formed": 2016,
  "secretBase": "Super tower",
  "active": true,
  "members": [
    {
      "name": "Molecule Man",
      "age": 29,
      "secretIdentity": "Dan Jukes",
      "powers": [
        "Radiation resistance",
        "Turning tiny",
        "Radiation blast"
      ]
    },
    {
      "name": "Madame Uppercut",
      "age": 39,
      "secretIdentity": "Jane Wilson",
      "powers": [
        "Million tonne punch",
        "Damage resistance",
        "Superhuman reflexes"
      ]
    },
    {
      "name": "Eternal Flame",
      "age": 1000000,
      "secretIdentity": "Unknown",
      "powers": [
        "Immortality",
        "Heat Immunity",
        "Inferno",
        "Teleportation",
        "Interdimensional travel"
      ]
    }
  ]
}
```

&#x20;"데이터 셀로 가져오기" 와 "데이터 리스트뷰 가져오기" 버튼을 클릭하면 아래와 같이 셀과 리스트뷰에 JSON 데이터를 가져오는 것을 확인할 수 있습니다.&#x20;

<figure><img src="../../../.gitbook/assets/image (1639).png" alt=""><figcaption></figcaption></figure>
