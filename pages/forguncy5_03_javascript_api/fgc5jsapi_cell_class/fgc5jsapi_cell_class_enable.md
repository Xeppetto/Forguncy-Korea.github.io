---
title: Forguncy API - Cell - enable
tags: [Forguncy, JavaScript, API, enable]
keywords: Forguncy API, JavaScript API, enable
last_updated: Jan 14, 2020
summary: "Forguncy API - Cell 클래스 중 enable Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-enable.html
folder: forguncy5_03_javascript_api
---

### Page - Enable Method
page.enable()
<br /><br />

### Enable Method 설명
특정 셀을 활성화합니다. 셀을 비활성화하시려면 비활성화(disable) 메소드를 사용하셔야 합니다.
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.enable을 사용하는 예제입니다. 버튼을 클릭하면 지정된 셀을 비활성화할 수 있습니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 "hyperlink"로 되어 있는 셀을 가져옵니다.
  var cell = page.getCell("hyperlink");

  //해당 Cell을 활성화합니다.
  cell.enable();
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하고, "하이퍼링크" 셀을 하나 생성합니다. 이후 좌측상단의 Cell Name에 'hyperlink'라고 입력해 줍니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_cell-enable01.png)
    <br /><br />

2. 하이퍼링크 셀을 선택하고 오른쪽 '셀 유형' 탭을 선택하고 "기타 > 비활성화하기"를 선택합니다.<br />
    이렇게 선택하면 해당 셀은 웹페이지 시작 시 비활성화된 상태로 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-enable02.png)
    <br /><br />

3. 버튼을 생성하여 아래와 같이 "자바스크립트로 직접 프로그래밍하기" 명령을 생성하고, 코드를 입력합니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_cell-enable03.png)
    <br /><br />

4. 해당 프로젝트를 실행하면 하이퍼링크가 비활성화된 상태로 마우스 커서를 올려도 변하지 않습니다.<br />
    이후 버튼을 클릭하면 하이퍼링크가 활성화되며, 마우스 커서를 올리면 손가락 모양으로 클릭할 수 있게 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-enable04.gif)

<br /><br />