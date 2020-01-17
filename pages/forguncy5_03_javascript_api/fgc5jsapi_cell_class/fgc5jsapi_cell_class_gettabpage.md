---
title: Forguncy API - Cell - getTabPage
tags: [Forguncy, JavaScript, API, getTabPage]
keywords: Forguncy API, JavaScript API, getTabPage
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 getTabPage Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-gettabpage.html
folder: forguncy5_03_javascript_api
---

### Cell - getTabPage Method
cell.getTabPage()
<br /><br />

### getTabPage Method 설명
"페이지 내 탭 컨트롤 셀" 유형을 사용하여, 지정한 탭의 하위 페이지 객체 정보를 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| tabIndex | number | 예	| 탭의 index 번호를 입력합니다. 탭의 index는 0부터 시작합니다. |

<br />

### Response 시 반환값
없음
<br /><br />

### 활용 예제
아래는 cell.getTabPage를 사용하는 예제입니다. 페이지의 탭컨트롤 내부 특정 탭에 포함된 하위 페이지 객체 정보를 가져와 화면에 보여줍니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 tabControl로 되어 있는 셀 인스턴스의 정보를 가져옵니다.
  var tabControlCell = page.getCell("tabControl");

  //tabControl 셀에서 index가 0인 하위 페이지의 객체 정보를 불러옵니다.
  var tab1 = tabControlCell.getTabPage(0);

  //하위 페이지 내에서 Cell Name이 myCell인 셀 인스턴스의 정보를 가져옵니다.
  var subPageCell = tab1.getCell("myCell");

  //가져온 셀의 값을 화면에 표시합니다.
  alert(subPageCell.getValue());
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 두 개 생성합니다. 첫 번 째 페이지에는 "페이지 내 탭 컨트롤 셀"을 선택합니다.<br />
    화면 왼쪽 상단의 Cell Name에 tabControl이라고 이름을 붙여줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-gettabpage01.png)
    <br /><br />

2. 두 번 째 페이지에는 아무 컨텐츠나 컨텐츠를 넣어 줍니다. 예제에서는 화면 내 결과 출력을 위해 텍스트를 입력했습니다. <br />
    이후 페이지 왼쪽 위에 해당 Cell Name을 myCell이라고 적어줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getcontainerpage02.png)
    <br /><br />

3. 페이지 내에 버튼을 한 개 추가하고, 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-gettabcount03.png)
    <br /><br />
    
4. 해당 프로젝트를 실행하고 탭을 이동하면서 버튼을 클릭하면 지정한 Tab Index 탭의 특정 셀 내용이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-gettabcount04.gif)

<br /><br />
