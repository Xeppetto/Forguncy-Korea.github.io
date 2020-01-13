---
title: Forguncy API - Page - getSubPageInfoByPageID
tags: [Forguncy, JavaScript, API, getSubPageInfoByPageID]
keywords: Forguncy API, JavaScript API, getSubPageInfoByPageID
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getSubPageInfoByPageID에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getsubpageinfobypageid.html
folder: forguncy5_03_javascript_api
---

### Page - getSubPageInfoByPageID Method
page.getSubPageInfoByPageID(pageID)
<br /><br />

### getSubPageInfoByPageID Method 설명
Page ID를 기반으로 하위 페이지 정보들을 가져옵니다. 브라우저상에 보이는 각 상위/하위 페이지들에 Forguncy는 각기 고유한 Page ID를 부여합니다.이를 이용하여 Forguncy로 제작하는 여러 기능들을 조절합니다. <br /><br />[CellTypeBase.getFormulaCalcContext]()와 [CommandBase.getFormulaCalcContext]() 메소드들을 이용하여 페이지 ID를 확인하실 수도 있습니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| pageID | string | 예 | 각 페이지에 부여된 ID를 입력합니다. |

<br />

### Response 시 반환값
SubPage 속성을 반환합니다. 자세한 내용은 SubPage[]를 참고하세요.

> 😄 SubPage Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 page.getSubPageInfoByPageID 사용하는 관련 사용 예제입니다. 해당 페이지의 이름을 보여줍니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //확인 중입니다.
  //아래 예제는 웹에서 작동하는 JavaScript가 아니라 Plugin 방식으로 개발할 때 사용하는 코드로 현재 예제를 개발 중입니다.
  //아래 예제 코드가 너무 오랫동안 실제 예제 없이 코드만 방치되어 있다면 기술지원으로 알려주세요. 가능한 빠르게 예제를 개발하여 보여드리겠습니다.
  var pageID = this.getFormulaCalcContext().PageID;
  var pageInfo = Forguncy.Page.getSubPageInfoByPageID(pageID);
  return pageInfo ? pageInfo.getListView(listViewName) : Forguncy.Page.getListView(listViewName, false);
~~~

<br />

### Forguncy 사용 예제

본 Method Plugin 방식으로 개발할 때 사용하는 코드로 현재 예제를 개발 중입니다.

위의 예제 코드가 너무 오랫동안 실제 예제 없이 코드만 방치되어 있다면 기술지원으로 알려주세요. 가능한 빠르게 예제를 개발하여 보여드리겠습니다.


<br /><br />