---
title: Forguncy ListView - 리스트뷰 세부 메뉴 사용하기
tags: [Forguncy, Github, 리스트뷰, ListView]
keywords: Forguncy, 엑셀, RPA, Github, 협업, 프로젝트
last_updated: Jun 15, 2020
summary: "Forguncy ListView의 세부 메뉴를 볼 수 있는 방법을 설명합니다."
sidebar: forguncy5_sidebar
permalink: forguncy5_listview_contextmenu.html
folder: forguncy5_05_listview
---

<h2>리스트뷰 학습 방법</h2>

  포건시 리스트뷰 학습 자료에서는 '이것을 어떻게 만드는가'는 설명하지 않습니다. 리스트뷰의 세부 메뉴들을 확인하셔서 어떤 옵션이 어떻게 작동하는 지에 대해 보시면서 학습해 주십시오.

  해당 리스트뷰의 내용들을 만드는 방법은 따로 매뉴얼을 작성하거나, 동영상을 제작하여 공개할 예정입니다.

<br /><br />

<h2>리스트뷰 세부 메뉴</h2>

1. 생성한 리스트뷰에서 마우스 오른쪽을 클릭하면 아래와 같이 메뉴가 나타납니다.

    ![]({{site.url}}/images/forguncy5/lv01-contextMenu01.png)

    | 구분 | 설명 |
    | --- | --- |
    | 셀 서식 | 리스트뷰 셀의 서식들을 지정합니다. 각 셀 단위로 지정할 수도 있고, 리스트뷰 전체 영역의 서식을 지정하실 수도 있습니다.|
    | 쿼리 조건 | 리스트뷰가 실행되는 시점(화면에 나타나는 시점)에 리스트뷰에서 보여줄 데이터를 선별하는 쿼리를 생성합니다.|
    | ListView 설정 | 리스트뷰의 세부 설정 값들을 조정할 수 있습니다. (뒤에 설명할 「디자인 메뉴」와 더불어 가장 많이 사용하는 기능입니다.)|
    | 세부 Detail ListView로 설정 | 리스트뷰의 특정 목록/값이 다른 데이터 테이블의 목록/값과 관련 있는 경우 이를 연결합니다.|
    | 열 이름 자동 생성 | 리스트뷰가 생성될 때 열 이름을 자동으로 생성하게 합니다.|
    | 모든 참조 찾기 | 리스트뷰에 명령이 추가되어 있거나, 다른 페이지/셀의 내용이 참조되어 있는 경우 이를 모두 찾아 연관성을 보여줍니다.|

2. 「ListView 설정」을 누르면 다음과 같은 세부 메뉴가 나타납니다. 각 항목들을 하나씩 눌러보며 학습하시면 됩니다.

    ![]({{site.url}}/images/forguncy5/lv01-contextMenu03.png)

<br /><br />

<h2>리스트뷰 디자인 메뉴</h2>

* 리스트뷰를 생성 후 선택하면, 리본 메뉴 상단에 리스트뷰 「디자인」 메뉴가 나타납니다. 여기에서는 리스트뷰의 모양 및 표현과 관련된 여러가지 설정을 하실 수 있습니다. (앞에서 설명한 「ListView 설정」 메뉴와 더불어 가장 많이 사용하는 기능입니다.)

    ![]({{site.url}}/images/forguncy5/lv01-contextMenu02.png)

    | 대분류 | 구분 | 설명 |
    | --- | --- | --- |
    | 속성 | ListView 이름 | 해당 리스트뷰의 이름을 설정합니다. 설정한 이름은 관련하여 명령을 수행하거나, JavaScript로 직접 코딩하는 기능을 생성하는 경우 활용합니다.|
    | | 크기 조정 시작 | 리스트뷰의 크기를 재조정합니다. 다시 한 번 클릭하면 조정이 완료됩니다.|
    | 세부 ListView | 세부 Detail ListView 설정 | 리스트뷰의 특정 목록/값이 다른 데이터 테이블의 목록/값과 관련 있는 경우 이를 연결합니다.|
    | 헤더 템플릿 | 열 헤더 | 리스트뷰의 상단에 구분할 수 있는 셀을 표시합니다.|
    | | 행 헤더 | 각 줄의 맨 앞에 구분할 수 있는 셀을 표시합니다.|
    | | 선택한 열 | (번역이 잘 못 된 케이스 - 수정 예정) 리스트뷰의 1번째 열에 체크박스(Checkbox)를 표시합니다. 체크박스를 이용하여 리스트뷰 여러 열에 대한 명령을 수행하거나, 다른 작업을 하도록 코딩할 수 있습니다.|
    | | 전체 행 보기 | (번역이 잘 못 된 케이스 - 수정 예정) 리스트뷰 하단에 전체 내용에 대해 평균을 내는 등 정리하는 내용을 표시할 수 있도록 합니다.|
    | 쿼리 조건 | 쿼리 조건 | 해당 리스트뷰가 실행되는 시점(화면에 나타나는 시점)에 리스트뷰에서 보여줄 데이터를 선별하는 쿼리를 생성합니다.|
    | | 정렬 기준 | 해당 리스트뷰에 데이터를 표시할 때 정렬하는 기준을 결정합니다.|
    | | 최상위 조건 | (번역이 잘 못 된 케이스 - 수정 예정) 데이터의 수가 많은 경우 초기에 리스트뷰를 표시할 때 몇 개를 표시할 지 정할 수 있습니다. 「제한 없음」으로 하면 해당 데이터 테이블의 모든 데이터를 표시합니다. 일반적으로 「실시간 처리」를 활성화하여 함께 사용합니다.|
    | | 실시간 처리 | 리스트뷰의 화면에 표시할 만큼만 데이터를 읽어온 경우 리스트뷰의 스크롤을 이동하면, 데이터를 실시간으로 읽어와 리스트뷰에 표시합니다.|
    | | 불러올 행 수 | 「실시간 처리」를 활성화하면 사용할 수 있는 기능으로, 실시간 처리할 때 어느 정도의 데이터를 읽어오는 가를 정합니다.|
    | 편집 | 편집 허용 | 리스트뷰를 클릭하여 수정/편집할 수 있도록 합니다. 체크 해제되어 있으면 「읽기전용」으로 표시됩니다.|
    | | 새 행 추가 허용 | 「편집 허용」을 사용 시 새로운 줄/행을 추가할 수 있도록 하는 기능합니다.|
    | | 삭제 허용 | 리스트뷰에서 데이터를 직접 삭제할 수 있도록 하는 기능입니다. 이 기능으로 데이터 삭제 시 데이터베이스에서도 삭제되므로 신중히 사용하십시오.|
    | 열 설정 | 숨기기 무시 | 리스트뷰가 포함된 셀을 「숨기기」한 경우 이 옵션을 선택하면 리스트뷰에 스크롤이 발생하며 내용이 모두 표시됩니다. 왼쪽 메뉴 중 「응용 > 숨기기 무시」를 참고하여 주세요.|
    | | 자동 병합 | 각 셀간 같은 값이 붙어 있을 경우 셀을 병합해서 표시합니다.|
    | ListView 스타일 | 스타일 | ListView의 색상, 모양 등을 빠르게 결정합니다. 그레이프시티에서 제공하는 기본 템플릿 색상을 테마로 제공합니다.|

<br /><br />

관련하여 문의사항이 있으시면 언제든지 그레이프시티 코리아 기술지원(support-kor@grapecity.com)으로 연락 주십시오.

<br /><br />