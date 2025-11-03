---
title: 외부 계정 관리
description: CRM 외부 계정을 구성하는 방법 알아보기
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# CRM 외부 계정 {#external-crm}

외부 CRM 유형 계정을 사용하여 Adobe Campaign을 서드파티 데이터베이스와 연결합니다.

이 외부 계정에 대한 구성 설정은 연결 중인 특정 데이터베이스 엔진에 따라 다릅니다. 지원되는 각 데이터베이스에 대한 자세한 설정 지침은 아래 섹션에 나와 있습니다.

## Microsoft Dynamics CRM

Microsoft Dynamics CRM 외부 계정을 사용하면 Campaign 인스턴스를 Microsoft Dynamics CRM 외부 데이터베이스에 연결할 수 있습니다.

Adobe Campaign 웹 사용자 인터페이스에서 Microsoft Dynamics CRM 외부 계정을 구성합니다.

1. [외부 계정을 만들고](external-account.md) **[!UICONTROL 외부 데이터베이스]**&#x200B;을(를) 외부 계정의 **[!UICONTROL 유형]**(으)로 선택하고 Microsoft Dynamics CRM을 **[!UICONTROL 공급자 유형]**(으)로 선택합니다.

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL Microsoft Dynamics CRM]** 외부 계정을 구성하려면 다음 필드를 채우십시오.

   ![Microsoft Dynamics CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-microsoft-1.png)

   +++ CRM OAuth 유형의 경우: 암호 자격 증명

   * **[!UICONTROL 서버]**: Microsoft CRM 서버의 URL을 입력하십시오.

     Microsoft CRM Server URL을 찾으려면 Microsoft Dynamics CRM 계정에 로그인하고 Dynamics 365를 선택한 다음 앱을 엽니다. 브라우저의 주소 표시줄에 서버 URL이 표시됩니다(예: `https://myserver.crm.dynamics.com/`).

   * **[!UICONTROL 계정]**: Microsoft CRM에 로그인하는 데 사용되는 계정을 지정합니다.

   * **[!UICONTROL 암호]**: 지정한 계정과 연결된 암호를 입력하십시오.

   * **[!UICONTROL 클라이언트 식별자]**: Microsoft Azure 관리 포털에 있는 클라이언트 ID를 입력하십시오.

   * **[!UICONTROL CRM 버전]**: Dynamics CRM 365 CRM 버전을 선택하십시오.

   +++

   </br>

   +++ CRM O-Auth 유형의 경우: 인증서

   * **[!UICONTROL 서버]**: Microsoft CRM 서버의 URL을 입력하십시오.

     Microsoft CRM Server URL을 찾으려면 Microsoft Dynamics CRM 계정에 로그인하고 Dynamics 365를 선택한 다음 앱을 엽니다. 브라우저의 주소 표시줄에 서버 URL이 표시됩니다(예: `https://myserver.crm.dynamics.com/`).

   * **[!UICONTROL 개인 키(Base64 인코딩)]**: Base64 형식으로 인코딩된 개인 키를 제공합니다.

     이렇게 하려면 Base64 인코더의 도움을 사용하거나 Linux용 명령줄 `base64 -w0 private.key`을(를) 사용합니다.

   * **[!UICONTROL 사용자 지정 키 식별자]**: 인증서에 사용되는 사용자 지정 키 식별자를 입력하십시오.

   * **[!UICONTROL 키 ID]**: 인증서와 연결된 키 ID를 입력하십시오.

   * **[!UICONTROL 클라이언트 식별자]**: Microsoft Azure 관리에서 찾은 클라이언트 ID를 입력하십시오.

   * **[!UICONTROL CRM 버전]**: Dynamics CRM 365 CRM 버전을 선택하십시오.

   +++

1. 연결을 설정한 후 **[!UICONTROL Microsoft CRM 구성 마법사]**&#x200B;에 액세스하여 Microsoft CRM 표 목록을 생성합니다.

   필요한 테이블을 선택하려면 **[!UICONTROL 다음]**&#x200B;을 클릭하세요.

   ![Microsoft Dynamics CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-microsoft-2.png)

1. **[!UICONTROL 테이블 레이블]** 및 **[!UICONTROL 테이블 내부 이름]**&#x200B;을(를) 지정하여 검색할 Microsoft CRM 테이블을 선택하거나 원격 테이블을 추가한 다음 **[!UICONTROL 선택됨]** 토글을 활성화합니다.

   **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

1. 선택한 테이블을 기반으로 Microsoft CRM 스키마를 만들려면 **[!UICONTROL 시작]**&#x200B;을 클릭하십시오.

1. 화면의 지침에 따라 Adobe Campaign 마케팅 기록 및 구독 관리의 페이지를 Microsoft Dynamics CRM에 직접 삽입합니다.

1. 마케팅 기록 페이지를 통합하기 위한 URL을 보려면 **[!UICONTROL 마케팅 기록 URL 표시]**&#x200B;를 클릭하고, 구독 관리 페이지를 통합하기 위한 URL을 보려면 **[!UICONTROL 잠재 고객 구독용 URL 표시]**&#x200B;를 클릭하십시오.

   ![Microsoft Dynamics CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-microsoft-3.png)

1. Microsoft CRM 외부 계정이 구성되면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

1. 이제 외부 계정이 만들어지면 **[!UICONTROL 열거형 동기화 중...]**&#x200B;을 클릭하여 Microsoft CRM에서 Adobe Campaign 웹 사용자 인터페이스로 열거형을 자동으로 동기화할 수 있습니다.

   ![Microsoft CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-microsoft-4.png)

1. Microsoft CRM 열거와 일치하는 Adobe Campaign 열거를 선택합니다.

   Adobe Campaign 값을 Microsoft CRM 값으로 바꾸려면 **[!UICONTROL 바꾸기]** 옵션을 활성화합니다.

## Salesforce {#salesforce}

Adobe Campaign에서 작동하도록 Salesforce 외부 계정을 구성하려면 다음 세부 정보를 제공해야 합니다.

1. [외부 계정을 만들고](external-account.md) **[!UICONTROL 외부 데이터베이스]**&#x200B;을(를) 외부 계정의 **[!UICONTROL 유형]**(으)로 선택하고 Salesforce.com을(를) **[!UICONTROL 공급자 유형]**(으)로 선택합니다.

   ![Salesforce 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-salesforce-1.png)

1. **[!UICONTROL 만들기]**&#x200B;를 클릭합니다.

1. **[!UICONTROL Salesforce]** 외부 계정을 구성하려면 다음 필드를 입력하십시오.

   * **[!UICONTROL CRM O-Auth 유형]**: **[!UICONTROL 암호 자격 증명]** 또는 **[!UICONTROL 자격 증명]**

   * **[!UICONTROL 계정]**: Salesforce CRM에 로그인하는 데 사용되는 계정입니다.

   * **[!UICONTROL 암호]**: 지정한 계정과 연결된 암호를 입력하십시오.

   * **[!UICONTROL 보안 토큰]**: 계정과 연결된 Salesforce 보안 토큰을 입력하십시오.

   * **[!UICONTROL API 버전]**: 버전 49를 선택합니다.

   ![Salesforce 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-salesforce-2.png)

1. **[!UICONTROL Salesforce CRM 구성 마법사]**&#x200B;를 열어 Salesforce CRM 표 목록을 생성한 다음 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

   ![Salesforce CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-salesforce-3.png)

1. **[!UICONTROL 테이블 레이블]** 및 **[!UICONTROL 테이블 내부 이름]**&#x200B;을 입력하여 검색할 Salesforce 테이블을 선택하거나 원격 테이블을 추가한 다음 **[!UICONTROL 선택됨]** 토글을 활성화합니다.

   **[!UICONTROL 다음]**&#x200B;을 클릭합니다.

1. 선택한 테이블을 기반으로 Salesforce CRM 스키마를 만들려면 **[!UICONTROL 시작]**&#x200B;을 클릭하십시오.

1. **[!UICONTROL Salesforce 링크 만들기 마법사...]**&#x200B;를 클릭하여 Salesforce에서 웹 링크를 생성합니다.

   그런 다음 **[!UICONTROL 다음]**&#x200B;을(를) 클릭하여 Salesforce에서 **리드** 및 **연락처**&#x200B;에 대한 웹 링크를 검색합니다.

1. Salesforce 웹 링크 목록으로 내보낼 링크를 선택합니다.

1. 화면의 지침에 따라 Adobe Campaign 웹 사용자 인터페이스에서 Salesforce CRM으로 **마케팅 기록** 및 **구독 관리** 페이지를 삽입하십시오.

1. Salesforce CRM 외부 계정이 구성되면 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

1. 이제 외부 계정이 만들어지면 **[!UICONTROL 열거형 동기화 중...]**&#x200B;을 클릭하여 Salesforce에서 Adobe Campaign 웹 사용자 인터페이스로 자동으로 열거형을 동기화할 수 있습니다.

   ![Salesforce CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-salesforce-4.png)

1. Salesforce 열거와 일치하는 Adobe Campaign 열거를 선택합니다.

   Adobe Campaign 값을 Salesforce 값으로 바꾸려면 **[!UICONTROL 바꾸기]** 옵션을 활성화합니다.

   ![Salesforce CRM 외부 계정 구성 필드를 보여주는 스크린샷입니다.](assets/crm-salesforce-5.png)

