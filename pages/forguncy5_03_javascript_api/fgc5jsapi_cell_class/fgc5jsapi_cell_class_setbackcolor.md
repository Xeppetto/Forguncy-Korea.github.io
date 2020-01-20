---
title: Forguncy API - Cell - setBackcolor
tags: [Forguncy, JavaScript, API, setBackcolor]
keywords: Forguncy API, JavaScript API, setBackcolor
last_updated: Jan 20, 2020
summary: "Forguncy API - Cell 클래스 중 setBackcolor Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-setbackcolor.html
folder: forguncy5_03_javascript_api
---

### Cell - setBackcolor Method
Cell.setBackcolor(color)
<br /><br />

### setBackcolor Method 설명
지정한 특정 셀의 배경 색상을 변경합니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| color | any | 예 | 색상을 설정합니다. 색상은 다음 세 가지 형식을 지원합니다. <br /><br />ㆍ색상 이름(red, blue, green 등)<br />ㆍ#fff000과 같은 16진수 색상 값<br />ㆍrgb(255, 0, 0)과 같은 rgb 코드 값 |

<br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 cell.setBackcolor를 사용하는 예제입니다. 지정한 특정 셀의 배경 색상을 변경합니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 myCell로 지정된 셀 인스턴스 정보를 가져옵니다.
  var cell = page.getCell("myCell");

  //셀의 배경 색상을 red로 지정합니다.
  var setColor = cell.setBackColor("red");
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. "텍스트 상자" 유형의 셀을 생성하고, 왼쪽위 Cell Name으로 myCell이라고 이름을 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setbackcolor01.png)
    <br /><br />

2. 페이지에 "버튼"을 하나 생성하고, 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setbackcolor02.png)
    <br /><br />

3. 해당 프로젝트를 실행하여 버튼을 클릭합니다. myCell 셀에 배경색이 더해집니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-setbackcolor03.gif)

<br /><br />
