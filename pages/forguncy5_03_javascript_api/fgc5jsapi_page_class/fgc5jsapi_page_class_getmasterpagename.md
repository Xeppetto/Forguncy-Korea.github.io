---
title: Forguncy API - Page - getMasterPageName
tags: [Forguncy, JavaScript, API, getMasterPageName]
keywords: Forguncy API, JavaScript API, getMasterPageName
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getMasterPageName Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getMasterPageName.html
folder: forguncy5_03_javascript_api
---

### Page - getMasterPageName Method
page.getMasterPageName()
<br /><br />

### getMasterPageName Method 설명
화면에 보이는 페이지를 구성하는 요소 중 Forguncy에서 설정한 마스터페이지의 이름을 가져옵니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string : 마스터페이지의 이름을 반환
<br /><br />

### 활용 예제
아래는 page.getMasterPageName을 사용하는 관련 사용 예제입니다. 페이지 작성 시 Forguncy에서 설정했었던 마스터페이지의 정보를 보여줍니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;

  //화면에 표시되는 페이지에 설정됭 마스터페이지 이름을 확인합니다.
  var masterPageName = page.getMasterPageName();
  
  //마스터페이지의 이름을 화면에 표시합니다.
  alert(masterPageName);
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하여 아무 내용이나 넣습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getmasterpagename01.png)
    <br /><br />

2. 생성한 페이지 목록에서 마우스 오른쪽 클릭 > 마스터페이지 설정 > FGC_유저마스터페이지를 선택합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getmasterpagename02.png)
    <br /><br />

3. 해당 페이지에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getmasterpagename03.png)
    <br /><br />

4. 프로젝트를 실행하여 버튼을 누르면 해당 페이지에 설정했었던 마스터 페이지의 이름이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getmasterpagename04.png)

<br /><br />