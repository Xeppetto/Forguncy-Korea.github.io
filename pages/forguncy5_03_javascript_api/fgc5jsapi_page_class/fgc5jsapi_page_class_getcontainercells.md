---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getContainerCells를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getcontainercells.html
folder: forguncy5_03_javascript_api
---

### Page - getCell Method
page.getContainerCells(includeSubPage)
<br /><br />

### getCell Method 설명
페이지 내 [탭 컨테이너]()와 [내용이 포함된 컨테이너]() Cell 유형의 Cell 인스턴스의 속성을 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| includeSubPage | boolean | 아니오 | 페이지 내 하위 페이지를 포함하는 컨테이너 또는 탭컨트롤이 존재하는 경우 하위 페이지까지 검색할 지 여부를 결정합니다. <br />기본값은 True이며 의미는 "검색함"입니다. False는 "검색하지 않음"입니다. |

<br />

### Response 시 반환값
Cell 속성을 반환합니다. 자세한 내용은 Cell[]을 참고하세요.

> 😄 Cell Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 page.getContainerCells를 사용하는 관련 사용 예제입니다. 페이지 내 Cell 중 컨테이너 유형의 Cell 인스턴스들의 정보를 불러옵니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  //페이지 내 컨테이너 셀들을 불러옵니다.
  var cell = page.getContainerCells();
  //Cell 인스턴스의 길이를 확인합니다.
  var len = cell.length;
  //Cell 길이를 화면에 표시합니다.
  alert(len);
~~~

<br />

### Forguncy 사용 예제

1. Forguncy에서 페이지 2개를 생성합니다. 

2. "페이지2"에 아무 내용이나 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcontainercells01.png)]
    <br /><br />

3. "페이지1"에 "페이지 내 탭 컨트롤 셀"과 "내용이 포함된 셀 타입"을 지정하고, 해당 셀의 내용으로 "페이지2"를 지정합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcontainercells02.png)]
    <br /><br />

    ※ 참고 : 위에서 사용한 셀 유형은 아래와 같은 위치에 있습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcontainercells04.png)]
    <br /><br />

4. "페이지1"에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcontainercells03.png)]
    <br /><br />

5. 해당 프로젝트를 실행하고, 버튼을 누르면 getContinerCells는 두 개의 셀 유형을 감지하여 2를 보여줍니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getcontainercells05.png)]

<br /><br />