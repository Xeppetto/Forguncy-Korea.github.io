---
title: Forguncy API - ListView - addNewRow
tags: [Forguncy, JavaScript, API, addNewRow]
keywords: Forguncy API, JavaScript API, Click
last_updated: Feb 7, 2020
summary: "Forguncy API - ListView 클래스 중 addNewRow Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_listview-class-addnewrow.html
folder: forguncy5_03_javascript_api
---

### ListView - addNewRow Method
listview.addNewRow
<br /><br />

### addNewRow Method 설명
새로운 행(Row)를 추가합니다. 내용을 포함하여 추가할 수도 있습니댜.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| rowValues | plain Object 또는 [] | 예	| 새로운 데이터 행(Row) |
| isText | boolean | 아니오	| rowValue Paramter를 텍스트로 분석해야 하는 지 여부를 정합니다. 아무 것도 입력하지 않은 경우 기본 값은 fasle입니다. |

<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 listview.addNewRow를 사용하는 예제입니다. 버튼을 클릭하면 미리 지정한 글자 상자가 나타납니다.
<br />

~~~javascript
    //현재 페이지에 Namespace를 선언합니다.
    var page = Forguncy.Page;
    
    //Cell Name이 button이라고 지정된 셀을 가져옵니다.
    var listview = page.getListView("listview1");

    //button 셀에 onClickEventFunction를 click할 때 이벤트가 발생하도록 binding합니다.
    listview.addNewRow (
    {
      "이름" : "이 설",
      "생년월일" : new Date(2012, 2, 7),
      "부서" : "마케팅"
    });
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. "버튼" 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 buitton이라고 이름을 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-click01.png)
    <br /><br />

2. 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-click02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 버튼을 클릭합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-click03.gif)
    <br /><br />

    ※참고 : bind 메소드로 이벤트를 바인딩 하는 경우 binding하는 시점에는 아무 이벤트가 발생하지 않는 것처럼 보여 두 번 클릭하는 것처럼 보일 수 있습니다. 이는 첫 번 째 클릭 시에는 cell.bind가 실행되어 CallBack 함수인 onClickEventFunction 함수가 버튼에 바인딩되는 이벤트가 실행되기 때문에 실제 눈에 보이지 않아서 그렇습니다. CallBack 함수를 Binding하는 경우는 이벤트를 바인딩하는 시점에 한 스텝이 더 진행됩니다. ([Jquery - bind 메소드 참조](https://www.w3schools.com/jquery/event_bind.asp))

<br /><br />
