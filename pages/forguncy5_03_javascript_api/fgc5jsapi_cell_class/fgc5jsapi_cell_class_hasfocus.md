---
title: Forguncy API - Cell - hasFocus
tags: [Forguncy, JavaScript, API, hasFocus]
keywords: Forguncy API, JavaScript API, hasFocus
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 hasFocus Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-hasfocus.html
folder: forguncy5_03_javascript_api
---

### Cell - hasFocus Method
cell.hasFocus()
<br /><br />

### hasFocus Method 설명
지정한 특정 셀에 포커스가 되어 있는 지 여부를 확인하고, 포커스 되도록 설정할 수 있습니다. 
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값

| 값 | 구분 | 의미 |
| --- | --- | --- |
| ture | boolean | 셀에 포커스가 되어 있음 |
| false | boolean | 셀에 포커스가 없음 |

<br />

### 활용 예제
아래는 cell.hasFocus를 사용하는 예제입니다. 지정한 특정 셀에 focus가 되어 있는 지 확인합니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 myCell로 지정된 셀 인스턴스의 속성을 가져옵니다.
  var cell = page.getCell("myCell");

  //myCell에 Focus가 되어 있는 지 확인합니다.
  var f = cell.hasFocus();

  //포커스 결과를 화면에 표시합니다.
  alert(f);
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. "텍스트 상자" 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 myCell이라고 이름을 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hasfocus01.png)
    <br /><br />

2. 페이지에 "버튼"을 하나 생성하고, 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hasfocus02.png)
    <br /><br />

3. 페이지에 "텍스트 상자"를 하나 생성하고, 해당 텍스트 상자 셀에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.<br />
    ※참고 : "텍스트 상자"에 입력한 명령은 사용자가 테스트 상자에 무언가를 입력하고나서 focus out되는 시점에 실행됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hasfocus03.png)
    <br /><br />

4. 해당 프로젝트를 실행합니다.<br />
    (1) 버튼을 클릭하면, 버튼에 focus가 오게 되므로 return되는 값은 false로 나타납니다.<br />
    (2) 다음은 두 번 째로 생성한 텍스트 상자에 아무 값이나 입력합니다. 이후 첫 번 째 텍스트 상자를 클릭하면, 두 번 째 텍스트 상자에 입력된 명령이 실행됩니다. 첫 번 째 상자를 클릭항여 focus 상태를 이동시켰으므로, focus는 첫 번 째 텍스트 상자에 있게 되고 return되는 값은 ture로 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hasfocus04.gif)

<br /><br />
