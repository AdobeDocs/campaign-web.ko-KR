---
audience: end-user
title: Adobe Campaign Web을 사용하여 캠페인 만들기
description: Adobe Campaign Web을 사용하여 크로스 채널 캠페인을 구축하는 방법 알아보기
badge: label="알파"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 22%

---


# 첫 캠페인 만들어 보기 {#create-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="캠페인 생성 속성"
>abstract="캠페인에 대한 속성 및 메타데이터를 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="캠페인 속성"
>abstract="캠페인 설정 및 메타데이터를 정의합니다."

캠페인에는 워크플로우 및 독립 실행형 게재가 포함될 수 있습니다. 속성, 일정, 작업, deliv 플러스 공정한 일정

## 캠페인 만들기

새 캠페인을 만들려면 다음 단계를 수행합니다.

1. 다음을 클릭합니다. **[!UICONTROL 캠페인]** 메뉴를 클릭하고 **[!UICONTROL 캠페인 만들기]** 단추를 클릭합니다.
1. 다음 항목 선택 **템플릿** 을 입력하여 캠페인에 대한 레이블을 제공합니다. 캠페인 템플릿은 새 캠페인을 만드는 데 다시 사용할 수 있도록 사전 구성되어 있습니다. 클라이언트 콘솔에서 만들어집니다.
   [자세히 보기](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=ko).
1. 필요한 경우 다음을 변경할 수 있습니다 **추가 옵션**: 내부 이름, 폴더, 할당자, 설명 및 특성.
1. 다음을 정의합니다. **예약** 을 참조하십시오. 시작 날짜에 도달하면 캠페인이 시작됩니다. 시작 및 종료 날짜가 캠페인 목록에 표시되며 필터로 사용할 수 있습니다. 이 [섹션](manage-campaigns.md#access-campaigns)을 참조하십시오.

   ![캠페인 속성 정의](assets/campaign-properties.png)

   >[!NOTE]
   >
   >나중에 **캠페인 설정 구성** 아이콘, 캠페인 레이블 옆에 있습니다. 이 [섹션](gs-campaigns.md#campaign-dashboard)을 참조하십시오

1. Click **Create**.
1. 캠페인에 워크플로우 및 게재 추가:

   * 다음에서 **워크플로** 탭을 클릭하고 **워크플로우 만들기**. 캠페인을 만들 때 기본 워크플로우가 자동으로 추가됩니다. 방법에 대한 자세한 내용 [워크플로우 만들기](../workflows/create-workflow.md)
   * 다음에서 **게재** 탭을 클릭하고 **게재 만들기**. [자세히 알아보기](../msg/gs-messages.md)

1. 사용 **로그** 및 **보고** 캠페인의 성과를 분석하는 단추입니다.

## 캠페인 모니터링 및 추적{#campaign-monitoring}

캠페인 모니터링은 캠페인을 분석하는 주요 단계입니다. 캠페인을 열고 **로그** 단추를 클릭합니다.

다음을 클릭하여 전용 보고서를 볼 수도 있습니다. **보고서** 단추를 클릭합니다. 이 [섹션](../reporting/campaign-reports.md)을 참조하십시오.

+++WORKF ++화면

<!--
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
