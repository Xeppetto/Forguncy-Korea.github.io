---
title: Forguncy API - Page - reloadBindingData
tags: [Forguncy, JavaScript, API, reloadBindingData]
keywords: Forguncy API, JavaScript API, reloadBindingData
last_updated: Jan 13, 2020
summary: "Forguncy API - Page 클래스 중 reloadBindingData Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-reloadbindingdata.html
folder: forguncy5_03_javascript_api
---

### Page - reloadBindingData Method
page.reloadBindingData(tableName)
<br /><br />

### reloadBindingData Method 설명
현재 페이지에 사용 중인 Database의 Table들과 View들을 다시 불러오기합니다.<br />
ListView의 설정에서 "자동으로 데이터 다시 불러오기"를 설정하셔도 같은 방식으로 작동합니다. <br />
혹은 reloadBindingData Method를 직접 사용하여 데이터베이스를 다시 불러올 수 있습니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| tableName | string | 예 | 다시 로딩해서 불러올 데이터베이스의 테이블 이름을 입력합니다. |

<br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.reloadBindingData를 사용하는 관련 사용 예제입니다. 지정된 테이블을 다시 불러옵니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //데이터베이스에서 데이터를 다시 불러옵니다.
  page.reloadBindingData("테이블이름");
~~~

<br />

### Forguncy 사용 예제

1. 이번 예제에서는 페이지를 생성하기 전에 데이터베이스 테이블을 한 개 생성합니다.<br />
    내용은 대충 만들어 보고 싶으셨던 대로 넣으시면 됩니다. 최소 1개의 Column은 생성하셔야 합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-reloadbindingdata01.png)
    <br /><br />

2.  페이지를 한 개 생성하고 ListView를 생성합니다. ListView에 위에서 생성한 테이블의 Column을 연결합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-reloadbindingdata02.png)
    <br /><br />

3. 버튼을 추가합니다. '명령 편집'으로 '자바스크립트로 직접 프로그래밍하기'하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-reloadbindingdata03.png)
    <br /><br />

4. 해당 프로젝트를 실행합니다. 화면에는 아래와 같이 ListView에 연결된 Database 테이블의 내용이 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-reloadbindingdata04.png)
    <br /><br />

5. Forguncy 에디어로 돌아가서 데이터베이스 테이블에 아무 내용이나 입력합니다.<br />
    데이터베이스 테이블의 내용을 변경하신 후 CTRL+S 혹은 저장하여 프로젝트를 저장합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-reloadbindingdata05.png)
    <br /><br />

6. 다시 웹브라우저로 돌아가서 버튼을 클릭하면 아래와 같이 프로젝트의 데이터 테이블에 수정 후 저장한 내용이 웹브라우저에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-reloadbindingdata06.png)

<br /><br />