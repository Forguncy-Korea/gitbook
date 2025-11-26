# forceSyncTableData 메서드

### 메서드&#x20;

Forguncy.forceSyncTableData(tableName, callback)

### 설명&#x20;

외부 테이블의 데이터를 복제본 테이블에 강제로 동기화합니다.

### 매개변수&#x20;

<table><thead><tr><th width="181.33333333333331">매개변수 </th><th width="156">형식 </th><th>설명 </th></tr></thead><tbody><tr><td>callback</td><td>Function</td><td>데이터를 동기화한 후 콜백 함수입니다.</td></tr><tr><td>tableName</td><td>string</td><td>데이터를 동기화할 복제본 테이블입니다.</td></tr></tbody></table>

### 반환값&#x20;

없음&#x20;

### 예제&#x20;

다음 예제 코드에서는 forceSyncTableData 메서드를 사용하여 외 테이블의 데이터를 복제본 테이블에 강제로 동기화합니다.

```javascript
// 외부 테이블의 데이터 동기화
Forguncy.forceSyncTableData("city",function (data) {
    // 동기화가 성공하면 동기화가 성공했음을 나타내는 경고 상자가 팝업됩니다.
    if(data){
        if(data.Success){
            alert("Success");
        }
        //동기화에 실패하면 경고창이 나타나 실패 정보를 보여줍니다.
        else{
            alert("Failed. ErrorMessage:" + data.ErrorMessage);
        }
    }
});
```

### 사용 예제&#x20;

![](https://help.grapecity.com.cn/download/thumbnails/72364673/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092718000\&api=v2) 연걸된 테이블의 복사본을 만듭니다.

<figure><img src="../../../../.gitbook/assets/image (1667).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364673/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092718000\&api=v2) 페이지에서 범위를 선택하고 아웃리치 테이블 복사본을 셀 범위로 드래그하여 필드를 바인딩합니다.

![](https://help.grapecity.com.cn/download/thumbnails/72364673/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092718000\&api=v2) 셀 범위를 선택하고 셀 유형을 단추로 설정하고 명령을 \[JavaScript 명령]으로 편집하고 JavaScript 코드를 입력합니다.

<figure><img src="../../../../.gitbook/assets/image (1844).png" alt=""><figcaption></figcaption></figure>

![](https://help.grapecity.com.cn/download/thumbnails/72364673/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092718000\&api=v2) 편집이 완료되면 \[확인]을 클릭하여 대화 상자를 닫습니다.

페이지를 실행하고 데이터 동기화 버튼을 클릭하면 동기화가 성공한다는 경고 상자가 나타납니다.

<figure><img src="../../../../.gitbook/assets/image (2085).png" alt=""><figcaption></figcaption></figure>
