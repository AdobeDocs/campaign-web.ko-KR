---
title: 외부 계정 관리
description: 외부 계정을 구성하는 방법 알아보기
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 2%

---

# 캠페인별 외부 계정 {#external-account}

선택한 외부 계정 유형에 따라 계정 설정을 구성하려면 아래 단계를 따르십시오.

## 바운스 메일 (POP3) {#bounce}

바운스 메일 외부 계정은 이메일 서비스 연결에 사용되는 외부 POP3 계정을 지정합니다. POP3 액세스용으로 구성된 모든 서버는 반송 메일을 받을 수 있습니다.

![바운스 메일(POP3) 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/external_account_bounce.png)

**[!UICONTROL 바운스 메일(POP3)]** 외부 계정을 구성하려면 다음 필드를 입력하십시오.

* **[!UICONTROL 서버]** - POP3 서버의 URL입니다.

* **[!UICONTROL 포트]** - POP3 연결 포트 번호(기본 포트: 110).

* **[!UICONTROL 계정]** - 사용자의 이름입니다.

* **[!UICONTROL 암호]** - 사용자 계정 암호입니다.

* **[!UICONTROL 암호화]** - 다음을 포함하여 선택한 암호화 유형:
   * 기본적으로(포트 110인 경우 POP3, 포트 995인 경우 POP3).
   * STARTTLS를 전송한 후 SSL로 전환하는 POP3.
   * POP3 비보안(기본적으로 포트 110).
   * POP3는 SSL(기본적으로 포트 995) 위에 보호됩니다.

* **[!UICONTROL 함수]** - 수신 전자 메일을 받을 계정을 구성하려면 **[!UICONTROL 인바운드 전자 메일]**&#x200B;을 선택하고, SOAP 요청을 처리하려면 **[!UICONTROL SOAP 라우터]**&#x200B;를 선택합니다.

>[!IMPORTANT]
>
>Microsoft OAuth 2.0을 사용하여 POP3 외부 계정을 구성하기 전에 먼저 Azure 포털에 애플리케이션을 등록해야 합니다. 자세한 정보는 이 [페이지](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}를 참조하십시오.

Microsoft OAuth 2.0을 사용하여 POP3 외부 환경을 구성하려면 Microsoft OAuth 2.0 옵션을 선택하고 다음 필드를 채우십시오.

* **[!UICONTROL Azure 테넌트]**

  Azure ID(또는 디렉터리(테넌트) ID)는 Azure 포털에 있는 애플리케이션 개요의 Essentials 드롭다운에서 찾을 수 있습니다.

* **[!UICONTROL Azure 클라이언트 ID]**

  클라이언트 ID(또는 애플리케이션(클라이언트) ID)는 Azure 포털에 있는 애플리케이션 개요의 Essentials 드롭다운에서 찾을 수 있습니다.

* **[!UICONTROL Azure 클라이언트 암호]**

  클라이언트 암호 ID는 Azure 포털에 있는 애플리케이션의 인증서 및 암호 메뉴에서 클라이언트 암호 열에 있습니다.

* **[!UICONTROL Azure 리디렉션 URL]**

  리디렉션 URL은 Azure 포털에 있는 애플리케이션의 인증 메뉴에서 찾을 수 있습니다. 다음 구문 nl/jsp/oauth.jsp(예: `https://redirect.adobe.net/nl/jsp/oauth.jsp`)으로 끝나야 합니다.

인터넷 액세스는 클라이언트 콘솔에서 연결 테스트 버튼을 사용하도록 설정해야 합니다. 설정 후 inMail 프로세스는 인터넷 없이 Microsoft 서버와 통신할 수 있습니다.

다른 자격 증명을 입력한 후 연결 설정 을 클릭하여 외부 계정 구성을 완료할 수 있습니다.

## 라우팅 {#routing}

외부 게재에 대한 특정 외부 계정을 구성하려면 아래 단계를 수행합니다.

1. 외부 계정을 만듭니다. [자세히 알아보기](create-external-account.md)

1. **[!UICONTROL 라우팅]** 유형을 선택하십시오.

   ![라우팅 외부 계정 유형 선택을 보여 주는 스크린샷입니다.](assets/external-account-routing.png){zoomable="yes"}

1. 원하는 채널을 선택하고 **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

1. 외부 계정 **[!UICONTROL 세부 정보]** 섹션에서 **[!UICONTROL 외부]**&#x200B;이(가) 기본적으로 **[!UICONTROL 배달 모드]**(으)로 선택됩니다.

   ![외부 계정 라우팅에 대한 게재 모드 구성을 보여 주는 스크린샷입니다.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >현재 **[!UICONTROL 외부]**&#x200B;만 사용할 수 있습니다.

1. 게재 실행 후 프로세스를 처리하려면 이를 사후 처리 워크플로우로 외부화합니다. [외부 신호](../workflows/activities/external-signal.md) 활동으로 워크플로우를 만들고 **[!UICONTROL 사후 처리]** 필드에서 선택합니다.

   ![외부 계정 라우팅에 대한 사후 처리 필드 구성을 보여 주는 스크린샷입니다.](assets/external-account-post-processing.png){zoomable="yes"}

1. **[!UICONTROL 활동]** 필드에서 로그에 표시되는 사후 처리 워크플로 활동의 이름을 편집합니다. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## 실행 인스턴스 {#instance-exec}

세그먼트화된 아키텍처가 있는 경우 제어 인스턴스와 연관된 실행 인스턴스를 식별하고 이들 인스턴스 간에 연결을 설정합니다. 트랜잭션 메시지 템플릿은 실행 인스턴스에 배포됩니다.

![실행 인스턴스 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/external_account_exec.png)

**[!UICONTROL 실행 인스턴스]** 외부 계정을 구성하려면:

* **[!UICONTROL URL]** - 실행 인스턴스가 설치된 서버의 URL.

* **[!UICONTROL 계정]** - 연산자 폴더에 정의된 메시지 센터 에이전트와 일치하는 계정의 이름입니다.

* **[!UICONTROL 암호]** - 연산자 폴더에 정의된 계정의 암호입니다.

* **[!UICONTROL 메서드]** - 웹 서비스와 FDA(Federated Data Access) 중에서 선택합니다.

  FDA의 경우 FDA 계정을 선택합니다. 외부 시스템에 대한 Campaign 연결은 고급 사용자로 제한되며 클라이언트 콘솔에서만 사용할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL 보관 워크플로 만들기]** - 인스턴스가 여러 개 있는지 여부에 관계없이 메시지 센터에 등록된 각 실행 인스턴스에 대해 실행 인스턴스와 연결된 각 외부 계정에 대해 별도의 보관 워크플로를 만드십시오.
