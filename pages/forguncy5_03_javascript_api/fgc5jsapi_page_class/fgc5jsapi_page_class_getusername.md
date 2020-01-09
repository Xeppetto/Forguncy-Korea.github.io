---
title: Forguncy API - Page - getUserName
tags: [Forguncy, JavaScript, API, getUserName]
keywords: Forguncy API, JavaScript API, getUserName
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getUserName에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getusername.html
folder: forguncy5_03_javascript_api
---

### Page - getUserName Method
page.getUserName()
<br /><br />

### getUserName Method 설명
현재 로그인하여 서비스를 사용 중인 사용자의 이름을 가져옵니다. 로그인한 사용자가 없는 경우 null값을 반환합니다. 
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string : 사용자의 이름을 반환

 <br /><br />

### 활용 예제
아래는 page.getUserName을 사용하는 관련 사용 예제입니다. 로그인한 사용자의 이름을 보여줍니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //로그인한 사용자의 이름을 가져옵니다.
  var userName = page.getUserName();

  //로그인한 사용자의 이름을 화면에 표시합니다.
  alert(userName);
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 생성한 후 셀에 "현재 사용자" 셀 유형을 적용합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getusername01.png)]
    <br /><br />

2. 해당 페이지에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getusername02.png)]
    <br /><br />

3. 프로젝트를 실행하여 버튼을 누르면 getUserName을 화면에 표시합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getusername03.png)]


<br /><br />