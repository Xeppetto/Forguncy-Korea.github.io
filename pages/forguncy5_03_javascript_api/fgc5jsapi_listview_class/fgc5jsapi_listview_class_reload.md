---
title: Forguncy API - ListView - reload
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, reload, Web, JavaScript, API
last_updated: Feb 10, 2020
summary: "Forguncy API - ListView 클래스 중 reload Method를 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_listview-class-reload.html
folder: forguncy5_03_javascript_api
---

### ListView - reload Method
listview.reload()
<br /><br />

### reload Method 설명
ListView를 다시 불러오기(reload) 합니다. ListView의 설정에 "자동으로 데이터 다시 불러오기" 옵션을 설정할 수도 있습니다. 
<br /><br />

### Parameter 설명
없음
<br /><br />

### Response 시 반환값
없음, void
<br /><br />

### 활용 예제
아래는 listview.reload를 사용하는 예제입니다. 버튼을 클릭하면 ListView의 값을 database에서 다시 불러옵니다.
<br />

~~~javascript
    //현재 페이지에 Namespace를 선언합니다.
    var page = Forguncy.Page;
    
    //이름이 ListView1인 ListView를 가져옵니다.
    var listview = page.getListView("ListView1");

    //ListView1이라는 이름을 가진 listview를 다시 불러오기(reload)합니다.
    listview.reload();
~~~

<br />

### Forguncy 사용 예제

1. 페이지 한 개 생성합니다. 데이터베이스 테이블을 한 개 생성한 후, 이름/생년월일/부서 열을 생성합니다.<br />
  데이터는 넣어도 되고 안 넣어도 됩니다. 본 예제에서는 알아보기 쉽게 하기 위해 가짜 데이터를 입력했습니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-reload01.png)
    <br /><br />

2. 화면의 영역을 선택하고 "ListView로 설정" 기능을 이용하여, ListView를 생성합니다.<br />
  이 때, 데이터베이스를 선택하라고 나타나는데, 위에서 생성한 테이블을 선택하시면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-reload02.png)
    <br /><br />

3. ListView에 데이터를 쉽게 입력하는 방법은 아래와 같습니다. 테이블의 열-이름을 드래그하면 됩니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-reload03.gif)
    <br /><br />

4. ListView의 이름을 설정합니다. ListView의 이름은 클릭 시 오른쪽의 '셀 유형' 탭에서 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-reload04.png)
    <br /><br />

5. 버튼을 한 개 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령을 이용하여 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-reload05.png)
    <br /><br />

6. 프로젝트를 생성합니다. 페이지가 로딩된 후 데이터베이스를 변경합니다. <br />
  프로젝트를 저장하고 다시 웹페이지로 돌아가서 Reload 버튼을 클릭하면 ListView에 새로 입력한 데이터가 나타납니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_listview-reload06.gif)

<br /><br />
