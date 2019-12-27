---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Dec 23, 2019
summary: "Forguncy API - Namespace를 사용하는 방법을 안내합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_namespace.html
folder: forguncy5_03_javascript_api
---

## 설명
네임스페이스(이후 Namespace)는 변수 이름이나 함수 이름과 같이 명칭을 사용하는 공간으로 소속을 나타내며, Forguncy API를 사용할 때 Namespace는 'Forguncy'라고 선언합니다.

\

## 예제
아래 코드가 어떤 의미인지에 대해 지금은 자세히 아실 필요가 없습니다. 향후 해당 내용을 설명할 때 다시 자세히 설명할 예정입니다. 

**(1) 화면 내 특정 button을 불러오는 예제**

~~~javascript
  //현재 페이지를 네임스페이스에 지정하여 가져옵니다.
  var page = Forguncy.Page;
  
  //현재 페이지에서 button이라는 버튼을 가져옵니다.
  var cell = page.getCell("button");
~~~

**(2) Database의 값을 Listview에 입력한 후 해당 ListView의 값을 가져오거나, 특정 Cell에 저장하는 예제**

~~~javascript
    //현재 페이지를 네임스페이스에 지정하여 가져옵니다.
    var page = Forguncy.Page;

    //ListView 값을 가져오기
    var listview01 = page.getListView("ListView_동물");
    var listview02 = page.getListView("ListView_식물");

    //ListView 값을 특정 셀에 저장하기
    page.getCell("animalName01").setValue(listview01.getValue(0,2));
    page.getCell("animalName02").setValue(listview01.getValue(1,2));
~~~

위와 같이 모든 Forguncy API를 사용할 때 지정하는 Namespace는 Forguncy.page로 지정하여 사용합니다.
