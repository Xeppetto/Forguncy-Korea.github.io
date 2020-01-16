---
title: Forguncy API - Cell - enable
tags: [Forguncy, JavaScript, API, enable]
keywords: Forguncy API, JavaScript API, enable
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 enable Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-enable.html
folder: forguncy5_03_javascript_api
---

### Cell - Enable Method
cell.enable()
<br /><br />

### Enable Method 설명
특정 셀을 활성화합니다. 셀을 비활성화하시려면 비활성화(disable) 메소드를 사용하셔야 합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.enable을 사용하는 예제입니다. 버튼을 클릭하면 지정된 셀을 비활성화할 수 있습니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 "hyperlink"로 되어 있는 셀을 가져옵니다.
  var cell = page.getCell("hyperlink");

  //해당 Cell을 활성화합니다.
  cell.enable();
~~~

<br />

### Forguncy 사용 예제

※참고 : disable과 enable은 한 세트이므로 같은 예제가 구성되어 있습니다.

1. 페이지를 한 개 생성하고, 체크박스 셀을 하나 생성합니다. 이후 좌측상단의 Cell Name에 checkbox라고 입력해 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-disable01.png)
    <br /><br />

2. 버튼을 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-disable02.png)
    <br /><br />

3. 또 다른 버튼을 하나 추가로 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-disable03.png)
    <br /><br />

4. 해당 프로젝트를 실행하고 체크박스를 클릭할 수 있는 지 확인합니다.<br />
    Disable 버튼을 클릭하면 체크박스가 회색으로 변경되며, 클릭이 불가능하게 변경됩니다.<br />
    Enable 버튼을 클릭하면 체크박스가 다시 클릭 가능한 상태로 변경됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-disable04.gif)

<br /><br />