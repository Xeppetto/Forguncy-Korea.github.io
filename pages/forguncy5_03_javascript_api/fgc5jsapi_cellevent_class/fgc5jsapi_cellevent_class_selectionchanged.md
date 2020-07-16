---
title: Forguncy JavaScript API - CellEvent - SelectionChanged
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, SelectionChanged, Web, JavaScript, API
last_updated: Jan 16, 2020
summary: "Forguncy JavaScript API - CellEvent 클래스 중 SelectionChanged Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cellevent-class-selectionchanged.html
folder: forguncy5_03_javascript_api
---

### CellEvent - SelectionChanged Method
CellEvents.selectionChanged
<br /><br />

### SelectionChanged Method 설명
지정한 특정 셀의 선택값이 변경되는 시점에 수행(trigger)되는 이벤트입니다. 콤보상자, 사용자선택상자 셀 유형을 지원합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string
<br /><br />

### 활용 예제
아래는 CellEvents.selectionChanged를 사용하는 예제입니다. 마우스가 지정한 그림 셀을 벗어나는 순간 글자 상자가 나타납니다.
<br />

~~~javascript
  //CallBack으로 사용할 이벤트를 정의합니다.
  var selectionChangedEvent  = function(arg) {
      alert("안녕하세요. Forguncy!");
  }
  
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;

  //Cell Name이 combo라고 되어 있는 셀 인스턴스 속성을 가져옵니다.
  var cell = page.getCell("combo");

  //combo 셀이 변경될 때 selectionChagnedEvent 이벤트를 binding합니다.
  cell.bind("selectionChanged", selectionChangedEvent);
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성하고, 콤보박스 셀을 생성합니다. 이후 왼쪽 상단의 Cell Name에 combo라고 입력합니다.<br />
  그런 다음 콤보박스 셀을 선택하고 오른쪽에 콤보박스에 나타날 값들을 입력해줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-selectionchanged01.png)
    <br /><br />

2. 콤보박스 셀을 클릭 후 '명령 편집'에서 "자바크스립트로 직접 프로그래밍하기" 명령을 추가하여, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-selectionchanged02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 나타나는 콤보박스의 값을 변경합니다. 첫 번 째 변경에 이벤트가 binding되고, 두 번 째 변경부터는 이벤트가 실행됩니다.<br />

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-selectionchanged03.gif)

    이벤트가 중첩되어 실행되는 것은 JavaScript 라이브러리의 이슈입니다. 실제 구현하실 때는 이를 고려하셔서 구현해 주세요.

<br /><br />
