---
title: Forguncy JavaScript API - Page - suspendCalc
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, suspendCalc, Web, JavaScript, API
last_updated: Jan 14, 2020
summary: "Forguncy JavaScript API - Page 클래스 중 suspendCalc Method에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-suspendcalc.html
folder: forguncy5_03_javascript_api
---

### Page - suspendCalc Method
Page.suspendCalc()
<br /><br />

### suspendCalc Method 설명
페이지 내 수식들을 작동하지 않도록 합니다. 페이지 내 계산을 다시 계속하기 위해 [resumeCalc](fgc5jsapi_page-class-resumecalc.html)와 함께 사용하시기를 추천합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.suspendCalc를 사용하는 관련 사용 예제입니다. resumeCalc와 함께 이용하면 해당 페이지의 수식 계산을 멈추거나, 계속 진행할 수 있습니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //페이지에서 수식 계산을 다시 진행합니다.
  page.suspendCalc();
~~~

<br />

### Forguncy 사용 예제

※알림: 아래 사용 예제는 [suspendCalc](fgc5jsapi_page-class-suspendcalc.html)와 [resumeCalc](fgc5jsapi_page-class-resumecalc.html)를 동시에 사용하므로, 같은 예제를 사용합니다.

1. 페이지를 한 개 생성하고, 셀 영역을 선택하여 "텍스트 상자"를 생성합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc01.png)
    <br /><br />

2. 텍스트 상자 아래 쪽에 병합 셀을 하나 생성하고, 위에서 생성한 텍스트 상자를 참조하도록 합니다. (화면에서 =B2로 표현되어 있습니다.)

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc02.png)
    <br /><br />

3. 해당 프로젝트를 실행하면 입력 박스 하나와 숫자 0이 나타납니다. 해당 입력 박스에 아무거나 입력 후 Enter키를 누르면 숫자 0은 입력한 대로 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc03.png)
    <br /><br />

4. Forguncy Editor로 돌아가 버튼을 한 개 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 생성하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc04.png)
    <br /><br />

5. 다시 해당 프로젝트를 실행한 후 "버튼"을 클릭합니다. 이후 입력 창에 아무거나 입력 후 Enter키를 눌러 봅니다. 값이 변경되지 않으면 suspendCalc가 잘 적용된 것입니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc05.png)
    <br /><br />

6. 다시 Forguncy Editor로 돌아가 버튼을 한 개 더 생성하고, 명령을 생성하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc06.png)
    <br /><br />

7. 다시 한 번 해당 프로젝트를 생성하고, 다음의 방법으로 테스트를 진행합니다.<br />
    (1) suspendCalc를 적용한 버튼을 클릭합니다.<br />
    (2) 입력 상자에 아무거나 입력 후 Enter키를 누릅니다. ▶ 값이 변하지 않으면 성공입니다.<br />
    (3) resumeCalc를 적용한 버튼을 클릭합니다.<br />
    (4) 입력 상자에 아무거나 입력 후 Enter키를 누릅니다. ▶ 값이 입력한 대로 변하면 성공입니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc07.gif)
    <br /><br />

<br /><br />