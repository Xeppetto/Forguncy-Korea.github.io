---
title: Forguncy JavaScript API
tags: [Forgunc, JavaScript, API]
keywords: Forguncy API, JavaScript API
last_updated: Dec 23, 2019
summary: "Forguncy JavaScript API를 소개합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_intro.html
folder: forguncy5_03_javascript_api
---

Forguncy는 Excel과 비슷한 환경으로 사용하기 위해 Forguncy 개발자들이 사용할 수 있는 API를 제공합니다. Forguncy는 기본적으로 '웹개발 도구'라는 특성을 가지고 있기 때문에 Forguncy를 활용하여 웹 화면에 표시되는 각 항목들은 Properties, Method, Interface, Page object, Table object, Cell object 등 여러 종류의 세부 속성 값들을 가지게 됩니다. Forguncy API는 이런 속성 값들을 활용하여 더 유연한 웹개발을 할 수 있도록 도와줍니다.

Forguncy에 기본 탑재된 API는 JavaScript로 제공하고 있으며, 본 문서는 JavaScript API 사용 방법에 대해 설명합니다. 혹은 사용자 스스로 Plug-in을 작성하여 API처럼 Forguncy에 추가하셔서 사용하실 수도 있습니다.

> 알림 : 본 페이지는 초보자들을 위한 문서가 아니며 웹개발을 어느 정도 이해하고 있는 웹개발자들을 위한 문서입니다. 주요 개발 용어들을 번역하기 보다 실무에서 사용하는 언어들 그대로 두었습니다. 그러므로 웹개발 초보자분들은 Forguncy 기능 매뉴얼부터 보시면서 차근차근 실력을 쌓아 주세요.

Forguncy JavaScript API의 종류는 다음과 같습니다. 각 항목의 링크를 누르면 세부 내용을 보실 수 있습니다.

1. Namespace
Namespace | 설명
Forguncy | Forguncy의 Namespace는 'Forguncy'라고 정의합니다.

2. Page Variable
Page 변수 | 설명
Page | Forguncy는 웹개발 도구이며 결과 값이 페이지 단위로 표시되므로 Namespace에 Page 변수를 붙여 사용합니다.

3. Method
Method | 설명
addTableData | Database의 table에 데이터를 추가할 수 있습니다.
addUserToRole | 특정 사용자를 필요한 사용자 그룹/역할에 추가할 수 있습니다.
addUser | Forguncy 사용자를 추가하거나, 도메인 사용자를 추가할 수 있습니다.


ConvertDateToOADate
이 메서드를 사용 하 여 DateTimeOADate로 변환 합니다.
DateTime을 OADate로 변환하려면이 방법을 사용하십시오.

ConvertOADateToDate
이 메서드를 사용하여 OADATE에서 DateTime으로 변환합니다.
이 방법을 사용하여 OADATE에서 DateTime으로 변환하십시오.

ConvertToCssColor
변환에 지정된 색상 텍스트는 색상의 육각형 값인 CSS 색상 텍스트입니다.
지정된 색상 텍스트를 색상의 16 진수 값인 CSS 색상 텍스트로 변환합니다.

deleteTableData
기본Key 매개 변수를 통해 지정된 고유 레코드를 제거합니다.
primaryKey 매개 변수를 통해 지정된 고유 레코드를 삭제하십시오.

deleteUserFromRole
이 메서드를 사용 하 여 지정 된 그룹에서 지정 된 사용자를 제거 합니다.
지정된 그룹에서 지정된 사용자를 제거하려면이 방법을 사용하십시오.

deleteUser
지정된 사용자를 삭제하려면이 방법을 사용하십시오.
이 메서드를 사용하여 지정된 사용자를 제거합니다.

getTableDataByCondition
조건별로 데이터 테이블 또는 뷰의 데이터를 가져옵니다.
조건을 통해 데이터 테이블 또는 보기에서 데이터를 가져옵니다.

getTableDataByOData
OData 쿼리 문자열을 통해 데이터를 가져옵니다.
OData 쿼리 문자열에서 데이터를 가져옵니다.

getTableData
데이터베이스의 기본 키를 통해 데이터 테이블의 레코드를 가져옵니다.
데이터베이스의 기본 키를 통해 데이터 테이블에 레코드를 가져옵니다.

modifyTablesData
데이터 테이블에서 데이터를 추가, 수정 및 삭제하십시오.
데이터 테이블에서 데이터를 추가, 수정 및 삭제합니다.

SendMail
제목과 내용이 지정된 이메일을 지정된 이메일 주소로 발송합니다 발신자는 현재 웹 사이트에 로그인 한 사용자입니다. 이 API를 사용하여 이메일을 보내려면 SMTP 서비스가 올바르게 구성되어 있어야합니다.
지정된 제목과 콘텐츠가 지정된 전자 메일 주소로 전자 메일을 보내고 보낸 사람은 현재 웹 사이트에 로그인한 사용자입니다. 이 API를 사용하여 전자 메일을 보내려면 SMTP 서비스를 올바르게 구성해야 합니다.

updateTableData
primaryKey 매개 변수는 업데이트 할 유일한 행을 지정합니다.
기본Key 매개 변수는 업데이트에 대한 고유 행 레코드를 지정합니다.


4. Class
5. Interface
6. ListView

