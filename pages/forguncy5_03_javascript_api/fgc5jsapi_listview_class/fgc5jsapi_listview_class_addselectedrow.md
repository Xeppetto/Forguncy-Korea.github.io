---
title: Forguncy API - ListView - addSelectedRow
tags: [Forguncy, JavaScript, API, addSelectedRow]
keywords: Forguncy API, JavaScript API, Click
last_updated: Feb 7, 2020
summary: "Forguncy API - ListView 클래스 중 addSelectedRow Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_listview-class-addselectedrow.html
folder: forguncy5_03_javascript_api
---

### ListView - addSelectedRow Method
listview.addSelectedRow(rowIndex)
<br /><br />

### addSelectedRow Method 설명
테이블의 특정 행을 선택합니다. ListView의 다중 선택을 활성화하는 경우 특정 행을 선택/해제할 수 있습니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| rowIndex | number | 예	| 0부터 시작하는 행의 인덱스 번호 |

<br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 listview.addSelectedRow를 사용하는 예제입니다. 버튼을 클릭하면 지정한 번호의 행이 ListView에서 선택/해제됩니다.
<br />

~~~javascript
    //현재 페이지에 Namespace를 선언합니다.
    var page = Forguncy.Page;
    
    //이름이 ListView1인 ListView를 가져옵니다.
    var listview = page.getListView("ListView1");

    //ListView의 2번째 행(Row)을 선택합니다.
    listview.addSelectedRow(2);
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. 데이터베이스 테이블을 한 개 생성한 후, 이름/생년월일/부서 열을 생성합니다.<br />
  데이터는 넣어도 되고 안 넣어도 됩니다. 본 예제에서는 알아보기 쉽게 하기 위해 가짜 데이터를 입력했습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow01.png)
    <br /><br />

2. 화면의 영역을 선택하고 "ListView로 설정" 기능을 이용하여, ListView를 생성합니다.<br />
  이 때, 데이터베이스를 선택하라고 나타나는데, 위에서 생성한 테이블을 선택하시면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow02.png)
    <br /><br />

3. 생성한 ListView의 제일 왼쪽 셀을 클릭 한 뒤, "디자인 탭 > 선택한 열" 옵션을 클릭합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addselectedrow05.png)
    <br /><br />

4. ListView에 데이터를 쉽게 입력하는 방법은 아래와 같습니다. 테이블의 열-이름을 드래그하면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addselectedrow06.gif)
    <br /><br />

5. 버튼을 한 개 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 이용하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addselectedrow07.png)
    <br /><br />

6. 프로젝트를 생성합니다. 버튼을 클릭하면 ListView의 세 번 째 줄의 체크 박스가 선택됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addselectedrow08.gif)
    <br /><br />

7. 참고 : ListView의 Index는 0에서부터 시작합니다. 첫 번 째 데이터부터 0, 1, 2, 3, ... 순으로 늘어납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addselectedrow09.png)

<br /><br />
