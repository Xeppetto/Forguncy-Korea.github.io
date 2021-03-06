---
title: Forguncy JavaScript API
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, Web, JavaScript, API
last_updated: Jan 7, 2020
summary: "Forguncy JavaScript API를 소개합니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_intro.html
folder: forguncy5_03_javascript_api
---

Forguncy는 프로그래밍에 전문성을 갖추지 않은 비-개발자들도 손쉽게 웹서비스를 개발할 수 있도록 해 줍니다. 이런 손쉬운 개발이 가능한 이유는 사용자가 웹개발 시 사용하는 내용들을 API와 그레이프시티의 기술력으로 자동화 해 두었기 때문에 가능합니다. 

Forguncy는 Excel과 비슷한 환경으로 사용하기 위해 Forguncy는 C#과 JavaScript로 프로그래밍된 API를 제공하고 있으며, 전문 개발자들은 Forguncy API를 사용하여 더 편리한 기능들을 만들 수 있습니다. Forguncy는 기본적으로 '웹개발 도구'라는 특성을 가지고 있기 때문에 Forguncy를 활용하여 웹 화면에 표시되는 각 항목들은 Properties, Method, Interface, Page object, Table object, Cell object 등 여러 종류의 세부 속성 값들을 가지게 됩니다. Forguncy API는 이런 속성 값들을 활용하여 더 유연한 웹개발을 할 수 있도록 도와줍니다.

C# API를 이용하셔서 Forguncy Builder에서 작업하는 환경과 Forguncy Server에서 작동하는 기능을 만드실 수 있고, JavaScript API로는 웹브라우저에서 사용자에게 보이는 기능들을 프로그램하실 수 있습니다.

본 문서는 JavaScript API 사용 방법에 대해 설명합니다. 혹은 사용자 스스로 Plug-in을 작성하여 기본 제공되는 API처럼 Forguncy에 추가하셔서 사용하실 수 있습니다.

<br /><br />

---

> 알림 : 본 페이지는 초보자들을 위한 문서가 아니며 웹개발을 어느 정도 이해하고 있는 웹개발자들을 위한 문서입니다. 주요 개발 용어들을 번역하기 보다 실무에서 사용하는 언어들 그대로 두었습니다. 그러므로 웹개발 초보자분들은 <font color="purple">Forguncy 기능 매뉴얼(준비 중)</font>부터 보시면서 차근차근 실력을 쌓아 주세요.

---

<br /><br />

Forguncy JavaScript API의 종류는 다음과 같습니다. 각 항목의 링크를 누르면 세부 내용을 보실 수 있습니다.

## Namespace

| Namespace | 상세 설명 |
| --- | --- |
| [Forguncy](fgc5jsapi_namespace.html) | Forguncy의 Namespace는 'Forguncy'라고 정의합니다. |

<br />

## Page Variable

| Page Variable | 상세 설명 |
| --- | --- |
| [Page](fgc5jsapi_page-variable.html) | Forguncy는 웹개발 도구이며 결과 값이 페이지 단위로 표시되므로 Namespace에 Page 변수를 붙여 사용합니다. |

<br />

## Method

| Method | 상세 설명 |
| --- | --- |
| addTableData | Database의 Table에 데이터를 추가합니다. |
| addUserToRole | 특정 사용자를 필요한 사용자 그룹/역할에 추가합니다. |
| addUser | Forguncy 사용자를 추가하거나, 도메인 사용자를 추가합니다. |
| ConvertDateToOADate | DateTime을 OADate로 변환합니다. |
| ConvertOADateToDate | OADate를 DateTime으로 변환힙니다. |
| ConvertToCssColor | 지정한 부분의 색상값을 CSS 색상 텍스트로 변환하여 표시합니다. |
| deleteTableData | Primary Key를 변수로 이용하여 특정 Data를 삭제합니다. |
| deleteUserFromRole | 지정한 사용자를 특정 그룹으로부터 제거합니다. |
| deleteUser | 지정한 사용자를 DB에서 삭제합니다. |
| getTableDataByCondition | 특정 조건을 지정하여 Database의 Table에 있는 Data를 가져옵니다. |
| getTableDataByOData | OData 쿼리 문자열을 이용하여 Database의 Table에 있는 Data를 가져옵니다. |
| getTableData | Database의 특정 Key값을 이용하여 Table에 있는 Data를 가져옵니다. |
| modifyTablesData | Database의 Table에서 Data를 추가/수정/삭제합니다. |
| SendMail | 제목과 내용, 수신자 이메일(현재 웹사이트 이용자)을 지정하여 이메일을 발송합니다. 이 API를 사용하려면 SMTP 서비스가 올바르게 구성해야 합니다. |
| updateTableData | Primary Key를 이용하여 Database Table의 특정 Row(행)의 데이터를 업데이트합니다. |

<br />

## Class

| Class | 상세 설명 |
| --- | --- |
| [Cell](fgc5jsapi_cell-class-list.html) | Cell Object 관련 Class입니다. |
| CellEvents | Cell에서 사용할 수 있는 이벤트 관련 Class입니다. |
| [Page](fgc5jsapi_page-class-list.html) | Page Object 관련 Class입니다. |
| Helper | Helper Method와 관련한 정보들의 속성을 제공하는 Class입니다. |
| [ListView](fgc5jsapi_listview-class-list.html) | ListView Object 관련 Class입니다. |
| ListViewEvents | ListView에서 사용할 수 있는 이벤트를 설정하는 Class입니다. |
| [PageEvents](fgc5jsapi_cellevent-class-list.html) | Page에서 사용할 수 있는 이벤트 관련 Class입니다. |
| SpecialPath | Forguncy 내 특정 경로와 관련된 Class입니다. |

<br />

## Interface

| Interface | 상세 설명 |
| --- | --- |
| CellLocationInfo | 특정 Cell의 위치 정보와 관련한 Interface입니다. |
| CellRange | Cell의 범위 값 정보와 관련한 Interface입니다. |
| CurrentRowInfoParam | 현재 Row(행)과 관련된 Parameter 정보에 관련한 Interface입니다. |
| FormulaCalcContext | Excel 방식의 수식 계산과 관련한 Interface입니다. |
| GetTableDataByConditionParams | Database의 Table 혹은 View에서 Data를 가져올 때 사용하는 Interface입니다. |
| IMergedColumnInfo | Column(열)과 관련된 정보들에 관련한 Interface입니다. |
| ListviewPaginationInfo | ListView를 지정한 개 수 만큼 나누어 화면에 표시하고, 대신 페이지를 나누도록 하는 데에 관련한 Interface입니다. |
| ListViewValueChangedEventArg | ListView의 값이 변경되는 내용과 관련한 Interface입니다. |
| ModifyData | Database의 Table에서 데이터를 변경하는 내용과 관련한 Interface입니다. |
| OrganizationLevelValueInfo | 사용자 정보 중 속한 조직 정보에 관련한 Interface입니다. |
| RowData | Database Table의 Row(행) 정보를 다루는 데 필요한 Interface입니다. |
| TableDataQueryPolicy | Database Table에 Qeury를 보내 Data를 가져올 때 사용하는 Interface입니다. |
| UserExtendProperties | 사용자와 관련한 세부 속성과 관련한 Interface입니다. |
| UserInfo | 사용자에 대한 정보와 관련한 Interface입니다. |

<br />

## ListView

| ListView | 상세 설명 |
| --- | --- |
| ListviewColumnType | ListView 테이블의 Column(열) 형식과 그에 관한 정보들을 나타냅니다. |
| QueryNullPolicy | Database의 Table 정보, 혹은 View 정보를 가져오는 동안 발생하는 Null에 대한 정책을 관리합니다. |

<br />

위 API 문서는 Forguncy Global 개발팀의 문서를 번역한 내용입니다. 이와 관련된 오류사항 신고, 문의사항은 그레이프시티 코리아 기술지원([support-kor@grapecity.com](support-kor@grapecity.com))으로 연락주십시오.
