---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Jan 7, 2020
summary: "Forguncy API - Page 클래스 중 Bind Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-bind.html
folder: forguncy5_03_javascript_api
---

### Page - Bind Method
page.bind (type, data, fn, targetPage)
<br /><br />

### Bind Method 설명
특정 페이지에 이벤트들을 bind합니다. 현재 화면에 보이는 페이지, 지정한 특정 페이지 혹은 모든 페이지에 이벤트를 bind할 수 있습니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| eventType | string | 예	| 페이지의 이벤트 유형을 표시하는 문자열입니다. <br />페이지에 추가할 수 있는 이벤트와 관련한 내용은 PageEvent Class를 참고하세요. |
| data | any | 아니오	| 이 항목은 필수 입력사항은 아니며 선택적으로 사용하는 Parameter입니다. <br />값을 입력하지 않으면 무시되며, 값을 입력한 경우 Event Handler로 전달된 특정 Parameter를 표시합니다.|
| fn | function | 예 | Bind한 이벤트의 Event Handler입니다. |
| targetPage | string	| 아니오 | 이벤트를 Bind할 페이지의 이름입니다.<br />전체 페이지에 Bind하는 경우 "*"를 사용하시면 됩니다.<br />아무 것도 입력하지 않으시면 현재 페이지에 Bind합니다. |

<br />

### Response 시 반환값
없음
<br /><br />

### 활용 예제
아래는 page.bind에 관련 사용 예제입니다. 다음 예제들을 응용하여 페이지에 이벤트를 Bind하세요.
<br />

**예제1)**

현재 페이지에 이벤트를 Bind하여 이벤트 핸들러 전달합니다. 이 예제에서는 사용자 파라미터는 사용하지 않습니다.

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  //가져온 현재 페이지를 로딩 시에 arg1, arg2를 사용하는 어떤 함수를 실행하도록 이벤트를 Bind합니다.
  page.bind("loaded", function (arg1, arg2) {
    //arg2.현재 페이지 이름을 보여주는 팝업을 표시합니다.
    alert(arg2.pageName);
  });
~~~

**예제2)**

"페이지1"이라는 이름의 페이지에 이벤트를 전달할 때, 사용자 파라미터를 생성하여 Bind합니다.

~~~javascript
  //파라미터로 사용할 변수를 선언하고 값을 지정합니다.
  var text = "ready";
  //"페이지1"이라는 이름을 가진 페이지를 불러옵니다.
  var page = Forguncy.Page;
  //페이지 이벤트를 Bind합니다.
  page.bind("loaded", text, function (arg1, arg2) {
    //arg1.data를 보여주는 팝업을 표시합니다.
    alert(arg1.data);
  }, "페이지1");
~~~

**예제3)**

모든 페이지(*)에 이벤트를 Bind하여 이벤트 핸들러로 전달합니다.

~~~javascript
  //화면에 표시되는 페이지를 불러옵니다.
  var page = Forguncy.Page;
  //가져온 현재 페이지를 로딩 시에 arg1, arg2를 사용하는 어떤 함수를 실행하도록 이벤트를 Bind합니다.
  page.bind("loaded", function (arg1, arg2) {
    //"*"로 선언되어 모든 페이지에 적용되므로, 페이지1일 때는 페이지1의 내용을, 페이지2일 때는 페이지2의 내용을 팝업에 표시합니다.
    alert(arg2.pageName);
  }, "*");
~~~

<br />

### Forguncy 사용 예제

페이지가 로딩되는 시점에 팝업 메시지를 띄우는 예제를 JavaScript로 생성하여, Forguncy의 특정 페이지(예제에서는 '페이지1'이라는 이름의 페이지)에 불러옵니다.
![]({{site.url}}/images/forguncy5/ex-ss_page-bind-01.png)
<img src="https://forguncy-korea.github.io/images/forguncy5/ex-ss_page-bind-01.png" width=800>

해당 프로젝트를 실행하면 페이지가 표시되기 전에 해당 Forguncy 페이지의 이름인 '페이지1'이 팝업으로 표시됩니다. 팝업에서 '확인'을 누르면 이후 페이지 내용이 표시됩니다.
![]({{site.url}}/images/forguncy5/ex-ss_page-bind-02.png)

<br /><br />