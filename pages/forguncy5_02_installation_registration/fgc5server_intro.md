---
title: Forguncy Server 소개
tags: [Forguncy 소개, Forguncy Server 소개]
keywords: Forguncy 제품 소개, Forguncy Server 소개, Forguncy Server 특징
last_updated: Jan 6, 2020
summary: "Forguncy Server를 소개하고 특장점을 설명합니다."
sidebar: forguncy5_sidebar
permalink: fgc5server_intro.html
folder: forguncy5_02_installation_registration
---

Forguncy Builder의 최대 강점은 전문적인 웹개발 지식 없이도 생성 가능한 간단한 화면 구성, 손쉬운 기능 구현입니다. 이런 강점이 가능한 이유는 Forguncy Server는 Builder에서 작성한 여러 요소들을 웹브라우저에서 표현할 수 있도록 하여 작동하는 API(Application Programming Interface)를 지원하기 때문입니다. Forguncy 자체 API는 사용자들이 작성한 화면과 기능을 변환하거나 해석하여 사용자의 웹브라우저에서 보여줍니다. 이런 Forguncy의 기술력을 사용하기 위해서는 Forguncy Server가 필수입니다.

![]({{site.url}}/images/forguncy5/fgc_server01.png)
<br /><br /><br />

### 어려운 고급 서버 기술을 몰라도 쉽게 설치가 가능하며, 손쉬운 배포와 서비스 관리가 가능합니다.

Forguncy Server는 Windows Server OS에 설치하기만 하면 바로 사용하실 수 있습니다. Forguncy Server를 사용하기 위해 별도의 서버 Framework를 이해하지 않으셔도 되며, IIS나 Apache 등 어려운 고도의 서버 기술을 몰라도 단순히 설치만으로 사용할 수 있는 서버입니다. 또한, Forguncy Server를 이용하기 위해서 어려운 배포(Deploy) 기술을 익힐 필요가 없습니다. Forguncy Builder에서 Server로의 배포 기능을 이용하여 서버 관리자의 정보를 입력하면, 사용자들은 곧바로 해당 서비스를 Forguncy Server를 설치한 서버에서 사용하실 수 있습니다.

![]({{site.url}}/images/forguncy5/fgc_server02.png)
<br /><br />

### 실행 중인 웹서버의 서비스를 중단하지 않고도 변경된 데이터를 반영할 수 있습니다.

일반적으로 운영 중인 서비스의 데이터를 변경할 때, 데이터베이스를 중단하지 않고 데이터를 변경하는 건 쉽지 않습니다. 특히 오래된 시스템일 수록 이 기술을 반영하는 데에 많은 인력과 시간 동안의 투입 공수를 산정해야 가능합니다. Forguncy Server에서는 간단히 배포 버튼을 누르는 것만으로 변경한 데이터베이스를 직접 운영 중인 서버에 반영할 수 있습니다.

<br />

### Forguncy 웹개발의 사용자 측면 절차를 설명합니다.

Forguncy를 사용하는 사용자들은 아래와 같은 방식으로 웹개발을 수행하시면 됩니다.

- Forguncy Builder에서 UI화면, 웹의 주요 기능을 개발한다.
- 데이터관리, 사용자 정보 관리가 필요한 경우 Forguncy Builder에서 개발한다.
- Forguncy Builder에서 간단한 배포 기능으로 Forguncy Server로 배포한다.
- Forguncy Server의 http 도메인 주소/프로젝트 주소로 접속한다.

![]({{site.url}}/images/forguncy5/fgc_server03.png)
<br /><br /><br />
