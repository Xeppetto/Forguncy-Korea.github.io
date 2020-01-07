---
title: Forguncy API - Namespace
tags: [Forguncy, JavaScript, API, Namespace]
keywords: Forguncy API, JavaScript API, Namespace
last_updated: Jan 7, 2020
summary: "Forguncy API - Page Class의 전체 Method 목록입니다. 구분의 링크를 클릭하시면 세부 페이지 내용을 보실 수 있습니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_page-class-list.html
folder: forguncy5_03_javascript_api
---

## Page Class 목록 설명
본 페이지에서는 Page Class 전체 Method 목록을 표시합니다.
<br /><br />

## Method 목록

| 구분 | Page Class - Method 목록 |
| [bind](fgc5jsapi_page-class-bind.html) | 특정 페이지에 이벤트들을 bind합니다. 현재 화면에 보이는 페이지, 지정한 특정 페이지 혹은 모든 페이지에 이벤트를 bind할 수 있습니다. |
| getCellArray | Cell의 이름을 기반으로 Cell 인스턴스의 속성을 가져옵니다. |
| getCellByLocation | |
| getCell | |
| getContainerCells | |
| getListViews | |
| getListView | |
| getMasterPageName | |
| getPageName | |
| getSubPageInfoByPageID | |
| getUserInfo | |
| getUserName | |
| ready | |
| recalc | |
| reloadBindingData | |
| resumeCalc | |
| setCurrentRow | |
| suspendCalc | |
| unbindAll | |
| unbind | |



getCellArray	셀 이름으로 셀 인스턴스 세트를 가져옵니다.
겟셀어레이 / 셀 이름으로 셀 인스턴스 집합을 가져옵니다.
Gets a set of cell instances by cell name.

getCellByLocation	셀의 위치 정보에서 셀 객체를 가져옵니다.
getCellByLocation / 셀의 위치 정보에서 셀 개체를 가져옵니다.

getCell	셀 이름으로 셀 인스턴스를 가져옵니다.
겟셀 / 셀 이름으로 셀 인스턴스를 가져옵니다.

getContainerCells	탭 및 페이지 컨테이너 유형의 모든 셀을 가져옵니다 .
get컨테이너 셀 / 탭 및 페이지 컨테이너 유형의 모든 셀을 가져옵니다. 

getListViews	페이지에서 모든 양식을 가져옵니다.
getList뷰 / 페이지의 모든 테이블을 가져옵니다.

getListView	양식 이름으로 양식을 가져옵니다.
getListView / 테이블 이름으로 테이블을 가져옵니다.

getMasterPageName	현재 페이지의 마스터 페이지 이름을 가져옵니다.
get마스터 페이지 이름 / 현재 페이지의 마스터 페이지 이름을 가져옵니다.

getPageName	현재 페이지의 이름을 가져옵니다.
getPageName / 현재 페이지의 이름을 가져옵니다.

getSubPageInfoByPageID	페이지 ID별로 자식 페이지를 가져옵니다. 브라우저에서 각 상위 및 하위 페이지에는 고유 한 ID가 있습니다. 이 방법은 플러그인에서 사용하기에 더 적합합니다. 사용자는 CellTypeBase.getFormulaCalcContext  및  CommandBase.getFormulaCalcContext 메소드를 통해 페이지 ID 를 얻을 수 있습니다 .
getSubPageInfoByPageID / 페이지 ID에서 하위 페이지를 가져옵니다. 브라우저에서 각 상위 및 하위 페이지에는 고유한 ID가 있습니다. 이 방법은 플러그인에 사용하기에 더 적합합니다. 사용자는 CellTypeBase.get포뮬러CalcContext 및 명령베이스.get포뮬러칼컨텍스트를 통해 페이지 아이디를 얻을 수 있습니다. 

getUserInfo	현재 로그인 한 사용자의 정보를 가져옵니다.
getUserInfo  현재 누워 있는 사용자에 대한 로그인 정보를 가져옵니다.

getUserName	현재 로그인 한 사용자의 사용자 이름을 가져 오거나 사용자가 로그인하지 않은 경우 null 값을 반환합니다.
getUserName /  현재 lym 사용자의 사용자 이름을 가져옵니다 및 사용자가 로그인 하지 않은 경우 빈 값을 반환 합니다.

준비	페이지가 준비되면 매개 변수의 콜백 함수가 호출됩니다. 페이지가 처리 될 때 페이지가 준비되도록 페이지의 처리 논리를 콜백 함수에 기록하는 것이 좋습니다.
준비 / 페이지가 준비되면 인수의 콜백 함수가 호출되고 페이지의 처리 논리를 콜백 함수에 기록하여 페이지가 작동될 때 페이지가 준비되도록 하는 것이 좋습니다.

재 계산하다	페이지의 모든 수식을 다시 계산하도록합니다.
레칼크 / 페이지의 모든 수식을 다시 계산하도록 강제합니다.

reloadBindingData	현재 페이지에서 사용 된 테이블 및 뷰에서 데이터를 다시로드하십시오.
로드바인딩데이터 / 현재 페이지에 사용된 테이블 및 뷰에서 데이터를 다시 로드합니다.

이력서	페이지를 복원하기위한 수식 계산 논리는 일반적으로 많은 수의 조작 셀 뒤에 사용됩니다. 및  suspendCalc 방법  쌍으로 사용.
이력서Calc / 복구 페이지의 수식 계산 논리는 일반적으로 셀에 대한 많은 수의 작업 후에 사용됩니다. suspendCalc 메서드와 쌍으로 사용하려면.

setCurrentRow	현재 행 설정 예를 들어, 표 1의 현재 행이 테이블의 첫 번째 행으로 설정되면 페이지의 표 1의 모든 바인딩 필드에 첫 번째 행의 데이터가 표시됩니다.
설정전류행 / 테이블 1의 현재 행을 테이블의 첫 번째 행으로 설정하는 등 현재 행을 설정하고 모든 테이블 1의 바인딩 필드는 페이지에 있는 첫 번째 행에 대한 데이터를 표시합니다.

일시 중지	일시 중단 된 페이지의 수식 계산 논리, 즉 페이지의 수식 계산이 일시 중지됩니다. 더 나은 성능을 위해 많은 수의 셀 값을 조작하기 전에 일반적으로 사용됩니다. resumeCalc 메소드를 사용하여 계산을 재개하십시오   .
일시 중단Calc / 일시 중단된 페이지에서 수식 계산인 수식 계산 논리를 일시 중단합니다. 일반적으로 더 나은 성능을 위해 많은 수의 작업 셀 값 앞에 사용됩니다. 복구 계산은 resumeCalc 방법을 사용합니다.

바인드 해제	페이지에서 모든 이벤트를 바인드 해제하십시오. 이 메소드는 이벤트 핸들러를 제거하거나 이벤트가 발생할 때 지정된 기능을 종료 할 수 있습니다.
언빈드올 / 페이지의 모든 이벤트를 바인딩 해제합니다. 메서드는 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 작업을 종료할 수 있습니다.

바인드 해제	특정 이벤트를 바인드 해제하십시오. 이 메소드는 선택된 이벤트 핸들러를 제거하거나 이벤트가 발생할 때 지정된 기능을 종료 할 수 있습니다.
언바인딩/특정 이벤트의 바인딩을 해제합니다. 메서드는 선택한 이벤트 처리기를 제거하거나 이벤트가 발생할 때 지정된 함수의 작업을 종료할 수 있습니다.