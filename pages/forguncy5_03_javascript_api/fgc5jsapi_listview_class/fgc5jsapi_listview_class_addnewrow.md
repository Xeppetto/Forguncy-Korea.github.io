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
    
    //이름이 ListView1인 ListView를 가져옵니다.
    var listview = page.getListView("ListView1");

    //가져온 ListView에 이름, 생년월일, 부서 데이터를 입력합니다.
    listview.addNewRow (
    {
      "이름" : "이설",
      "생년월일" : new Date(2012, 2, 7),
      "부서" : "마케팅"
    });
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

3. ListView에 데티어를 쉽게 입력하는 방법은 아래와 같습니다. 테이블의 열-이름을 드래그하면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow03.gif)
    <br /><br />

4. ListView의 이름을 설정합니다. ListView의 이름은 클릭 시 오른쪽의 '셀 유형' 탭에서 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow04.png)
    <br /><br />

5. ListView 내부의 각 열-이름을 설정합니다. ListView의 2번 째 줄에 열 이름을 정할 수 있습니다.<br />
  이렇게 설정해야 ListView라는 형식의 control을 웹에서 사용할 수 있습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow05.png)
    <br /><br />

6. 버튼을 한 개 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 이용하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow06.png)
    <br /><br />

7. 프로젝트를 생성합니다. 버튼을 클릭하면 ListView에 데이터가 입력됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-addnewrow07.gif)

<br /><br />
