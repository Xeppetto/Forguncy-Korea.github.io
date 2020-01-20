---
title: Forguncy API - Cell - getContentPage
tags: [Forguncy, JavaScript, API, getContentPage]
keywords: Forguncy API, JavaScript API, getContentPage
last_updated: Jan 16, 2020
summary: "Forguncy API - Cell 클래스 중 getContentPage Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-getcontentpage.html
folder: forguncy5_03_javascript_api
---

### Cell - getContentPage Method
Cell.getContentPage()
<br /><br />

### getContentPage Method 설명
"내용이 포함된 셀" 유형을 사용하는 경우, 내용란에 들어가는 하위 페이지 객체를 가져옵니다. 
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
SubPage 속성을 반환합니다. 자세한 내용은 SubPage[]을 참고하세요.

> 😄 SubPage Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 cell.getContentPage를 사용하는 예제입니다. 페이지 내에 포함된 하위 페이지 객체 내부의 정보를 불러옵니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //Cell Name이 container라고 되어 있는 셀 인스턴스의 정보를 가져옵니다.
  var containerCell = page.getCell("container");

  //container셀이 포함하고 있는 하위 페이지 객체를 가져옵니다.
  var subPage = containerCell.getContentPage();

  //하위 페이지의 이름이 '페이지1'인지 확인합니다.
  if (subPage.getPageName() == "페이지1") {

    //하위 페이지 객체 정보 중 Cell Name이 myCell인 셀 인스턴스의 정보를 가져옵니다.
    var subPageCell = subPage.getCell("myCell");
  };

  //가져온 하위 페이지 셀 인스턴스의 정보 중 값을 화면에 표시합니다.
  alert(subPageCell.getValue());
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 두 개 생성합니다. 첫 번 째 페이지에는 "내용이 포함된 셀"을 선택합니다.<br />
    화면 왼쪽 상단의 Cell Name에 container라고 이름을 붙여줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getcontainerpage01.png)
    <br /><br />

2. 두 번 째 페이지에는 아무 컨텐츠나 컨텐츠를 넣어 줍니다. 예제에서는 화면 내 결과 출력을 위해 텍스트를 입력했습니다. <br />
    이후 페이지 왼쪽 위에 해당 Cell Name을 myCell이라고 적어줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getcontainerpage02.png)
    <br /><br />

3. 다시 첫 번 째 페이지로 가시 "내용이 포함된 셀"에 두 번 째 페이지를 넣어 줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getcontainerpage03.png)
    <br /><br />

4. 페이지에 버튼을 하나 생성하고, 해당 버튼에 "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getcontainerpage04.png)
    <br /><br />
    
5. 해당 프로젝트를 실행하고 버튼을 클릭하면 하위 페이지의 myCell에 들어 있는 테스트 값이 화면에 표시됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_cell-getcontainerpage05.gif)

<br /><br />
