---
title: Forguncy API - Cell - getValue
tags: [Forguncy, JavaScript, API, getValue]
keywords: Forguncy API, JavaScript API, getValue
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 getValue Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-getvalue.html
folder: forguncy5_03_javascript_api
---

### Cell - getValue Method
cell.getValue()
<br /><br />

### getValue Method 설명
특정 셀에 입력된 값을 가져옵니다. 셀의 값을 가져와 여러가지 작업을 수행할 수 있습니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
아무거나, any
<br /><br />

### 활용 예제
아래는 page.getValue를 사용하는 예제입니다. 버튼을 클릭하면 지정된 셀을 비활성화할 수 있습니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 "myCell"로 되어 있는 셀 인스턴스 정보를 가져옵니다.
  var cell = page.getCell("myCell");

  //myCell에 기록된 값을 불러옵니다.
  var cellValue = cell.getValue();

  //myCell의 값을 팝업으로 화면에 표시합니다.
  alert(cellValue);
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀에 텍스르를 입력합니다. 이후 좌측상단의 Cell Name에 myCell이라고 입력해 줍니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getvalue01.png)
    <br /><br />

2. 버튼을 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getvalue02.png)
    <br /><br />

3. 해당 프로젝트를 실행하고, 버튼을 클릭하면 myCell에 입력된 값(value)가 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getvalue03.gif)

<br /><br />