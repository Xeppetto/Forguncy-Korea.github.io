---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Jan 8, 2020
summary: "Forguncy API - Page 클래스 중 getCellByLocation을 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getcellbylocation.html
folder: forguncy5_03_javascript_api
---

### Page - getCellByLocation Method
page.getCellByLocation(cellLocation)
<br /><br />

### getCellByLocation Method 설명
Cell의 위치 정보를 참조하여 Cell 인스턴스의 속성을 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| cellLocation | [CellLocationInfo]() | 예 | 특정 Cell의 위치 정보를 입력합니다. |

<br />

### Response 시 반환값
Cell 속성을 반환합니다. 자세한 내용은 Cell[]을 참고하세요.
<br /><br />

### 활용 예제
아래는 page.getCellByLocation을 사용하는 관련 사용 예제입니다. 다음 예제들을 응용하여 특정 Cell 인스턴스의 속성을 이용할 수 있습니다.
<br />

~~~javascript
  interface CellLocationInfo{
    //The row index of the cell, starting from 0
    Row: number;
    //Column index of the cell, starting from 0
    Column: number;
    //The page where the cell is located
    PageName: string;
  }
~~~

<br />

### Forguncy 사용 예제

1. Forguncy에서 빈 페이지 2개를 생성합니다. <br />
    "페이지1"에서 아래와 같이 셀 범위를 선택 > 셀 유형을 "내용이 포함된 셀 타입" 선택 > 하위 페이지로 "페이지2"를 지정합니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellarray02.png)]
    <br />
    ※ 참고 : "내용이 포함된 셀 타입"이라는 셀 유형은 아래와 같은 위치에 있습니다.<br />
    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellarray01.png)]
    <br />
2. "페이지2"로 이동하여 아래 그림과 같이 셀 영역을 설정합니다. <br />
    (1) 셀 유형은 '없음' 상태로 그냥 놔두시면 됩니다.<br />
    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellarray03.png)]
    <br />
    (2) 이후 좌측 상단에 "myCell"이라고 붙여 줍니다.<br />
    <br />
3. "페이지1"로 돌아가서 아래 그림과 같이 "버튼"을 생성하고, 버튼에 명령을 설정합니다.<br />
    (1) 셀 영역을 선택하신 후 셀 유형을 "버튼"으로 선택합니다.<br />
    <br />
    (2) 버튼 셀을 선택 시 우측에 나타나는 패널에 "명령 편집"으로 이동합니다.<br />
    <br />
    (3) "JavaScript로 직접 프로그래밍하기" 명령을 이용하여 스크립트를 작성합니다.<br />
    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellarray04.png)]
    <br />
4. 프로젝트를 실행합니다.

5. 웹브라우저에서 아래와 같이 '버튼'을 클릭하면, 1이라는 팝업창이 나타납니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellarray05.png)]

<br /><br />