---
title: Adobe Campaign 웹 인터페이스에 연결
description: Adobe Campaign Web 사용자 인터페이스에 접속하는 방법 알아보기
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
source-git-commit: 8006eeb6088d7d6ef99f374b2b846978cd679c01
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 68%

---

# Adobe Campaign에 연결 {#connect-to-campaign}

Experience Cloud는 Adobe의 디지털 마케팅 애플리케이션, 제품 및 서비스 통합 제품군입니다. 직관적인 인터페이스에서 클라우드 애플리케이션, 제품 기능, 서비스에 빠르게 액세스할 수 있습니다. 이 페이지에서 Adobe Experience Cloud에 연결하고 Adobe Campaign 웹 인터페이스에 액세스하는 방법을 알아봅니다.

## Adobe Experience Cloud에 로그인 {#sign-in-to-exc}

SSO(Single Sign-On)만 사용하여 Campaign에 접속할 수도 있습니다. 보통은 Experience Cloud 관리자가 애플리케이션 및 서비스에 대한 액세스 권한을 부여합니다. Experience Cloud 초대 이메일에 나온 단계를 따르면 됩니다.

Adobe Experience Cloud에 로그인하려면 다음 기본 단계를 따르십시오.

1. [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}로 이동합니다.

1. Adobe ID 또는 Enterprise ID를 사용하여 로그인합니다. [이 문서](https://helpx.adobe.com/kr/enterprise/using/identity.html){target="_blank"}에서 Adobe의 ID 유형에 대해 자세히 알아보세요.

   Experience Cloud에 로그인하면 모든 솔루션 및 앱에 빠르게 액세스할 수 있습니다.

   ![Adobe Experience Cloud 홈 페이지를 보여주는 스크린샷](assets/exc-home.png){zoomable="yes"}

1. 올바른 조직에 속해 있는지 확인하십시오.

   ![Adobe Experience Cloud에서 조직 선택을 보여 주는 스크린샷](assets/exc-orgs.png){zoomable="yes"}{width="50%" align="left"}

   [이 문서](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=ko){target="_blank"}에서 Adobe Experience Cloud의 조직에 대해 자세히 알아보세요.

## Adobe Campaign 액세스 {#access-to-campaign}

Campaign 환경에 액세스하려면 Adobe Experience Cloud 홈페이지의 **빠른 액세스** 섹션에서 **캠페인**&#x200B;을 선택합니다.

다른 Adobe Experience Cloud 솔루션에 이미 연결되어 있는 경우 화면 오른쪽 상단의 솔루션 전환기에서 Campaign 환경으로 이동합니다.

![Adobe Experience Cloud에서 솔루션 전환기를 보여 주는 스크린샷](assets/solution-switcher.png){zoomable="yes"}

Campaign 컨트롤 패널을 포함한 여러 환경에 액세스할 수 있는 경우 적절한 인스턴스의 **시작** 버튼을 클릭합니다.

![Adobe Campaign의 시작 단추를 표시하는 스크린샷](assets/launch-campaign.png){zoomable="yes"}

이제 Campaign에 연결되었습니다. [이 페이지](user-interface.md)에서 사용자 인터페이스 사용 방법에 대해 알아보십시오.

### 액세스 제어 {#access-control}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="권한 필요"
>abstract="오브젝트를 만들려면 먼저 관리자가 권한을 부여해야 합니다."

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="이 대상자는 읽기 전용입니다."
>abstract="이 대상자를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="이 서비스는 읽기 전용입니다."
>abstract="이 서비스를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="수신자 읽기 전용 프로필"
>abstract="이 프로필을 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="이 캠페인은 읽기 전용입니다."
>abstract="이 캠페인을 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="이 게재는 읽기 전용입니다."
>abstract="이 게재를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="이 워크플로는 읽기 전용입니다."
>abstract="이 워크플로를 편집할 권한이 없습니다. 필요한 경우 관리자에게 액세스 권한을 요청하십시오."

액세스 제어는 게재, 수신자 또는 워크플로와 같은 기본 목록의 개체 및 데이터에 대한 액세스를 제한합니다. 이러한 제한 사항은 Explorer의 탐색 트리에도 적용됩니다. 또한 사용자 인터페이스에서 오브젝트를 생성, 삭제, 복제 및 편집하려면 권한이 필요합니다.

Campaign 웹의 모든 권한은 Campaign 클라이언트 콘솔 권한과 동기화됩니다. Campaign 관리자만 사용자 권한을 정의하고 수정할 수 있습니다.

Campaign 웹 사용자 인터페이스를 검색할 때 사용 권한에 따라 데이터, 개체 및 기능에 액세스할 수 있습니다. 예를 들어 폴더에 대한 액세스 권한이 없으면 해당 폴더를 볼 수 없습니다. 권한은 오브젝트 및 데이터 관리에도 영향을 미칩니다. 특정 폴더에 대한 쓰기 권한이 없으면 사용자 인터페이스에서 표시되더라도 해당 폴더에서 게재를 생성할 수 없습니다.

[여기에서 권한을 조회하고 관리](permissions.md)하는 방법을 알아볼 수 있습니다.

## Adobe Experience Cloud 상단 탐색 {#top-bar}

인터페이스의 상단 막대를 탐색하여 다음과 같은 작업을 수행할 수 있습니다.

* Campaign 웹 사용자 인터페이스에 대한 피드백을 공유합니다.
* 조직 간에 전환합니다.
* Adobe Experience Cloud 솔루션과 앱 간을 전환합니다.
* [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=ko){target="_blank"}에서 도움말을 검색합니다.
* 제품 알림을 확인합니다.
* Adobe 프로필을 편집하고 [좋아하는 언어를 업데이트](#language-pref) 또는 [밝은 테마/어두운 테마로 전환](#dark-theme)과 같은 설정을 관리합니다.

![Adobe Experience Cloud 상단 탐색 모음을 표시하는 스크린샷](assets/do-not-localize/unified-shell.png){zoomable="yes"}{width="50%" align="left"}

## 지원되는 브라우저 {#browsers}

Adobe Campaign Web은 최신 버전의 Google Chrome, Safari 및 Microsoft Edge에서 최적으로 작동하도록 디자인되었습니다. 이전 버전 또는 다른 브라우저에서 특정 기능을 사용하는 데 문제가 발생할 수 있습니다.

## 언어 환경 설정 {#language-pref}

Adobe Campaign Web은 현재 다음 언어로 제공됩니다.

* 영어(미국) - EN-US
* 프랑스어 - FR
* 독일어 - DE
* 이탈리아어 - IT
* 스페인어 - ES
* 포르투갈어(브라질) - PTBR
* 일본어 - JP
* 한국어 - KR
* 중국어 간체 - CHS
* 중국어 번체 - CHT

Campaign Web의 기본 언어는 사용자 프로필에 지정된 기본 언어에 따라 결정됩니다. Campaign 서버 및 클라이언트 콘솔의 언어와 관련이 없습니다.

언어를 변경하려면 다음 작업을 수행하십시오.

1. 오른쪽 상단의 프로필 아이콘을 클릭한 다음 **환경 설정**&#x200B;을 선택합니다.
1. 이메일 주소 아래에 표시된 언어 링크를 클릭합니다.
1. 원하는 언어를 선택하고 **저장**&#x200B;을 클릭합니다. 사용 중인 구성 요소가 첫 번째 언어로 현지화되어 있지 않은 경우 두 번째 언어를 선택할 수 있습니다.


## 어두운 테마 및 밝은 테마 {#dark-theme}

Adobe Campaign은 밝은 테마와 어두운 테마로 제공됩니다. 기본적으로 사용자 인터페이스는 밝은 테마로 활성화됩니다. 어두운 테마로 전환하려면 프로필 아이콘을 클릭하고 **어두운 테마** 전환을 사용하여 활성화하거나 비활성화합니다.

사용자 프로필 설정 및 계정 환경 설정은 [이 섹션](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=ko#preferences){target="_blank"}에서 자세히 설명합니다.

Experience Cloud 중앙 인터페이스 구성 요소에 대한 자세한 내용은 [이 설명서](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=ko){target="_blank"}를 참조하십시오.