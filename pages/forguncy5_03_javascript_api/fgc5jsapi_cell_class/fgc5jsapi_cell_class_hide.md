---
title: Forguncy API - Cell - hide
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, hide, Web, JavaScript, API
last_updated: Jan 15, 2020
summary: "Forguncy API - Cell 클래스 중 hide Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-hide.html
folder: forguncy5_03_javascript_api
---

### Cell - Hide Method
Cell.hide()
<br /><br />

### Hide Method 설명
특정 셀을 숨기기합니다. 셀을 숨길 때 셀에 입력된 값과 유형 등은 숨길 수 있지만, 셀의 배경색상은 숨길 수 없습니다. [show()](fgc5jsapi_cell-class-show.html) 메소드와 함께 사용할 수 있습니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 cell.hide를 사용하는 예제입니다. 버튼을 클릭하면 지정한 셀을 숨기기할 수 있습니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 "myCell"인 셀 인스턴스 정보를 가져옵니다.
  var cell = page.getCell("myCell");

  //myCell을 숨기기합니다.
  cell.hide();
~~~

<br />

### Forguncy 사용 예제

※참고 : show와 hide는 한 세트이므로 같은 예제가 구성되어 있습니다.

1. 페이지를 한 개 생성하고, 아무 유형이나 선택해 셀을 하나 생성합니다. 이후 좌측상단의 Cell Name에 'myCell'이라고 입력해 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hide01.png)
    <br /><br />

2. 버튼을 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hide02.png)
    <br /><br />

3. 또 다른 버튼을 추가로 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hide03.png)
    <br /><br />

4. 해당 프로젝트를 실행하면 작동하는 Cell의 UI로 활성화되어 있음을 알 수 있습니다.<br />
    이후 'Hide 버튼'을 클릭하면 해당 셀이 숨기기 처리되고, 'Show 버튼'을 클릭하면 보이기 처리됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hide04.gif)

<br /><br />