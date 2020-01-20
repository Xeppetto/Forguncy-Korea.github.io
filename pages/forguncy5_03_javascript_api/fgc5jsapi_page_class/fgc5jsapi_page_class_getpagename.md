---
title: Forguncy API - Page - getPageName
tags: [Forguncy, JavaScript, API, getPageName]
keywords: Forguncy API, JavaScript API, getPageName
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getPageName Method에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getPageName.html
folder: forguncy5_03_javascript_api
---

### Page - getPageName Method
Page.getPageName()
<br /><br />

### getPageName Method 설명
화면에 표시되는 현재 페이지의 이름을 가져옵니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string : 해당 페이지의 이름을 반환
<br /><br />

### 활용 예제
아래는 page.getPageName을 사용하는 관련 사용 예제입니다. 해당 페이지의 이름을 보여줍니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //화면에 표시되는 페이지의 이름을 확인합니다.
  var pageName = page.getPageName();

  //페이지의 이름을 화면에 표시합니다.
  alert(pageName);
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고 우측 패널에서 "페이지 설정" 탭을 선택 후 페이지의 "이름"을 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getpagename01.png)
    <br /><br />

2. 해당 페이지에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getpagename02.png)
    <br /><br />

3. 프로젝트를 실행하여 버튼을 누르면 해당 페이지에 설정했었던 페이지의 이름이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getpagename03.gif)

<br /><br />