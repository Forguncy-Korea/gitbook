# 조건 형식 - 확인 대화 상자

조건부 명령을 설정할 때 조건은 \[확인 대화 상자]를 선택하고 대화 상자의 내용에 따라 긍정 또는 부정 답변을 수행한 후 해당 명령을 실행합니다.

<figure><img src="../../../.gitbook/assets/image (2311).png" alt=""><figcaption></figcaption></figure>

## 대화 상자를 확인

확인 대화 상자에서 아이콘, 제목, 텍스트 및 예/아니요, 버튼,텍스트를 설정해야 합니다. 없음, 묻기, 정보, 오류 및 경고로 설정할 수 있습니다.

다음은 확인 대화 상자를 사용하는 방법을 보여 주는 예제입니다.

![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A41.png?version=1\&modificationDate=1648092558000\&api=v2) 주문 목록 페이지에서 다음 그림과 같이 리스트뷰 업데이터 명령만들기라는 명령으로 "추가" 버튼 설정합니다.

![](<../../../.gitbook/assets/image (1799).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A42.png?version=1\&modificationDate=1648092558000\&api=v2) 페이지에서 \[제출] 버튼 추가하여 명령을 \[조건] 명령으로 설정합니다.

![](<../../../.gitbook/assets/image (1512).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A43.png?version=1\&modificationDate=1648092558000\&api=v2) 조건을 설정합니다. \[If \[조건식]을 클릭하고 \[확인 대화 상자]를 선택합니다.

아이콘, 확인 대화 상자 제목, 텍스트 확인 및 예/아니요 버튼의 텍스트를 설정할 수 있습니다.

확인 텍스트를 설정할 때 수식 사용을 선택하여 페이지의 셀을 선택합니다.

![](<../../../.gitbook/assets/image (423).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A44.png?version=1\&modificationDate=1648092558000\&api=v2)  명령을 설정합니다. \[If \[조건식]에서 \[빈 명령]을 클릭하고 오른쪽의 \[명령 선택] 콤보 상자에서 \[리스트뷰 업데이트 명령 만들기]를 선택합니다. 유형은 \[리스트뷰 반영]입니다.

설정이 완료되면 확인을 클릭합니다.

![](<../../../.gitbook/assets/image (1079).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A45.png?version=1\&modificationDate=1648092558000\&api=v2)  조건부 분기를 추가합니다. \[조건-> Else 추가]를 선택하면 팝업 확인 대화 상자에서 \[아니오]를 선택한 후 명령이 실행되지 않는 명령을 설정할 수 있습니다.

설정이 완료되면 확인을 클릭합니다.

![](<../../../.gitbook/assets/image (1563).png>)

![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A46.png?version=1\&modificationDate=1648092558000\&api=v2) 페이지를 실행한 후 추가 버튼 클릭하면 데이터가 데이터베이스에 커밋되지 않은 주문 목록에 새 레코드가 추가됩니다.

![](<../../../.gitbook/assets/image (1628).png>)



![](https://help.grapecity.com.cn/download/thumbnails/72354281/%E6%AD%A5%E9%AA%A47.png?version=1\&modificationDate=1648092558000\&api=v2) \[제출] 버튼을 클릭하면 확인 대화 상자가 나타납니다.

* \[예]를 선택하면 양식 제출 작업이 수행되어 데이터가 데이터베이스에 제출됩니다.

![](<../../../.gitbook/assets/image (452).png>)
