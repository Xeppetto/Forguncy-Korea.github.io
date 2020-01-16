---
title: Forguncy API - Cell - setValue
tags: [Forguncy, JavaScript, API, setValue]
keywords: Forguncy API, JavaScript API, setValue
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 setValue Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-setvalue.html
folder: forguncy5_03_javascript_api
---

### Cell - setValue Method
cell.setValue(value)
<br /><br />

### setValue Method 설명
지정한 특정 셀에 지정한 값을 입력합니다. 값은 임의의 값일 수 있으며, 웹에서 표현할 수 있는 형식이라면 제한이 없습니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| value | any | 예 | 웹에서 표현할 수 있는 값을 아무거나 입력합니다. |

<br />

### Response 시 반환값
아무거나, any
<br /><br />

### 활용 예제
아래는 cell.setValue를 사용하는 예제입니다. 지정한 특정 셀에 값을 입력합니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 myCell인 셀 인스턴스 정보를 가져옵니다.
  var textCell = page.getCell("myCell");

  //해당 Cell에 값을 설정합니다.
  textCell.setValue("안녕하세요. Forguncy!!");
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, 빈 셀에 하나를 생성합니다. 이후 좌측상단의 Cell Name에 myCell이라고 입력해 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setvalue01.png)
    <br /><br />

2. 버튼을 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setvalue02.png)
    <br /><br />

3. 해당 프로젝트를 실행하고, 버튼을 클릭하면 myCell에 입력된 값(value)가 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setvalue03.gif)

<br /><br />