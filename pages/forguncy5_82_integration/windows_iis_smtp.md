---
title: Forguncy Server 관련 설치 - IIS에 SMTP 설치하기
tags: [Forguncy, IIS, Server]
keywords: Forguncy, 엑셀, RPA, IIS, Server, Addons, SMTP, 자동 메일 보내기
last_updated: Jun 20, 2020
summary: "Forguncy를 100% 활용하기 위해 추가로 SMTP를 설정하는 방법입니다."
sidebar: forguncy5_sidebar
permalink: windows_iis_smtp.html
folder: forguncy5_82_integration
---

본 페이지에서는 포건시를 이용하여 메일을 보내는 방법을 설명합니다.

<br />

> ※ 중요 안내<br />
  <br />
   • 본 페이지에서는 SMTP를 IIS 서버에 설치하고 활용하는 방법을 설명합니다.<br />
   • SMTP는 그레이프시티의 저작물이 아니며, 마이크로스프트에서 제공하는 기능입니다. 관련 기능 문의는 마이크로소프트로 해 주시기 바랍니다.<br />
   • 본 페이지의 내용은 포건시 서버가 Windows Server에 설치되어 있다고 가정한 매뉴얼입니다. 그 외 종류, 예를 들어 Windows7이나 Windows10 등, 서버가 아닌 제품에 SMTP 설정 및 포건시와의 연동은 고려하지 않았습니다.<br />

<br />

<h2>SMTP란?</h2>
SMTP(간이 우편 전송 프로토콜, Simple Mail Transfer Protocol)의 약자로 Windows Server에서 이메일을 주고 받을 수 있도록 하는 메일 서비스를 말합니다.

그 외, 자세한 내용은 [위키백과](https://ko.wikipedia.org/wiki/%EA%B0%84%EC%9D%B4_%EC%9A%B0%ED%8E%B8_%EC%A0%84%EC%86%A1_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C){:target="_blank"} 등 인터넷 검색을 활용해 주십시오.

<br />

<h2>SMTP 설치하기</h2>

1. 먼저 윈도우 서버의 ‘서버 관리자’를 실행합니다.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_001.png)

    <br />

2. 서버 관리자에서 ‘관리 > 역할 및 기능 추가’ 메뉴를 선택합니다.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_002.png)

    <br />

3. ‘역할 및 기능 추가 마법사’에서 진행하다가 ‘기능’ 탭에서 ‘SMTP 서버’에 체크합니다.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_003.png)

    <br />

4. SMTP를 처음 설치하는 경우 추가 기능을 설치한다는 팝업창이 나타날 수 있습니다. ‘기능 추가’ 버튼을 누르시고 계속 진행하십시오.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_004.png)

    <br />

5. ‘SMTP 서버’에 체크하셨으면 하단의 ‘다음’ 버튼을 눌러 계속 진행하십시오.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_005.png)

    <br />

6. ‘설치’ 버튼이 나타나면 클릭하여 설치하시고, 다음 그림과 같이 설치가 종료되면 ‘닫기’ 버튼을 클릭하여 설치를 완료하십시오.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_006.png)

    <br />

<h2>IIS에 SMTP 설정하기</h2>

1. 윈도우의 ‘제어판 > 관리도구’로 이동하십시오.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_007.png)

    <br />

2. ‘관리 도구’에는 2개의 IIS서버 설정 도구가 있습니다. 이 중 ‘IIS인터넷 정보 서비스 6.0 관리자’ 를 선택하십시오.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_008.png)

    <br />

3. 간단한 보안 정책을 적용하고 가겠습니다. 인터넷 정보 서비스 콘솔에서 [SMTP Virtual Server #1]에 마우스 오른쪽을 클릭 후 ‘속성’을 선택하세요.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_009.png)

    <br />

4. 속성 창에서 ‘엑세스’ 탭으로 이동하신 후 ‘릴레이’ 버튼을 클릭하세요.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_010.png)

    <br />

5. 릴레이 제한을 걸지 않으면 외부 해커가 해당 SMTP 서버를 스팸 메일 발송지로 이용할 수 있기 때문에 설정이 필요합니다. 아래의 그림을 참고하여 보안 정책을 적용해 주세요.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_011.png)

    <br />

6. ‘확인’ 버튼을 눌러 변경 사항을 저장하신 후, 모든 속성창을 받으시면 됩니다.

    <br />

<h2>포건시 서버에 SMTP 설정하기</h2>

1. 포건시 서버를 실행합니다.<br />
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_012.png)

    <br />

2. 웹브라우저에서 포건시 서버 콘솔이 시작되면 Administrator 계정과 암호를 입력하고 로그인합니다.<br />

3. ‘설정 > SMTP 설정’ 페이지로 이동하여 SMTP 정보를 입력합니다.
    ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_013.png)

    <br />

4. ‘테스트 이메일 주소’에 테스트 메일을 받을 주소를 입력합니다.<br />

5. ‘테스트 이메일 보내기’버튼을 클릭한 후, 입력한 이메일 주소로 메일 발송을 확인합니다.<br />

> ※참고사항<br />
  ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_014.png)<br />
  SMTP를 설정하면 총 4가지의 폴더구조를 볼 수 있습니다. 각 폴더의 기능은 다음과 같습니다.<br />
  • Badmail : SMTP 서버는 정상 처리하였으나, 발송 후 받는 사람 정보/서버 등에 문제가 생겨 반송된 경우 실패 사유와 함께 기록됩니다.<br />
  • Drop : 메일 형식이 잘 못 된 경우 메일 발송할 수 없으므로 이곳에 저장됩니다.<br />
  • Pickup : 처음 발송 시도되는 메시지가 보관되는 장소입니다.<br />
  • Queue : 발송 시 이곳을 거쳐 발송되며, 발송자/SMTP서버측의 문제로 못나가고 있는 경우 이곳에 남아있게 됩니다.<br />

  <br />

<h2>SMTP 메일 발송 오류 시</h2>

  최근 많은 회사에서 Google Suite나 Microsoft Office 365를 사용합니다. SMTP 설정하여 진행 시 서버에서 이를 차단하는 경우가 있습니다. SMTP 폴더에 생성된 파일을 열어보면 아래와 같이 오류 내용이 쓰여 있으므로, 기록된 오류 내용을 보고 조치를 취하시면 됩니다.
  ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_015.png)

  <br />

<h2>포건시 빌더에서 메일 보내기 기능 만들기</h2>

  포건시 빌더를 이용하여 메일을 보내는 기능을 만들어 보겠습니다. 

  결과를 먼저 소개하겠습니다. (그림으로만 나오는 점 양해 부탁드립니다.) 아래와 같은 화면처럼 주소 입력란에 이메일 주소를 입력하고 ‘테스트 메일 보내기’ 버튼을 클릭하면 메일을 받을 수 있습니다.
  ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_019.png)

  <br />
  
  support-kor@grapecity.com으로 실제 이메일을 받은 내용은 아래와 같습니다.
  ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_016.png)

  <br />

  위와 같이 작동하는 포건시 웹-애플리케이션을 서버로 배포해 보겠습니다.<br />
  
  본 예제는 포건시 빌더와 「포건시 서버」가 정상적으로 설치 완료되어 있다는 전제 하에 진행하는 예제입니다.<br />

  <br />

  1. 먼저 포건시를 실행합니다.<br />
      ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_017.png)

      <br />

  2. 아래와 같은 화면을 만듭니다.<br />
      ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_020.png)

      * 위 화면은 ②에 받는 분의 이메일 주소를 입력하고, ①의 버튼을 누르면 메일이 발송되도록 구현하였습니다.
      * ①은 버튼으로 만들고, ②는 텍스트 박스로 만들어 줍니다.

      <br />

  3. 버튼에 명령을 추가하여 이메일 보내기 명령을 아래와 같은 형식으로 구성합니다.<br />
      ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_021.png)

      <br />

  3. 상단 리본 메뉴에서부터 ‘배포 > 서버 배포’를 선택합니다. <br />

  4. 나타나는 ‘배포 설정’ 팝업에서 올바른 Administrator 계정, 암호, 서버 정보 등을 입력합니다.<br />
      ![]({{site.url}}/images/forguncy5/smtp/windows_iissmtp_018.png)

      <br />

  5. ‘배포’ 버튼을 눌러 웹-애플리케이션을 서버로 배포합니다. <br />

  6. 성공하면 웹브라우저에서 해당 서버의 주소로 애플리케이션이 실행됩니다. 이메일 주소를 입력하여 SMTP 기능이 정상 작동하는 지 확인하십시오.<br />

<br /><br />
