---
title: Forguncy API - Cell - 전체 목록
tags: [Forguncy, JavaScript, API]
keywords: Forguncy API, JavaScript API, cell, Web, JavaScript, API
last_updated: Jan 14, 2020
summary: "Forguncy API - Cell Class의 전체 Method 목록입니다. 구분의 링크를 클릭하시면 세부 페이지 내용을 보실 수 있습니다."
sidebar: forguncy5_sidebar
permalink: fgc5jsapi_cell-class-list.html
folder: forguncy5_03_javascript_api
---

## Cell Class 목록 설명
본 페이지에서는 Cell Class 전체 Method 목록을 표시합니다.
<br /><br />

## Method 목록

| Method 목록 | 상세 설명 |
| --- | --- |
| [disable](fgc5jsapi_cell-class-disable.html) | 특정 셀을 비활성화합니다. 셀을 비활성화하면 클릭하거나 사용하실 수 없습니다. 다시 사용하시려면 활성화(enable)하셔야 합니다. |
| [enable](fgc5jsapi_cell-class-enable.html) | 특정 셀을 활성화합니다. 셀을 비활성화하시려면 비활성화(disable) 메소드를 사용하셔야 합니다. |
| [hide](fgc5jsapi_cell-class-hide.html) | 특정 셀을 숨기기합니다. 셀을 숨길 때 셀에 입력된 값과 유형 등은 숨길 수 있지만, 셀의 배경색상은 숨길 수 없습니다. [show()](fgc5jsapi_cell-class-show.html) 메소드와 함께 사용할 수 있습니다. |
| [show](fgc5jsapi_cell-class-show.html) | 특정 셀을 보이기합니다. 셀에 입력된 값과 유형 등을 보이기합니다. [hide()](fgc5jsapi_cell-class-hide.html) 메소드와 함께 사용할 수 있습니다. |
| [getValue](fgc5jsapi_cell-class-getvalue.html) | 특정 셀에 입력된 값을 가져옵니다. 셀의 값을 가져와 여러가지 작업을 수행할 수 있습니다. |
| [setValue](fgc5jsapi_cell-class-setvalue.html) | 지정한 특정 셀에 지정한 값을 입력합니다. 값은 임의의 값일 수 있으며, 웹에서 표현할 수 있는 형식이라면 제한이 없습니다. |
| [bind](fgc5jsapi_cell-class-bind.html) | 선택한 특정 셀에 한 개 이상의 이벤트를 bind하고, 이벤트 발생 시 실행할 함수를 지정합니다. |
| [unbind](fgc5jsapi_cell-class-unbind.html) | 선택한 셀에 지정된 이벤트들을 unbind/해제하거나, 발생한 특정 이벤트를 종료시킬 수 있습니다. |
| [unbindall](fgc5jsapi_cell-class-unbindall.html) | 모든 셀에 지정된 이벤트들을 모두 unbind/해제하거나, 발생한 모든 이벤트를 종료시킬 수 있습니다. |
| [getTabCount](fgc5jsapi_cell-class-gettabcount.html) | 아래는 cell.getTabCount를 사용하는 예제입니다. 전체 탭의 수를 보여줍니다. |
| [getActiveTabIndex](fgc5jsapi_cell-class-getactivetabindex.html) | 탭페이지 셀 유형을 사용할 때, 활성화된 탭의 index 번호를 가져옵니다. |
| [showTab](fgc5jsapi_cell-class-showtab.html) | "페이지 내 탭 컨트롤 셀" 유형을 사용하여 지정한 탭을 화면에 활성화합니다. |
| [getTabPage](fgc5jsapi_cell-class-gettabpage.html) | 탭의 index 번호를 입력합니다. 탭의 index는 0부터 시작합니다. |
| [getContentPage](fgc5jsapi_cell-class-getcontentpage.html) | "내용이 포함된 셀" 유형을 사용하는 경우, 내용란에 들어가는 하위 페이지 객체를 가져옵니다. |
| [hasFocus](fgc5jsapi_cell-class-hasfocus.html) | 지정한 특정 셀에 포커스가 되어 있는 지 여부를 확인하고, 포커스 되도록 설정할 수 있습니다. |
| [setFocus](fgc5jsapi_cell-class-setfocus.html) | 보통 상황에서는 사용자가 마우스로 클릭한 요소에 Focus가 배치됩니다. 하지만 setFocus를 이용해서 지정한 특정 셀에 Focus를 보낼 수 있습니다. |
| [setBackColor](fgc5jsapi_cell-class-setbackcolor.html) | 지정한 특정 셀의 배경 색상을 변경합니다. |
| [setForeColor](fgc5jsapi_cell-class-setforecolor.html) | 지정한 특정 셀의 글자 색상을 변경합니다. |