---
title: Forguncy API - CellEvent - Click
tags: [Forguncy, JavaScript, API, Click]
keywords: Forguncy API, JavaScript API, Click
last_updated: Jan 16, 2020
summary: "Forguncy API - CellEvent 클래스 중 Click Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cellevent-class-click.html
folder: forguncy5_03_javascript_api
---

### CellEvent - Click Method
CellEvents.Click
<br /><br />

### Click Method 설명
셀을 클릭하는 시점에 수행(trigger)되는 클릭 이벤트를 발생시킵니다. 버튼, 그림, 하이퍼링크 셀 유형을 지원합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
string
<br /><br />

### 활용 예제
아래는 cell.Click를 사용하는 예제입니다. 버튼을 클릭하면 미리 지정한 글자 상자가 나타납니다.
<br />

~~~javascript
    //클릭 시 실행한 binding 함수를 정의합니다.
    var onClickEventFunction = function(arg) {

        //화면에 표시할 문구를 정의합니다.
        alert("안녕하세요. Forguncy!");
    }

    //현재 페이지에 Namespace를 선언합니다.
    var page = Forguncy.Page;
    
    //Cell Name이 button이라고 지정된 셀을 가져옵니다.
    var cell = page.getCell("button");

    //button 셀에 onClickEventFunction를 click할 때 이벤트가 발생하도록 binding합니다.
    cell.bind("click", onClickEventFunction);
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. "버튼" 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 buitton이라고 이름을 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-click01.png)
    <br /><br />

2. 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-click02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 버튼을 클릭합니다.<br />
    ※참고 : bind 메소드로 이벤트를 바인딩 하는 경우 binding하는 시점에는 아무 이벤트가 발생하지 않는 것처럼 보여 두 번 클릭하는 것처럼 보일 수 있습니다. 이는 첫 번 째 클릭 시에는 cell.bind가 실행되어 CallBack 함수인 onClickEventFunction 함수가 버튼에 바인딩되는 이벤트가 실행되기 때문에 실제 눈에 보이지 않아서 그렇습니다. CallBack 함수를 Binding하는 경우는 이벤트를 바인딩하는 시점에 한 스텝이 더 진행됩니다. ([Jquery - bind 메소드 참조](https://www.w3schools.com/jquery/event_bind.asp))

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-click03.gif)

<br /><br />
