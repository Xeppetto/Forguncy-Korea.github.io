---
title: Forguncy JavaScript API - Page - getCell
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, getCell, Web, JavaScript, API
last_updated: Jan 9, 2020
summary: "Forguncy JavaScript API - Page 클래스 중 getCell Method에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getcell.html
folder: forguncy5_03_javascript_api
---

### Page - getCell Method
Page.getCell(name, includeSubPage)
<br /><br />

### getCell Method 설명
개별 Cell Name을 기반으로 Cell 인스턴스의 속성을 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| name | string | 예 | 특정 Cell에 부여된 Cell Name을 입력합니다. |
| includeSubPage | boolean | 아니오 | 페이지 내 하위 페이지를 포함하는 컨테이너 또는 탭컨트롤이 존재하는 경우 하위 페이지까지 검색할 지 여부를 결정합니다. <br />기본값은 True이며 의미는 "검색함"입니다. False는 "검색하지 않음"입니다. |

<br />

### Response 시 반환값
Cell 속성을 반환합니다. 자세한 내용은 Cell[]을 참고하세요.

> 😄 Cell Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 page.getCell을 사용하는 관련 사용 예제입니다. 특정 Cell의 Cell Name으로 페이지를 검색하여 해당 Cell을 선택하고, 원하는 단어를 입력합니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;

  //페이지 내에서 myCell이라는 Cell Name을 가진 Cell을 불러옵니다.
  var cell = page.getCell("myCell");
  
  //myCell이라는 Cell Name을 가진 Cell에 Forguncy라고 입력합니다.
  cell.setValue("Forguncy");
~~~

<br />

### Forguncy 사용 예제

1. Forguncy에서 페이지 2개를 생성합니다. 

2. "페이지1"에 셀 범위를 선택한 후 병합합니다. "페이지 2"에도 셀 범위를 선택한 후 병합합니다.

3. "페이지1"의 셀에는 myCell1, "페이지2"의 셀에는 myCell2라고 입력합니다. 화면 좌측 위에 입력하시면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcell01.png)
    <br /><br />
    
4. "페이지1"에서 아래와 같이 셀 범위를 선택 > 셀 유형을 "내용이 포함된 셀 타입" 선택 > 하위 페이지로 "페이지2"를 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcell03.png)
    <br /><br />

    ※ 참고 : "내용이 포함된 셀 타입"이라는 셀 유형은 아래와 같은 위치에 있습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcellarray01.png)
    <br /><br />

5. "페이지1"에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcell02.png)
    <br /><br />

6. 해당 프로젝트를 실행하고, 버튼을 누르면 myCell1과 myCell2에 각각 Forguncy1, Forguncy2라고 입력됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcell04.gif)

<br /><br />