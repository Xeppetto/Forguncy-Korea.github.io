---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Jan 8, 2020
summary: "Forguncy API - Page 클래스 중 getCell에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getcell.html
folder: forguncy5_03_javascript_api
---

### Page - getCell Method
page.getCell(name, includeSubPage)
<br /><br />

### getCell Method 설명
개별 Cell Name을 기반으로 Cell 인스턴스의 속성을 가져옵니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| name | string | 예 | 특정 Cell에 부여된 Cell Name을 입력합니다. |
| includeSubPage | boolean | 아니오 | 페이지 내 포함된 하위 페이지들에서도 Cell Name을 검색할 지 선택합니다.<br />기본값은 True이며 "검색함"이고, False로 설정할 경우 "하위 페이지 검색 안함"으로 설정됩니다. |

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

1. aaaaa

<br /><br />