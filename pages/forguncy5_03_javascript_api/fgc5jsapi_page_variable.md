---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Dec 23, 2019
summary: "Forguncy API - Page 변수를 사용하는 방법을 안내합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-variable.html
folder: forguncy5_03_javascript_api
---

## 설명
Forguncy API에서 Page 객체(Object)는 화면에 보이는 Forguncy로 제작한 웹페이지 객체를 말합니다. 
<br /><br />

## 유형
[Page 클래스 전체 보기](fgc5jsapi_page-class-list.html)

## 예제

**예제1) Cell 객체 불러오기**
Forguncy API의 Forguncy Namespace를 이용하여 페이지 객체를 선언하고, 해당 페이지에 존재하는 특정 Cell 객체를 불러옵니다.<br />

~~~javascript
  //현재 페이지를 Forguncy Namespace를 이용하여 불러옵니다.
  var page = Forguncy.Page;
  
  //현재 페이지에서 button이고 지정된 Cell을 가져옵니다.
  var cell = page.getCell("button");
~~~

**예제2) ListView 객체의 값들을 불러오기**
ListView 객체를 선언하여 해당 객체의 값들을 불러옵니다. 이후 다른 API들을 이용하여 해당 ListView 객체의 값들을 추가, 변경, 삭제 등을 구현하실 수 있습니다. 자세한 내용은 ListView 클래스를 참고하세요.

~~~javascript
    //현재 페이지를 Forguncy Namespace를 이용하여 불러옵니다.
    var page = Forguncy.Page;

    //ListView1이라는 객체의ㅌ 값들을 불러오기
    var listview = page.getListView("ListView1");
~~~
