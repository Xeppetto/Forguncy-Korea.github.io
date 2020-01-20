---
title: Forguncy API - Cell - bind
tags: [Forguncy, JavaScript, API, bind]
keywords: Forguncy API, JavaScript API, bind
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 Bind Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-bind.html
folder: forguncy5_03_javascript_api
---

### Cell - Bind Method
Cell.bind (type, data, fn)
<br /><br />

### Bind Method 설명
선택한 특정 셀에 한 개 이상의 이벤트를 bind하고, 이벤트 발생 시 실행할 함수를 지정합니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| eventType | string | 예	| 셀 이벤트 유형을 표시하는 문자열입니다. <br />셀이 지원하는 이벤트의 종류는 [CellEvents()]()를 참고하세요. |
| data | any | 아니오	| 이 항목은 필수 입력사항은 아니며 선택적으로 사용하는 Parameter입니다. <br />값을 입력하지 않으면 무시되며, 값을 입력한 경우 Event Handler로 전달된 특정 Parameter를 표시합니다.|
| fn | function | 예 | Bind한 이벤트의 Event Handler입니다. |

<br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 cell.bind를 사용하는 예제입니다. 버튼 클릭 시 지정된 이벤트가 실행되도록 이벤트를 Binding 할 수 있습니다.
<br />

**예제1)**

~~~javascript
  //onClick 이벤트를 생성합니다. 입력한 문자열을 팝업으로 화면에 표시합니다.
  var onClick = function(arg) {
      alert("안녕하세요. Forguncy!");
  }

  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 button이라고 지정되어 있는 셀 인스턴스의 정보를 가져옵니다.
  var cell = page.getCell("button");

  //button 셀에 onClick 이벤트를 binding합니다.
  cell.bind("click", onClick);
~~~

**예제2)**

~~~javascript
  //변수를 선언하고, 선언한 변수를 이벤트로 전달하려 합니다.
  var text = "안녕하세요. Forguncy!!";

  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;

  //Cell Name이 button이라고 지정되어 있는 셀 인스턴스의 정보를 가져옵니다.
  var cell = page.getCell("button");

  //button 셀에 text라고 선언한 변수를 입력하고, 해당 이벤트의 실행은 변수를 화면에 표시하도록 합니다.
  cell.bind("click", text, function (arg) {
    alert(arg.data);
  });
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개를 생성하고, 버튼을 생성한 후 왼쪽 위 Cell Name에 button이라고 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-bind01.png)
    <br /><br />

2. 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-bind02.png)
    <br /><br />
    
3. 해당 프로젝트를 실행하고 버튼을 클릭하면 화면에 지정한 이벤트의 문자열이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-bind03.gif)

<br /><br />