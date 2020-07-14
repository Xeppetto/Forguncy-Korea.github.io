---
title: Forguncy API - Cell - getActiveTabIndex
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, getActiveTabIndex, Web, JavaScript, API
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 getActiveTabIndex Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-getactivetabindex.html
folder: forguncy5_03_javascript_api
---

### Cell - getActiveTabIndex Method
Cell.getActiveTabIndex()
<br /><br />

### getActiveTabIndex Method 설명
"페이지 내 탭 컨트롤 셀" 유형을 사용할 때, 활성화된 탭의 index 번호를 가져옵니다. 
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 cell.getactivetabindex를 사용하는 예제입니다. 활성화된 탭의 인덱스를 보여줍니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //탭페이지 유형의 셀 인스턴스 정보를 가져옵니다.
  var tabControlCell = page.getCell("tabControl");

  //현재 활성화된 탭의 index 번호를 불러옵니다. index는 0부터 시작합니다.
  var activeTabIndex = tabControlCell.getActiveTabIndex();

  //현재 활성화된 탭의 index 번호를 화면에 표시합니다.
  alert(activeTabIndex);
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 여러 개 생성합니다. 예제에서는 총 5개의 페이지를 생성했습니다.<br />
    '페이지2 ~ 페이지5'까지는 그림이나 텍스트 등 컨텐츠를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getactivetabindex01.png)
    <br /><br />

2. '페이지1'에 "페이지 내 탭 컨트롤 셀" 유형의 셀을 생성합니다. <br />
    오른쪽 '셀 유형'에 "탭"을 '페이지2 ~ 페이지5'까지 나타나도록 지정합니다.<br />
    이후 페이지 왼쪽 위에 해당 Cell Name을 tabControl이라고 적어줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getactivetabindex02.png)
    <br /><br />

3. 페이지 내에 버튼을 한 개 추가하고, 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getactivetabindex03.png)
    <br /><br />
    
4. 해당 프로젝트를 실행하고 탭을 이동하면서 버튼을 클릭하면 화면에 활성화되어 있는 탭의 Tab Index 번호가 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getactivetabindex04.gif)

<br /><br />
