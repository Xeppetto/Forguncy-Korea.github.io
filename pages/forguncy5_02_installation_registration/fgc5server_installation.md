---
title: Forguncy Server 설치
tags: [제품 설치, Forguncy Server 설치]
keywords: Forguncy Server 설치
last_updated: Nov 29, 2019
summary: "Forguncy Server 설치하는 방법입니다."
sidebar: forguncy5_sidebar
permalink: fgc5server_installation.html
folder: forguncy5_02_installation_registration
---

Forguncy Server는 온라인에 다수의 서비스를 배포할 목적으로 사용하시는 도구입니다. Forguncy Builder로 개발하시는 중에는 Forguncy Server를 사용하지 않으셔도 됩니다.

Forguncy Server를 사용하지 않아도 Forguncy Builder만으로 서비스를 제작하여 실행하는 것이 가능하며,  Forguncy Builder에서 프로젝트를 실행하면 가상 서버가 실행되므로, 실행 중인 해당 컴퓨터의 IP 혹은 컴퓨터 이름으로 접속하시면 실행 중인 서비스를 이용하실 수 있습니다. <font color="purple">여기(준비 중)</font>를 클릭하셔서 자세한 내용을 확인하세요.

1. Forguncy Server는 아직 내부 정책상 온라인으로 배포하고 있지 않습니다. Forguncy Server는 다운로드 하시려면 그레이프시티 코리아 Forguncy 영업 담당자에게 연락해 주세요. 

- **그레이프시티 코리아 영업 대표:** [sales-kor@grapecity.com](mailto:sales-kor@grapecity.com)

2. Forguncy Server 설치 파일 다운로드가 완료되면, 다운로드 받은 Forguncy5.0.104_ServerKR.exe를 더블 클릭합니다. (본 매뉴얼은 해당 버전을 기준으로 설명합니다.)
    
    ![]({{site.url}}/images/forguncy5/installation_server_icon.png)

    ※ 참고 : 설치할 수 있는 시스템 호환성은 아래와 같습니다. 설치 전 세부 내용을 참고하여 주세요.
    
    | 구분 | Forguncy Server 시스템 요구사항 |
    | --- | --- |
    | 운영체제 |  윈도우 7 SP1 <br /> 윈도우 8.1 업데이트<br /> 윈도우 10 <br /> 윈도우 서버 2008 SP2 <br /> 윈도우 서버 2008 R2 SP1<br /> 윈도우 서버 2012<br /> 윈도우 서버 2012 R2 업데이트 <br />  윈도우 서버 2016 <br />  윈도우 서버 2019 <br />(Server Core 제외) |
    | 하드웨어 |  CPU: 코어™ i3 2GHz 이상 (듀얼 코어 이상 추천)<br /> 메모리: 최소 4GB 이상 (8GB 이상 추천)<br /> HDD 남은 공간: 최소 300MB 이상 (80GB 이상 추천)<br />(<font color="red">⚠</font> .NET Framework가 설치되지 않은 경우 HDD 2GB 이상 필요) |
    | 프레임워크 |  .NET 프레임워크 4.6 이상 버전 <br />(<font color="red">⚠</font> 해당 버전의 .NET 프레임워크가 설치되어 있지 않은 경우 별도로 설치하셔야 합니다.) |

    | 구분 | 외부 데이터베이스 연결 요구사항 |
    | Microsoft Access | MS Access DB 연결 시 Forguncy Server에 MS Access가 설치되어 있어야 합니다. |
    | Microsoft SQL Server | <br />  2012 SP3<br />  2014 SP2<br />  2016 SP2<br />  2017<br />  2019 <br />그 외 버전은 지원하지 않음 |
    | Oracle Database | 11g Release 2 (11.2)/12c Release 2 (12.2)/18c (18.3)<br /> ※ 32 비트 버전의 Oracle Database Client 설치가 필수 |
    | ODBC 데이터 원본 | ※ ODBC가 지원하는 모든 종류의 데이터베이스에 연결이 가능합니다.<br />그러나 모든 DB의 기능을 사용할 수 있는 것은 아니며, 제한이 있을 수 있습니다. |

    ※ 참고 : ODBC 데이터 연결 시 외부 데이터베이스와 직접 동기화되거나, 권한을 얻어 사용하지 않습니다. 향후 Version6에서 관련 업그레이드 예정되어 있습니다.

3. Forguncy Server 설치 화면이 나타납니다.

    (1) "사용자 라이선스 동의서를 확인하였으며 이에 동의함"에 동의하셔야 설치가 진행됩니다.

    ![]({{site.url}}/images/forguncy5/installation_server01.png)

    (2) 대상폴더는 기본으로 두셔도 되고, 사용자가 필요한 위치로 옮기셔도 됩니다.

    (3) EULA(사용자 라이선스 동의서)에 동의하시면 "설치" 버튼이 활성화됩니다. 클릭하셔서 설치를 진행해 주세요.

    ![]({{site.url}}/images/forguncy5/installation_server02.png)

<br /><br />

설치가 완료되면 Forguncy Server를 실행해 주세요.

설치 중 오류, 혹은 설치 후 Forguncy Server 실행 관련하여 문의사항이 있으신 경우 그레이프시티 코리아 기술지원([support-kor@grapecity.com](mailto:support-kor@grapecity.com))으로 연락주십시오.  오류가 발생한 경우에 대한 상황을 스크린샷 찍어주시거나, 명확히 설명해 주시면 빠른 문제 해결에 도움이 됩니다. 

그레이프시티 제품을 사용해 주셔서 고맙습니다.
