---
title: Forguncy API - Page - setCurrentRow
tags: [Forguncy, JavaScript, API, setCurrentRow]
keywords: Forguncy API, JavaScript API, setCurrentRow
last_updated: Jan 14, 2020
summary: "Forguncy API - Page 클래스 중 setCurrentRow Method에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-setcurrentrow.html
folder: forguncy5_03_javascript_api
---

### Page - setCurrentRow Method
page.setCurrentRow(currentRowParam) 혹은 page.setCurrentRow(currentRowInfoPluginParam)
<br /><br />

### setCurrentRow Method 설명
Database 특정 값이 들어 있는 행을 지정합니다. 예를 들어, 어떤 데이터가 어떤 테이블의 3번째 행에 들어 있다면, 그 3번째 행의 모든 내용들이 화면의 페이지에 표시될 수 있도록 Database Table의 특정 행을 선택합니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| currentRowParam | function | 예 | 웹 개발 시 사용하며, 데이터 테이블의 현재 선택된 행(Row) 라인 값을 참조합니다. |
| currentRowInfoPluginParam | function | 예 | 플러그인 개발 시 사용하며, 데이터 테이블의 현재 선택된 행(Row) 라인 값을 참조합니다. |


### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.setCurrentRow를 사용하는 관련 사용 예제입니다. 

**JavaScript 예)** 데이터 테이블의 특정 조건을 검색 및 이용하여, 테이블의 특정 라인을 선택합니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //데이터 테이블의 현재 행(Row)을 선택합니다.
  page.setCurrentRow(
  {
    //'직원테이블'을 선택합니다.
    TableName: "직원테이블",

    //PrimaryKey로 ID가 2인 행을 찾습니다.
    PrimaryKey: {
      ID: 2
    }
  });
~~~

**C# 예)** Forguncy Plugin을 만들 때 사용할 코드 예제입니다.

~~~c#
  SetCurrentRowCommand.prototype.execute = function () {
    
    //Forguncy로 생성한 페이지에서 setCurrentRow를 선언합니다.
    Forguncy.Page.setCurrentRow({

      //QueryCondition 클래스에서 현재 행의 정보를 참조하게 합니다.
      QueryCondition: this.CommandParam.CurrentRowInfo,
      FormulaCalcContext: this.getFormulaCalcContext()
    });
  }
~~~

<br />

### Forguncy 사용 예제

1. 데이터베이스 테이블을 한 개 생성하고, 테이블 내에 레코드 값을 최소 3개 이상 작성합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-setcurrentrow01.png)
    <br /><br />

2. 페이지를 한 개 생성하고, 아래와 같이 데이터 테이블의 Column을 매핑시켜 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-setcurrentrow02.png)
    <br /><br />
    ※참고 : 데이터 테이블의 컬럼을 화면에 매핑시키는 방법은 아래 그림처럼 끌어다놓기(Drag & Drop) 하시면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-setcurrentrow03.gif)
    <br /><br />

3. 버튼을 한 개 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 이용하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-setcurrentrow04.png)
    <br /><br />

4. 해당 프로젝트를 실행하면 빈 화면이 나타납니다. 버튼을 입력하면 코드에 입력된 대로 Primary Key인 ID가 2인 정보가 화면에 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-setcurrentrow05.png)

<br /><br />