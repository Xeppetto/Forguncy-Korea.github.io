---
title: Forguncy API - CellEvent - MouseEnter
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, MouseEnter, Web, JavaScript, API
last_updated: Jan 16, 2020
summary: "Forguncy API - CellEvent 클래스 중 MouseEnter Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cellevent-class-mouseenter.html
folder: forguncy5_03_javascript_api
---

### CellEvent - MouseEnter Method
CellEvents.mouseEnter
<br /><br />

### MouseEnter Method 설명
마우스 커서가 지정한 특정 셀로 들어오는 시점에 수행(trigger)되는 이벤트입니다. 버튼, 그림, 하이퍼링크 셀 유형을 지원합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string
<br /><br />

### 활용 예제
아래는 CellEvents.mouseEnter를 사용하는 예제입니다. 마우스가 지정한 그림 셀 위로 올라가면 글자 상자가 나타납니다.
<br />

~~~javascript
  //CallBack으로 사용할 이벤트를 정의합니다.
  var enteringMouseEvent = function(arg) {
      alert("안녕하세요. Forguncy!");
  }
  
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;

  //Cell Name이 picture라고 되어 있는 셀 인스턴스 속성을 가져옵니다.
  var cell = page.getCell("picture");

  //picture 셀에 enteringMouseEvent 이벤트를 binding합니다.
  cell.bind("mouseEnter", enteringMouseEvent);
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성하고, 이미지 셀을 생성하여 그림을 삽입합니다.<br />
  이후 왼쪽 상단의 Cell Name에 picture라고 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-mouseenter01.png)
    <br /><br />

2. 그림 셀을 클릭 후 '명령 편집'에서 "자바크스립트로 직접 프로그래밍하기" 명령을 추가하여, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-mouseenter02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 나타나는 그림에 마우스 커서를 올리면 팝업창이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-mouseenter03.gif)

<br /><br />
