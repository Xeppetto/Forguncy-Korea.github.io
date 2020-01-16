---
title: Forguncy API - Cell - unbindAll
tags: [Forguncy, JavaScript, API, unbindAll]
keywords: Forguncy API, JavaScript API, unbindAll
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 unbindAll Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-unbindall.html
folder: forguncy5_03_javascript_api
---

### Cell - UnbindAll Method
cell.unbindAll을()
<br /><br />

### Unbind Method 설명
모든 셀에 지정된 이벤트들을 모두 unbind/해제하거나, 발생한 모든 이벤트를 종료시킬 수 있습니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 cell.unbindAll을 사용하는 예제입니다. cell.bind 메소드에서 사용한 예제를 unbind하여 작동하지 않도록 합니다.
<br />

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

  //모든 셀에 연결된 이벤트들을 모두 unbinding/해제합니다.
  cell.unbindAll();
~~~

<br />

### Forguncy 사용 예제

※참고 : unbind와 unbindall은 실제 사용하는 방법은 동일하며, 페이지 내 Event Handler의 수가 얼마나 많은 가에 따라 선택적으로 사용하실 수 있습니다. 이에 따라 같은 '사용 예제'를 사용합니다.

1. 페이지 한 개를 생성하고, 버튼을 생성한 후 왼쪽 위 Cell Name에 button이라고 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-bind01.png)
    <br /><br />

2. 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-bind02.png)
    <br /><br />
    
3. 해당 프로젝트를 실행하고 버튼을 클릭하면 화면에 지정한 이벤트의 문자열이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-bind03.gif)
    <br /><br />

4. 해당 버튼의 자바스크립트 명령에 unbind 코드를 추가합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-unbindall04.png)
    <br /><br />

5. 해당 프로젝트를 실행하고 버튼을 클릭해도 아무런 이벤트가 발생하지 않습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-unbind05.gif)

<br /><br />