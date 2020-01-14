---
title: Forguncy API - Page - getUserInfo
tags: [Forguncy, JavaScript, API, getUserInfo]
keywords: Forguncy API, JavaScript API, getUserInfo
last_updated: Jan 9, 2020
summary: "Forguncy API - Page 클래스 중 getUserInfo Method에 대해 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-getuserinfo.html
folder: forguncy5_03_javascript_api
---

### Page - getUserInfo Method
page.getUserInfo()
<br /><br />

### getUserInfo Method 설명
현재 로그인하여 서비스를 사용 중인 사용자 정보를 가져옵니다.
<br /><br />

### Parameter 설명
없음

1. UserInfo 인터페이스에 대한 자세한 내용은 다음과 같습니다.

    ~~~javascript
      interface UserInfo{
        //사용자이름 - Forguncy에서 사용자 이름은 로그인 ID를 의미합니다.
        UserName?: string;

        //사용자 전체 이름
        FullName?: string;

        //사용자가 등록한 사진이 있는지 확인
        HasPicture?: boolean;

        //사용자의 역할 그룹을 표시, 여러 개인 경우 ; 표시로 분리
        Role?: string;

        //사용자의 이메일 주소
        Email?: string;

        //사용자의 조직 정보 표시, 여러 개인 경우 | 표시로 분리
        OrganizationSuperior?: string;

        //그 외, 관리자가 추가 지정한 사용자 속성
        Properties?: UserExtendProperties[];

        //사용자가 속한 조직의 단계
        OrganizationLevelValues?: OrganizationLevelValueInfo[];
      }
    ~~~

2. 관리자가 추가 지정한 사용자 정의 속성인 UserExtendProperties 인터페이스에 대한 내용은 다음과 같습니다.

    ~~~javascript
      interface UserExtendProperties{
        //관리자가 추가 지정한 사용자 속성명
        PropertyName: string;

        //해당 속성에 대한 값 지정
        Value: string;
      }
    ~~~

3. 사용자가 속한 조직의 단계인 OrganizationLevelValueInfo 인터페이스에 대한 내용은 다음과 같습니다.

    ~~~javascript
      interface OrganizationLevelValueInfo{
        //조직 단계의 이름
        OrganizationLevelName: string;

        //해당 단계에 대한 값 지정
        Value: string;
      }
    ~~~

<br /><br />

### Response 시 반환값
UserInfo 속성을 반환합니다. 자세한 내용은 UserInfo[]를 참고하세요.

> 😄 UserInfo Method 관련 내용은 준비 중입니다.

<!-- <br /><br /> 위 memo를 삭제할 때 comment 제거 -->

### 활용 예제
아래는 page.getUserInfo를 사용하는 관련 사용 예제입니다. 현재 로그인한 사용자의 인스턴스 속성 전부를 보여줍니다.
<br />

~~~javascript
  //현재 페이지를 불러옵니다.
  var page = Forguncy.Page;
  
  //로그인한 사용자 인스턴스의 속성들을 가져옵니다.
  var userInfo = page.getUserInfo();

  //사용자 정보 JSON을 표시합니다.
  alert(JSON.stringify(userInfo, null, " "));
  
  //사용자 정보 중 해당 사용자의 사용자 이름을 확인합니다.
  var name = userInfo.UserName;

  //사용자 정보 중 해당 사용자의 역할 그룹을 확인합니다.
  var role = userInfo.Role;

  //사용자 정보 중 해당 사용자의 전체 이름을 확인합니다.
  var fullName = userInfo.FullName;
~~~

<br />

### Forguncy 사용 예제

1. 페이지를 생성한 후 셀에 "현재 사용자" 셀 유형을 적용합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getuserinfo01.png)
    <br /><br />

2. 해당 페이지에 버튼을 생성하고, "자바스크립트로 직접 프로그래밍하기" 명령으로 코드를 입력합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getuserinfo02.png)
    <br /><br />

3. 프로젝트를 실행하여 버튼을 누르면 getUserInfo를 화면에 표시합니다.

    ![]({{site.url}}/images/forguncy5/ex-ss_page-getuserinfo03.png)
        
<br /><br />