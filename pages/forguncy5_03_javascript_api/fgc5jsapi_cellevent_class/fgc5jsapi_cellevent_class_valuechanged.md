---
title: Forguncy API - CellEvent - ValueChanged
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, ValueChanged, Web, JavaScript, API
last_updated: Jan 16, 2020
summary: "Forguncy API - CellEvent 클래스 중 ValueChanged Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cellevent-class-valuechanged.html
folder: forguncy5_03_javascript_api
---

### CellEvent - ValueChanged Method
CellEvents.valueChanged
<br /><br />

### ValueChanged Method 설명
지정한 특정 셀의 입력 값이 변경되는 시점에 수행(trigger)되는 이벤트입니다. 입력 상자, 여러 줄 입력 상자 등 입력하는 형식의 셀 유형을 지원합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string
<br /><br />

### 활용 예제
아래는 CellEvents.valueChanged 사용하는 예제입니다. 입력 상자에 글자를 입력하면 글자 상자가 나타납니다.
<br />

~~~javascript
  //CallBack으로 사용할 이벤트를 정의합니다.
  var valueChangedEvent  = function(arg) {
      alert("안녕하세요. Forguncy!");
  }
  
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;

  //Cell Name이 myCell이라고 되어 있는 셀 인스턴스 속성을 가져옵니다.
  var cell = page.getCell("myCell");

  //input 셀이 변경될 때 valueChangedEvent 이벤트를 binding합니다.
  cell.bind("valueChanged", valueChangedEvent);
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성하고, 텍스트 상자 셀을 생성합니다. 이후 왼쪽 상단의 Cell Name에 myCell이라고 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-valuechanged01.png)
    <br /><br />

2. 텍스트 상자 셀을 클릭 후 '명령 편집'에서 "자바크스립트로 직접 프로그래밍하기" 명령을 추가하여, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-valuechanged02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 나타나는 텍스트 상자에 값을 입력 후 엔터키를 누릅니다. 이후 값을 변경한 후 다시 엔터키를 누르면 경고창이 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-valuechanged03.gif)

    이벤트가 중첩되어 실행되는 것은 JavaScript 라이브러리의 이슈입니다. 실제 구현하실 때는 이를 고려하셔서 구현해 주세요.
    
<br /><br />
