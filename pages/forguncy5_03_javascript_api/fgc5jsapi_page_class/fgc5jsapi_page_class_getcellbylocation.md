---
title: Forguncy JavaScript API - Page - getCellByLocation
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, getCellByLocation, Web, JavaScript, API
last_updated: Jan 8, 2020
summary: "Forguncy JavaScript API - Page 클래스 중 getCellByLocation Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getcellbylocation.html
folder: forguncy5_03_javascript_api
---

### Page - getCellByLocation Method
Page.getCellByLocation(cellLocation)
<br /><br />

### getCellByLocation Method 설명
Forguncy의 좌표값을 기반으로 Cell의 위치 정보를 참조하여 Cell 인스턴스의 속성을 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| cellLocation | [CellLocationInfo]() | 예 | 특정 Cell의 위치 정보를 입력합니다. |

> 😄 CellLocationInfo 관련 내용은 준비 중입니다.

CellLocationInfo 인터페이스 타입은 아래와 같이 정의되어 있습니다.

~~~javascript
  interface CellLocationInfo{
    //0부터 해당 Cell의 Row 위치까지의 index값
    Row: number;

    //0부터 해당 Cell의 Column 위치까지의 index값
    Column: number;

    //해당 Cell이 위치한 특정 페이지의 이름
    PageName: string;
  }
~~~

<br />

### Response 시 반환값
Cell 속성을 반환합니다. 자세한 내용은 Cell[]을 참고하세요.

> 😄 Cell Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 page.getCellByLocation을 사용하는 관련 사용 예제입니다. 특정 Cell의 위치 정보를 이용해 해당 Cell의 배경색을 설정합니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;

  //'페이지1' 내에서 Row 2, Column 3 위치에 있는 Cell을 지정합니다.
  var cell = page.getCellByLocation({
    Row: 2,
    Column: 3,
    PageName: "페이지1"
  });
  
  //지정한 해당 Cell의 배경색상을 빨간색으로 설정합니다.
  var setColor = cell.setBackColor("red");
~~~

<br />

### Forguncy 사용 예제

1. 아래 그림 과 같이 Forguncy에서 페이지를 생성하고, 셀의 위치를 알아볼 수 있게 아무 내용이나 입력합니다.

2. 버튼을 생성하고, 해당 바튼의 "명령 편집"을 실행하여, "자바스크립트로 직접 프로그래밍하기" 명령을 생성합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellbylocation01.png)
    <br /><br />
    
3. 해당 프로젝트를 실행한 후, 버튼을 클릭하면 아래와 같이 Row 2, Column 3 위치에 배경색상이 변경됩니다.
    
    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellbylocation02.gif)
    <br /><br />

4. Forguncy에서는 A Column을 0, 1 Row를 0으로 Index 값을 가지며, 이를 기준으로 Cell의 위치를 계산합니다.<br />
    그러므로 A1는 Index(0, 0), B2는 Index (1, 1)이 되는 방식입니다. 그러므로 Column 3, Row 2는 D3가 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellbylocation03.png)

<br /><br />