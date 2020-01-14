---
title: Forguncy API - Page - setCurrentRow
tags: [Forguncy, JavaScript, API, setCurrentRow]
keywords: Forguncy API, JavaScript API, setCurrentRow
last_updated: Jan 14, 2020
summary: "Forguncy API - Page 클래스 중 setCurrentRow에 대해 설명합니다."
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

예 - JavaScript) 데이터 테이블의 특정 조건을 검색 및 이용하여, 테이블의 특정 라인을 선택합니다.
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

예 - C#) Forguncy Plugin을 만들 때 사용할 코드 예제입니다.

~~~C#
  SetCurrentRowCommand.prototype.execute = function () {
    
    //Forguncy로 생성한 페이지에서 setCurrentRow를 선언합니다.
    Forguncy.Page.setCurrentRow({

      //QueryCondition 클래스에서 현재 행의 정보를 참조하게 합니다.
      QueryCondition: this.CommandParam.CurrentRowInfo,
      FormulaCalcContext: this.getFormulaCalcContext()
    });
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 셀 영역을 선택하여 "텍스트 상자"를 생성합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc01.png)]
    <br /><br />

2. 텍스트 상자 아래 쪽에 병합 셀을 하나 생성하고, 위에서 생성한 텍스트 상자를 참조하도록 합니다. (화면에서 =B2로 표현되어 있습니다.)

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc02.png)]
    <br /><br />

3. 해당 프로젝트를 실행하면 입력 박스 하나와 숫자 0이 나타납니다. 해당 입력 박스에 아무거나 입력 후 Enter키를 누르면 숫자 0은 입력한 대로 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc03.png)]
    <br /><br />

4. Forguncy Editor로 돌아가 버튼을 한 개 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 생성하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc04.png)]
    <br /><br />

5. 다시 해당 프로젝트를 실행한 후 "버튼"을 클릭합니다. 이후 입력 창에 아무거나 입력 후 Enter키를 눌러 봅니다. 값이 변경되지 않으면 suspendCalc가 잘 적용된 것입니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc05.png)]
    <br /><br />

6. 다시 Forguncy Editor로 돌아가 버튼을 한 개 더 생성하고, 명령을 생성하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc06.png)]
    <br /><br />

7. 다시 한 번 해당 프로젝트를 생성하고, 다음의 방법으로 테스트를 진행합니다.<br />
    (1) suspendCalc를 적용한 버튼을 클릭합니다.<br />
    (2) 입력 상자에 아무거나 입력 후 Enter키를 누릅니다. ▶ 값이 변하지 않으면 성공입니다.<br />
    (3) resumeCalc를 적용한 버튼을 클릭합니다.<br />
    (4) 입력 상자에 아무거나 입력 후 Enter키를 누릅니다. ▶ 값이 입력한 대로 변하면 성공입니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-resumecalc07.png)]
    <br /><br />

<br /><br />