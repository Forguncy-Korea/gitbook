# AutoDisconnectTimeout 메서드

#### 메서드 <a href="#autodisconnecttimeout-fang-fa-fang-fa" id="autodisconnecttimeout-fang-fa-fang-fa"></a>

페이지.자동 연결 끊기타임아웃

#### 설명 <a href="#autodisconnecttimeout-fang-fa-miao-shu" id="autodisconnecttimeout-fang-fa-miao-shu"></a>

사용자 작업 시간 제한은 자동으로 연결을 끊고 동시 사용자 수를 해제합니다. 단위는 분이며 기본값은 0입니다.

#### **매개 변수**  <a href="#autodisconnecttimeout-fang-fa-can-shu-shuo-ming" id="autodisconnecttimeout-fang-fa-can-shu-shuo-ming"></a>

없음&#x20;

#### **반환값**  <a href="#autodisconnecttimeout-fang-fa-fan-hui-zhi" id="autodisconnecttimeout-fang-fa-fan-hui-zhi"></a>

없음&#x20;

#### 예제 <a href="#autodisconnecttimeout-fang-fa-shi-li" id="autodisconnecttimeout-fang-fa-shi-li"></a>

다음 예제 코드에서는 AutoDisconnectTimeout 메서드를 사용하여 시간 제한을 30으로 설정합니다.

```
// 현재 페이지 가져오기
var page = Forguncy.Page;
// 타임아웃설정 
page.AutoDisconnectTimeout = 30;
```
