---
title: Forguncy API - Page - recalc
tags: [Forguncy, JavaScript, API, recalc]
keywords: Forguncy API, JavaScript API, recalc
last_updated: Jan 13, 2020
summary: "Forguncy API - Page 클래스 중 recalc Method와 관련해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-recalc.html
folder: forguncy5_03_javascript_api
---

### Page - recalc Method
page.recalc()
<br /><br />

### recalc Method 설명
페이지 내 모든 수식을 다시 계산하도록 합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.recalc를 사용하는 관련 사용 예제입니다. 해당 페이지의 수식을 강제로 다시 계산합니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //페이지의 모든 수식을 강제로 다시 계산하도록 합니다.
  page.recalc();
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀에 =NOW()라고 입력합니다. 해당 함수는 Excel에서 "현재 날짜와 시간"을 표시하는 함수입니다.<br />
    ※참고 : Forguncy는 Excel에서 사용하는 함수를 사용하여 웹에서 결과를 볼 수 있도록 해 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-recalc01.png)
    <br /><br />

2. 버튼을 추가합니다. '명령 편집'으로 '자바스크립트로 직접 프로그래밍하기'하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-recalc02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 버튼을 클릭하면 아래와 같이 현재 시간이 변경되어 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-recalc03.gif)

<br /><br />