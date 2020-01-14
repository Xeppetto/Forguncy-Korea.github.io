---
title: Forguncy API - Page - unbindall
tags: [Forguncy, JavaScript, API, unbindall]
keywords: Forguncy API, JavaScript API, unbindall
last_updated: Jan 14, 2020
summary: "Forguncy API - Page 클래스 중 unbindall Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-unbindall.html
folder: forguncy5_03_javascript_api
---

### Page - UnbindAll Method
page.unbindall (targetPage)
<br /><br />

### UnbindAll Method 설명
특정 페이지에 이벤트들을 unbind합니다. Event handler를 페이지에서 제거하거나, 발생한 특정 이벤트를 종료시킬 수 있습니다.
<br /><br />

### Parameter 설명

| Parameter 이름 | 타입 | 필수 | 상세 설명 |
| --- | --- | --- | --- |
| targetPage | string	| 아니오 | 이벤트를 Unbind할 페이지의 이름입니다.<br />전체 페이지에 Unbind하는 경우 "*"를 사용하시면 됩니다.<br />아무 것도 입력하지 않으시면 현재 페이지에만 Unbind합니다. |

<br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 page.unbindall을 사용하는 예제입니다. 다음 예제들을 응용하여 페이지 내에서 작동하는 이벤트를 Bind/Unbind 할 수 있습니다.
<br />

~~~javascript
  //현재 페이지에 Namespace를 선언합니다.
  var page = Forguncy.Page;
  
  //가져온 현재 페이지를 로딩 시에 arg1, arg2를 사용하는 어떤 함수를 실행하도록 합니다.
  var eventHandler = function (arg1, arg2) {
      
      //arg2.현재 페이지 이름을 보여주는 팝업을 표시합니다.
      alert(arg2.pageName);
  };

  //위에서 설정한 이벤트를 페이지에 bind합니다.
  page.bind("Loaded", eventHandler);
  
  //현재 페이지에 bind된 이벤트들을 모두 unbind all/모두 해제합니다.
  page.unbindAll();
  
  //'페이지1'이라는 이름을 가진 페이지에서만 이벤트를 unbind all합니다.
  page.unbindAll("페이지1");
  
  //모든 페이지에서 이벤트를 unbind all합니다.
  page.unbindAll("*");
~~~

<br />

### Forguncy 사용 예제

1. 이번 예제에서는 페이지 생성 전에 아래와 같이 2개의 js 파일을 생성합니다.<br />
    (1) 하나는 이벤트를 페이지 로딩 시점(OnLoad)에 binding 하는 스크립트입니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-unbindall01.png)
    <br />

    (2) 다른 하나는 같은 코드 내용이지만, 이벤트를 binding함과 동시에 unbinding 하는 스크립트입니다.
    ![]({{site.url}}/images/forguncy5/ex-ss_page-unbindall02.png)
    <br /><br />

2. 페이지를 한 개 생성한 후, "페이지 설정" > "사용자 JavaScript"의 폴더 아이콘을 클릭하여 binding한 스크립트를 먼저 가져옵니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-unbindall03.png)
    <br />

    프로젝트를 저장하여 실행하면, 아래와 같이 페이지 이름을 출력하는 팝업창이 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-unbindall04.png)
    <br /><br />

3. 이번엔 unbinding 하는 스크립트를 가져옵니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-unbindall05.png)
    <br />

    프로젝트를 저장하여 실행하면 팝업창이 나타나지 않고, 해당 페이지가 바로 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-unbindall06.png)

<br /><br />