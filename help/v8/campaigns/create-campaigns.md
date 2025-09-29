---
audience: end-user
title: Adobe Campaign Web을 사용하여 캠페인 만들기
description: Adobe Campaign Web을 사용하여 크로스 채널 캠페인을 구축하는 방법 알아보기
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 36%

---

# 첫 캠페인 만들기 {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="캠페인 생성 속성"
>abstract="이 화면에서 캠페인 설정을 정의합니다. 템플릿을 선택하고 캠페인 레이블을 입력합니다. 추가 설정을 찾아 기본 내부 이름, 폴더를 변경하고, 설명을 추가하고, 할당자를 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="캠페인 속성"
>abstract="이 화면에서 캠페인 설정(레이블, 내부 이름, 폴더, 설명)을 확인하고 업데이트할 수 있습니다. 어떤 사용자에게 할당되었는지도 확인할 수 있습니다."

새 캠페인을 만들려면 해당 설정 및 일정을 정의하고 워크플로우 및 게재를 포함하십시오.

## 캠페인 만들기 {#campaign-create}

새 캠페인을 만들려면 다음 단계를 수행합니다.

1. **[!UICONTROL 캠페인]** 메뉴를 클릭하고 **[!UICONTROL 캠페인 만들기]** 단추를 클릭합니다.

   ![캠페인 메뉴의 &quot;캠페인 만들기&quot; 단추를 표시하는 스크린샷](assets/create-campaign-button.png)

1. 사용할 **템플릿**&#x200B;을(를) 선택하고 캠페인 레이블을 제공하십시오. [자세히 보기](manage-campaigns.md#manage-campaign-templates)
1. 필요한 경우 **추가 옵션**&#x200B;을 변경합니다. 내부 이름, 폴더, 할당자, 설명 및 특성입니다.
1. 캠페인의 **일정**&#x200B;을(를) 정의합니다. [이 섹션](#campaign-schedule)에서 캠페인 일정을 설정하는 방법을 알아보세요.
1. **만들기**&#x200B;를 클릭합니다.

   ![내부 이름, 폴더, 피할당자, 설명 및 특성에 대한 필드를 포함하여 캠페인 속성 화면을 보여주는 스크린샷입니다.](assets/create-a-campaign-properties.png)

1. 캠페인에 워크플로우 및 게재 추가:

   * **워크플로** 탭에서 **워크플로 만들기**&#x200B;를 클릭합니다. 캠페인을 만들 때 기본 워크플로우가 자동으로 추가됩니다. [워크플로를 만드는 방법](../workflows/create-workflow.md)에 대해 자세히 알아보세요.

   * **게재** 탭에서 **게재 만들기**&#x200B;를 클릭합니다. [자세히 알아보기](../msg/gs-messages.md)

## 캠페인 모니터링 및 추적 {#campaign-monitoring}

캠페인 모니터링은 캠페인의 효과를 분석하는 주요 단계입니다. 캠페인을 열고 **로그** 단추를 클릭합니다.

**보고서** 단추를 클릭하여 전용 보고서를 볼 수도 있습니다. 이 [섹션](../reporting/campaign-reports.md)을 참조하십시오.

## 캠페인 일정 정의 {#campaign-schedule}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="캠페인 예약"
>abstract="캠페인 일정을 선택합니다. 캠페인을 만들 수 있으며 시작 날짜가 되면 캠페인이 시작됩니다. 기본적으로 캠페인 시작 날짜는 생성일이며 5일 동안 지속됩니다. 시작 일자와 종료 일자는 캠페인 목록에 표시되고 필터로 사용할 수 있습니다."

시작 날짜에 도달하면 캠페인이 시작됩니다. 시작 날짜에 도달하지 않은 한 캠페인은 **[!UICONTROL 초안]** 상태입니다. 시작 날짜에 도달하면 **[!UICONTROL 진행 중]**(으)로 바뀝니다. 종료 날짜에 도달하면 캠페인이 **[!UICONTROL 완료됨]**(으)로 설정됩니다.

시작 및 종료 날짜가 캠페인 목록에 표시되며 필터로 사용할 수 있습니다. 이 [섹션](manage-campaigns.md#access-campaigns)을 참조하십시오.

>[!NOTE]
>
>나중에 캠페인 레이블 옆에 있는 **캠페인 설정 구성** 아이콘을 통해 이러한 속성을 수정할 수 있습니다. 이 [섹션](gs-campaigns.md#campaign-dashboard)을 참조하십시오.

날짜에 도달하면 워크플로우의 컨텍스트에서 해당 캠페인에서 만들어지고 전송할 준비가 된 게재가 실제로 전송됩니다. 이 경우 워크플로우가 시작되었어야 합니다.

<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.
-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header

About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and helps you organize your marketing activities: you can separate them by country, by brand, by unit, and similar criteria.

A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.

To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

* Timeline
* About dynamic reports
* Creating a campaign

In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card, and access a program or sub-program.

Click on the Create button, and select Campaign.

In the Creation mode screen, select a campaign type.

The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date for your campaign. These dates only apply to the campaign itself.

Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

>[!NOTE]
>
>Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.

Programs and campaigns icons and statuses:

Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

* Gray: the program/campaign has not yet started - Editing status.
* Blue: the program/campaign is in progress - In progress status.
* Green: the program/campaign has finished - Finished status.

By default, the current date is automatically shown as the validity start date, and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.

Business.Adobe.com resources
-->