---
title: Forguncy API - Page - getListViews
tags: [Forguncy, JavaScript, API, getListViews]
keywords: Forguncy API, JavaScript API, getListViews
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getListViews Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getlistviews.html
folder: forguncy5_03_javascript_api
---

### Page - getListViews Method
Page.getListViews(includeSubPage)
<br /><br />

### getListViews Method 설명
페이지 내 모든 ListView들을 그룹으로 묶어 해당 인스턴스 그룹의 속성을 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| includeSubPage | boolean | 아니오 | 페이지 내 하위 페이지를 포함하는 컨테이너 또는 탭컨트롤이 존재하는 경우 하위 페이지까지 검색할 지 여부를 결정합니다. <br />기본값은 True이며 의미는 "검색함"입니다. False는 "검색하지 않음"입니다. |

<br />

### Response 시 반환값
ListView 속성을 반환합니다. 자세한 내용은 ListView[]를 참고하세요.

> 😄 ListView Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 page.getListViews를 사용하는 관련 사용 예제입니다. 페이지 내 Cell 중 컨테이너 유형의 Cell 인스턴스들의 정보를 불러옵니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;

  //페이지 내 ListView 인스턴스들을 불러옵니다.
  var listview = page.getListViews();
  
  //ListView 인스턴스 그룹의 길이를 확인합니다.
  var len = listview.length;
  
  //ListView 인스턴스 그룹의 길이를 화면에 표시합니다.
  alert(len);
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 한 개 생성하여 Database Table을 연결하는 ListView를 생성합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getlistviews01.png)
    <br /><br />

2. 해당 페이지에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 추가합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getlistviews02.png)
    <br /><br />

3. 프로젝트를 실행하여 버튼을 누르면 getListViews에서 화면의 ListView 개수를 화면에 표시합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getlistviews03.gif)

<br /><br />