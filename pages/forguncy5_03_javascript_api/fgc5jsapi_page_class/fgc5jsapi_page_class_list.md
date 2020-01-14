---
title: Forguncy API - Page - 전체 목록
tags: [Forguncy, JavaScript, API, page]
keywords: Forguncy API, JavaScript API, page
last_updated: Jan 13, 2020
summary: "Forguncy API - Page Class의 전체 Method 목록입니다. 구분의 링크를 클릭하시면 세부 페이지 내용을 보실 수 있습니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-list.html
folder: forguncy5_03_javascript_api
---

## Page Class 목록 설명
본 페이지에서는 Page Class 전체 Method 목록을 표시합니다.
<br /><br />

## Method 목록

| Method 목록 | 상세 설명 |
| --- | --- |
| [getUserInfo](fgc5jsapi_page-class-getuserinfo.html) | 현재 로그인하여 서비스를 사용 중인 사용자 정보를 가져옵니다. |
| [getUserName](fgc5jsapi_page-class-getusername.html) | 현재 로그인하여 서비스를 사용 중인 사용자의 이름을 가져옵니다. 로그인한 사용자가 없는 경우 null값을 반환합니다. |
| [bind](fgc5jsapi_page-class-bind.html) | 특정 페이지에 이벤트들을 bind합니다. 현재 화면에 보이는 페이지, 지정한 특정 페이지 혹은 모든 페이지에 이벤트를 bind할 수 있습니다. |
| [getCellByLocation](fgc5jsapi_page-class-getcellbylocation.html) | 특정 Cell의 위치 정보를 참조하여 Cell 인스턴스의 속성을 가져옵니다. |
| [getCell](fgc5jsapi_page-class-getcell.html) | 개별 Cell Name을 기반으로 Cell 인스턴스의 속성을 가져옵니다. |
| [getCellArray](fgc5jsapi_page-class-getcellarray.html) | 여러 개의 Cell들을 그룹으로 묶어 Cell Group Name을 기반으로 Cell Group 인스턴스의 속성을 가져옵니다. |
| [getContainerCells](fgc5jsapi_page-class-getcontainercells.html) | 페이지 내 [탭 컨테이너]()와 [내용이 포함된 컨테이너]() 등 다른 페이지를 불러오는 Cell 유형들을 그룹으로 묶어 해당 인스턴스 그룹의 속성을 가져옵니다. |
| [getListView](fgc5jsapi_page-class-getlistview.html) | 화면에 보이는 ListView 중 하나의 이름을 기반으로 하여 해당 ListView 인스턴스의 속성을 가져옵니다. |
| [getListViews](fgc5jsapi_page-class-getlistviews.html) | 페이지 내 모든 ListView들을 그룹으로 묶어 해당 인스턴스 그룹의 속성을 가져옵니다. |
| [getPageName](fgc5jsapi_page-class-getPageName.html) | 화면에 표시되는 현재 페이지의 이름을 가져옵니다. |
| [getMasterPageName](fgc5jsapi_page-class-getMasterPageName.html) | 화면에 보이는 페이지를 구성하는 요소 중 Forguncy에서 설정한 마스터페이지의 이름을 가져옵니다. |
| [getSubPageInfoByPageID](fgc5jsapi_page-class-getsubpageinfobypageid.html) | Page ID를 기반으로 하위 페이지 정보들을 가져옵니다. 브라우저상에 보이는 각 상위/하위 페이지들에 Forguncy는 각기 고유한 Page ID를 부여합니다.<br/>이를 이용하여 Forguncy로 제작하는 여러 기능들을 조절합니다. <br />[CellTypeBase.getFormulaCalcContext]()와 [CommandBase.getFormulaCalcContext]() 메소드들을 이용하여 페이지 ID를 확인하실 수도 있습니다. |
| [ready](fgc5jsapi_page-class-ready.html) | 페이지 로딩이 완료된 후 Ready 메소드에 정의한 Callback 함수가 호출됩니다.<br />페이지 내 기능 로직을 처리하는 방법으로 페이지 내의 모든 요소들이 작동 준비되었을 때 Callback으로 처리하는 방식이 더 추천하는 방식입니다. |
| [recalc](fgc5jsapi_page-class-recalc.html) | 페이지 내 모든 수식을 다시 계산하도록 합니다. |
| [reloadBindingData](fgc5jsapi_page-class-reloadbindingdata.html) | 현재 페이지에 사용 중인 Database의 Table들과 View들을 다시 불러오기합니다. |
| [resumeCalc](fgc5jsapi_page-class-resumecalc.html) | 페이지 내 작동하지 않는 수식들을 다시 작동하도록 합니다. <br />페이지 내 계산을 일시 중지하기 위해 [suspendCalc](fgc5jsapi_page-class-suspendcalc.html)와 함께 사용하시기를 추천합니다. |
| [setCurrentRow](fgc5jsapi_page-class-setcurrentrow.html) | Database 특정 값이 들어 있는 행을 지정합니다. 예를 들어, 어떤 데이터가 어떤 테이블의 3번째 행에 들어 있다면, 그 3번째 행의 모든 내용들이 화면의 페이지에 표시될 수 있도록 Database Table의 특정 행을 선택합니다. |
| [suspendCalc](fgc5jsapi_page-class-suspendcalc.html) | 페이지 내 수식들을 작동하지 않도록 합니다. 페이지 내 계산을 다시 계속하기 위해 [resumeCalc](fgc5jsapi_page-class-resumecalc.html)와 함께 사용하시기를 추천합니다. |
| unbindAll | 페이지 내 모든 이벤트들에 대한 bind를 해제합니다. 이 메소드는 Event handler를 제거하거나, 특정 함수의 이벤트 실행을 종료시킬 수 있습니다. |
| unbind | 특정 이벤트에 대한 bind를 해제합니다. 이 메소드는 선택한 Event handler를 제거하거나, 선택한 이벤트의 실행을 종료시킬 수 있습니다. |


