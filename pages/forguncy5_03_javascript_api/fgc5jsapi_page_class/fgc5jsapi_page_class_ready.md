---
title: Forguncy API - Page - ready
tags: [Forguncy, JavaScript, API, ready]
keywords: Forguncy API, JavaScript API, ready
last_updated: Jan 13, 2020
summary: "Forguncy API - Page 클래스 중 ready Method와 관련해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-ready.html
folder: forguncy5_03_javascript_api
---

### Page - ready Method
page.ready(fn)
<br /><br />

### ready Method 설명
페이지 로딩이 완료된 후 Ready 메소드에 정의한 Callback 함수가 호출됩니다.<br />페이지 내 기능 로직을 처리하는 방법으로 페이지 내의 모든 요소들이 작동 준비되었을 때 Callback으로 처리하는 방식을 추천합니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| fn | function | 예 | 페이지의 로딩이 완료되어 사용 준비되면 호출되는 Callback 함수명입니다. |

<br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.ready를 사용하는 관련 사용 예제입니다. 사용 중인 사용자의 이름을 보여줍니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //ready Method의 Callback 함수에 아래 로직을 추가합니다.
  page.ready(function () {
    
    //"button"이라는 이름의 Cell에 "Click" 이벤트를 binding합니다.
    page.getCell("button").bind("click", function () {
      
      //현재 사용 중인 사용자의 이름을 팝업으로 표시합니다.
      alert(page.getUserName());
    })
  });
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀 범위를 선택하여 "현재 사용자" 셀 유형을 추가합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-ready01.png)
    <br /><br />

2. 버튼을 추가합니다. (✅중요) 이 때, 화면 좌측 상단에 Forguncy Cell Name을 'button'으로 지정해 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-ready02.png)
    <br /><br />

3. ready Method는 페이지의 실행 시점(OnLoad 시점)에 실행되는 스크립트이므로, 외부 파일로 만들어 해당 페이지에 연결해 줍니다.<br />
    아래 그림은 Notepad++로 스크립트를 작성 > 저장 > Forguncy에 가져오기 한 예제입니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-ready03.png)
    <br /><br />

4. 해당 프로젝트를 실행하여 버튼을 클릭하면 아래와 같이 현재 사용자의 이름이 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-ready04.gif)

<br /><br />