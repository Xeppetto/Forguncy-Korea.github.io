---
title: Forguncy API - Cell - setFocus
tags: [Forguncy, JavaScript, API, setFocus]
keywords: Forguncy API, JavaScript API, setFocus
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 setFocus Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-setfocus.html
folder: forguncy5_03_javascript_api
---

### Cell - setFocus Method
cell.setFocus()
<br /><br />

### setFocus Method 설명
지정한 특정 셀의 배경색을 설정합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 cell.setFocus를 사용하는 예제입니다. 지정한 특정 셀로 focus를 보내어 지정합니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 myCell로 지정된 셀 인스턴스의 속성을 가져옵니다.
  var cell = page.getCell("myCell");

  //myCell이 Focus되도록 설정합니다.
  cell.setFocus();
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. "텍스트 상자" 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 myCell이라고 이름을 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-hasfocus01.png)
    <br /><br />

2. 페이지에 "버튼"을 하나 생성하고, 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setfocus02.png)
    <br /><br />

3. 해당 프로젝트를 실행합니다. "텍스트 상자"와 "버튼"이 나타나며, 둘 중 어디에도 Focus는 없는 상태입니다.<br />
    버튼을 클릭하면 텍스트 상자에 Focus가 이동하며, 커서가 깜빡거리는 모습을 관찰할 수 있습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setfocus03.gif)

<br /><br />
