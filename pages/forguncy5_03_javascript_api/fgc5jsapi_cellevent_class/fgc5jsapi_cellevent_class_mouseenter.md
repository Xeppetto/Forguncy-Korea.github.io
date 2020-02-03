---
title: Forguncy API - CellEvent - MouseEnter
tags: [Forguncy, JavaScript, API, MouseEnter]
keywords: Forguncy API, JavaScript API, MouseEnter
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
아래는 CellEvents.PivotTableClick를 사용하는 예제입니다. 버튼을 클릭하면 미리 지정한 글자 상자가 나타납니다.
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

1. 페이지 한 개 생성하고, ListView를 생성하여 Database Table에 연결합니다.<br />
    Database에 Table을 생성하고 데이터를 넣는 방법과 ListView를 생성하는 방법 등은 자세한 설명을 생략합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-pivottableclick01.png)
    <br /><br />

2. 페이지에 "피벗 테이블" 셀 유형을 추가합니다. 왼쪽위의 Cell Name에 pitvottablecell이라고 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-pivottableclick02.png)
    <br /><br />

3. 오른쪽 '셀 유형' 패널에서 "피벗 테이블 설정"을 선택하여 피벗 테이블을 미리 설정한 ListView와 연동합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-pivottableclick03.png)
    <br /><br />

4. JS 파일을 생성하고, 오른쪽 패널에서 "페이지 설정 > 사용자 JavaScript"에 해당 JavaScript 파일을 불러오기 합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-pivottableclick04.png)
    <br /><br />

5. 해당 프로젝트를 실행하여 피벗 테이블을 클릭하면, 팝업창이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cellevent-pivottableclick05.gif)

<br /><br />
