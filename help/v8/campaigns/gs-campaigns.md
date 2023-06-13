---
audience: end-user
title: 캠페인 시작하기
description: 크로스 채널 캠페인 시작 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
exl-id: f2b9f8e6-5ded-4a47-89e9-96650cd78229
source-git-commit: 7daead11e097f6179c99adb0e9496dec567cb29a
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 10%

---


# 캠페인 시작하기 {#campaigns}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="크로스채널 캠페인 디자인 및 보내기"
>abstract="Adobe Campaign 기능을 사용하면 중앙 집중식 고객 데이터를 관리하고, 고객 커뮤니케이션 및 캠페인을 디자인하며, 이메일, 푸시 및 SMS와 같은 다양한 채널에서 개인화된 경험을 만들 수 있습니다."

Adobe Campaign을 사용하면 내장된 캠페인 관리 기능을 사용하여 타깃팅된 마케팅 이니셔티브를 손쉽게 오케스트레이션할 수 있습니다. 일정을 정의하는 기능을 통해 캠페인 기간 및 타이밍을 계획하여 전략적 목표에 부합하고 대상자 참여를 극대화할 수 있습니다.

캠페인과 관련된 워크플로우 및 게재를 여러 개 추가하여 다양한 채널에 개인화된 경험을 만들어 각 터치포인트가 의도한 대상과 공감하도록 할 수 있습니다.

캠페인은 전용 보고 지표를 제공하여 전체 캠페인의 성과에 대한 포괄적인 통찰력을 얻으므로, 캠페인의 효과를 평가하고, 트렌드를 식별하며, 데이터 중심의 결정을 내려 향후 노력을 최적화할 수 있습니다.

<!--
Use Adobe Campaign to create cross-channel campaigns. With its marketing campaign orchestration capabilities, you can manage and centralize customer data, design customer communications and campaigns, and create personalized experiences across different channels. In this version, email, push and SMS channels are available.

Design and execute high-volume email campaigns to deliver personalized messages, for all platforms and screen sizes. 
Measure the effectiveness of your deliveries with detailed reports including the counts of opens, clicks, forwards, and more. With Adobe Campaign segmentation capabilities, you can run queries against a high-volume database, and easily define dynamic marketing segments which perfectly target your campaigns.
-->

<!--
Get Started with campaigns
Adobe Campaign offers a set of solutions that help you personalize and deliver campaigns across all of your online and offline channels. You can create, configure, execute and analyze marketing campaigns. All marketing campaigns can be managed from a unified control center. Discover how to browse and create marketing campaigns in this section.

Campaigns include actions (deliveries) and processes (importing or extracting files), as well as resources (marketing documents, delivery outlines). They are used in marketing campaigns. Campaigns are part of a program, and programs are included in a campaign plan.
-->

## 캠페인 액세스 및 관리{#access-campaigns}

새 캠페인을 만들거나 기존 캠페인을 관리하려면 **[!UICONTROL 캠페인]** 메뉴 아래의 제품에서 사용할 수 있습니다. 다음 두 가지 탭을 사용할 수 있습니다.

* 다음 **찾아보기** 탭에는 기존 캠페인이 모두 나열됩니다. 캠페인을 클릭하여 대시보드를 열거나 다음을 클릭하여 새 캠페인을 만들 수 있습니다. **캠페인 만들기** 단추를 클릭합니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오

* 다음 **템플릿** 탭에는 사용 가능한 모든 캠페인 템플릿이 나열됩니다. 캠페인 템플릿은 새 캠페인을 만드는 데 다시 사용할 수 있도록 사전 구성되어 있습니다. 클라이언트 콘솔에서 만들어집니다. [자세히 보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=ko).

목록의 각 캠페인에는 현재 상태, 만든 날짜, 마지막으로 수정한 시간 등에 대한 정보가 표시됩니다.

다음을 클릭하여 표시된 열을 사용자 지정할 수 있습니다. **사용자 지정 레이아웃에 대한 열 구성** 아이콘은 목록의 오른쪽 위 모서리에 있습니다. 이렇게 하면 목록에 추가 정보를 추가할 수 있습니다. 또한 검색 창과 필터를 사용하여 목록 내에서 손쉽게 검색할 수 있습니다. [자세히 알아보기](../get-started/user-interface.md#list-screens)

예를 들어 캠페인 일정을 필터링할 수 있습니다. 필터 패널을 열고 다음을 사용합니다. **시작 - 종료 날짜** 섹션:

![캠페인 목록](assets/campaign-filter-on-dates.png)

## 캠페인 대시보드{#campaign-dashboard}

다음에서 **찾아보기** 캠페인 목록의 탭에서 캠페인을 클릭하여 대시보드를 표시합니다. 다음 두 가지 탭을 사용할 수 있습니다.

* 다음 **워크플로** 탭에는 캠페인에 연결된 모든 워크플로가 나열됩니다. 이 탭에서는 캠페인 내에 새 워크플로우를 만들 수도 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오
* 다음 **게재** 탭에는 캠페인에 연결된 모든 게재가 나열됩니다. 캠페인 내에 새 게재를 만들 수도 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오

다음 **캠페인 설정 구성** 아이콘을 사용하면 캠페인을 생성할 때 정의된 캠페인 속성을 수정할 수 있습니다. 이 [섹션](create-campaigns.md#create-campaigns)을 참조하십시오

