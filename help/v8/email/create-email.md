---
audience: end-user
title: 첫 번째 이메일 보내기
description: Campaign Web UI를 사용하여 첫 번째 전자 메일을 보내는 방법을 배웁니다
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 871737ba2ab444eaaafde2a3822879629d956e1c
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 0%

---

# 첫 번째 이메일 보내기 {#first-email}

![](../assets/do-not-localize/badge.png)

이 사용 사례에서 첫 번째 타겟팅된 이메일을 만드는 방법을 알아봅니다. 은 및 골드 충성도 고객에게 특정 날짜에 전자 메일 전송을 예약합니다.

사전 정의된 디자인 템플릿을 사용하면 고객 프로필 속성을 기반으로 개인화된 컨텐츠도 이메일에 제공합니다.

![](assets/delivery-list.png)

## 이메일 만들기 {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="이메일 템플릿 선택"
>abstract="템플릿은 Adobe Campaign v8 콘솔에서 정의됩니다. 유형화 규칙, 개인화 또는 라우팅 매개 변수와 같은 사전 정의된 매개 변수를 포함하는 특정 게재 구성입니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="전자 메일 속성"
>abstract="속성은 게재 이름을 지정하고 분류하는 데 도움이 되는 일반적인 게재 매개 변수입니다. 게재가 Adobe Campaign v8 콘솔에 정의된 확장 스키마를 기반으로 하는 경우, 일부 특정 **사용자 지정 옵션** 필드를 사용할 수 있습니다."

1. 새 게재를 만들려면 다음 위치로 이동하십시오. **[!UICONTROL 게재]** 메뉴 및 선택 **[!UICONTROL 이메일]** 를 채널로 설정합니다.

1. 사용할 템플릿을 선택하고 을(를) 클릭합니다 **[!UICONTROL 게재 만들기]**.

   >[!NOTE]
   >
   >템플릿은 나중에 사용할 수 있도록 저장된 사전 구성된 게재 설정입니다. Adobe Campaign 콘솔에서 관리 사용자가 만들 수 있습니다. [게재 템플릿으로 작업하는 방법 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. 이메일에 대한 레이블을 제공하고 필요에 따라 추가 옵션을 구성합니다.

   * **[!UICONTROL 내부 이름]**: 게재에 고유 식별자를 할당하고
   * **[!UICONTROL 폴더]**: 게재를 특정 폴더에 저장,
   * **[!UICONTROL 배달 코드]**: 이 필드를 사용하여 고유한 명명 규칙에 따라 게재를 구성할 수 있습니다.
   * **[!UICONTROL 설명]**: 게재에 대한 설명을 지정합니다.
   * **[!UICONTROL 자연]**: 분류 목적으로 이메일의 특성을 지정합니다.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >특정 사용자 지정 필드로 스키마를 확장한 경우, **[!UICONTROL 사용자 지정 옵션]** 섹션을 참조하십시오.

   ![](assets/email-properties.png)

   또한 유형화 규칙 및 타겟 매핑과 같은 고급 설정은 게재 이름 옆에 있는 버튼을 클릭하여 액세스할 수 있습니다. 이러한 설정은 선택한 템플릿에서 미리 구성되지만 필요에 따라 특정 전자 메일에 대해 편집할 수 있습니다.

## 이메일 콘텐츠 만들기 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="이메일 콘텐츠를 디자인하는 방법 알아보기"
>abstract="이메일 디자이너를 사용하는 방법을 알아보십시오."

이 사용 사례에서는 사전 정의된 템플릿을 사용하여 이메일을 디자인합니다.

사전 정의된 템플릿을 사용하여 이메일을 디자인하려고 합니다. 전자 메일 콘텐츠 구성에 대한 자세한 지침은 [이 섹션](../content/edit-content.md).

1. 전자 메일 콘텐츠 만들기를 시작하려면 **[!UICONTROL 컨텐츠 편집]** 버튼을 클릭합니다.

   이렇게 하면 이메일 콘텐츠를 구성하고 이메일 디자이너를 사용하여 디자인할 수 있는 전용 인터페이스로 이동합니다.

   ![](assets/edit-content.png)

1. 이메일의 제목란을 입력하고 표현식 편집기를 사용하여 개인화합니다. [콘텐츠를 개인화하는 방법 알아보기](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. 전자 메일 본문을 디자인하려면 **[!UICONTROL 이메일 본문 편집]** 버튼을 클릭합니다.

   이메일 콘텐츠를 만드는 데 사용할 방법을 선택합니다. 이 예제에서는 사전 정의된 디자인 템플릿을 사용합니다.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. 템플릿을 선택하면 이메일 디자이너에 표시되며, 여기에서 필요한 편집 및 개인화를 추가할 수 있습니다.

   예를 들어 이메일 제목에 개인화를 추가하려면 구성 요소 블록을 선택하고 **[!UICONTROL 개인화 추가]**.

   ![](assets/add-perso.png)

1. 콘텐츠에 만족하면 디자인을 저장하고 닫습니다. 클릭 **[!UICONTROL 저장]** 전자 메일 만들기 화면으로 돌아갑니다.

   ![](assets/save-content.png)

## 대상자 정의 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="대상자 정의"
>abstract="마케팅 메시지에 가장 적합한 대상을 선택합니다. Campaign v8 인스턴스 또는 Adobe Experience Platform에서 이미 정의된 기존 대상을 선택하거나, 규칙 빌더로 새 대상을 만들도록 선택할 수 있습니다."

이 사용 사례에서는 기존 대상자에게 이메일을 보냅니다. 대상 사용 방법에 대한 추가 지침은 [이 섹션](../audience/about-audiences.md).

1. 전자 메일 대상자를 선택하려면 **[!UICONTROL 대상 선택]** 버튼을 클릭하고 목록에서 기존 대상자를 선택합니다.

   이 예에서는 은 및 골드 충성도 포인트 수준에 속하는 고객을 타깃팅하는 기존 대상을 사용하려고 합니다.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >목록에서 사용할 수 있는 대상은 Campaign V8 인스턴스나 대상/소스 통합이 인스턴스에 구성된 경우 Adobe Experience Platform에서 가져옵니다.
   >
   >대상/소스 통합을 사용하면 Experience Platform 세그먼트를 Adobe Campaign에 보내고, 캠페인 게재 및 추적 로그를 Adobe Experience Platform에 보낼 수 있습니다. [Campaign과 Adobe Experience Platform을 함께 사용하는 방법 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. 대상자를 선택하면 추가 규칙을 적용하여 타겟을 세분화할 수 있습니다.

   타겟팅되지 않은 사용자와 비교하여 전자 메일 수신자의 동작을 분석하도록 컨트롤 그룹을 설정할 수도 있습니다. [컨트롤 그룹 작업 방법 알아보기](../audience/control-group.md)

   ![](assets/audience-selected.png)

## 전송을 예약합니다 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="전송을 예약합니다"
>abstract="보내는 날짜와 시간을 정의합니다. 마케팅 메시지에 가장 적합한 시간을 선택하면 공개 비율을 최대화할 수 있습니다."

전자 메일 전송을 예약하려면 를 클릭합니다. **[!UICONTROL 활성화]** 원하는 전송 날짜 및 시간을 설정합니다.

기본적으로 **[!UICONTROL 보내기 전 확인]** 옵션이 활성화되어 있으면 예약된 날짜 및 시간에 이메일을 전송하기 전에 전송을 확인해야 합니다. 예약된 날짜와 시간에 자동으로 이메일을 보내려면 이 옵션을 비활성화할 수 있습니다.

![](assets/schedule.png)

## 이메일 미리 보기 및 테스트 {#preview-test}

전자 메일을 보내기 전에 미리 보고 테스트하여 본인의 기대에 부합하는지 확인할 수 있습니다.

이 사용 사례에서는 타겟팅된 프로필 중 일부를 가장하는 동안 이메일을 미리 보고 테스트 버전을 특정 이메일 주소로 보냅니다.

전자 메일을 미리 보고 테스트하는 방법에 대한 추가 정보는 [이 섹션](../preview-test/preview-test.md).

1. 전자 메일을 검토하고 보내려면 **[!UICONTROL 검토 및 보내기]**. 구성된 모든 속성, 대상 및 일정과 함께 이메일 미리 보기가 표시됩니다. 수정 단추를 클릭하여 이러한 요소를 편집할 수 있습니다.

1. 이메일을 미리 보고 테스트 버전을 보내려면 **[!UICONTROL 컨텐츠 시뮬레이션]** 버튼을 클릭합니다. 그러면 미리 보기 인터페이스가 열립니다.

   ![](assets/review-email.png)

1. 왼쪽에서 이메일을 미리 보는 데 사용할 프로필을 선택합니다.

   오른쪽 창에는 선택한 프로필에 따라 전자 메일 미리 보기가 표시됩니다. 여러 개의 프로필을 추가한 경우 프로필 간을 전환하여 해당 이메일을 미리 볼 수 있습니다.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. 전자 메일의 테스트 버전을 보내려면 **[!UICONTROL 테스트]** 그런 다음 사용할 모드를 선택합니다.

   이 예제에서는 **[!UICONTROL 기본 대상에서 대체]** 모드에서는 이메일에 타겟팅된 프로필 중 일부를 가장하는 동안 테스트 버전을 특정 이메일 주소로 보냅니다.

   ![](assets/proof-mode.png)

1. 클릭 **[!UICONTROL 주소 추가]** 및 테스트 버전을 받을 이메일 주소를 지정합니다.

   각 이메일 주소에 대해 가장할 프로필을 선택합니다. Adobe Campaign에서 타겟에서 임의의 프로필을 선택하도록 할 수도 있습니다.

   ![](assets/proof-test-profile.png)

1. 클릭 **[!UICONTROL 테스트 전자 메일 보내기]** 전송을 확인합니다.

   테스트 버전은 와 함께 선택한 프로필을 사용하여 지정된 이메일 주소로 전송됩니다 **[증명 x]** 접두사를 사용합니다.

   ![](assets/proof-sent.png)

   을(를) 클릭하여 언제든지 전송된 테스트 이메일에 전송 상태를 확인하고 액세스할 수 있습니다 **[!UICONTROL 테스트 전자 메일 로그 보기]** 단추 클릭.

## 이메일 보내기 및 모니터링 {#prepare-send}

이메일을 검토하고 테스트한 후 준비를 시작하고 보낼 수 있습니다.

1. 전자 메일 준비를 시작하려면 **[!UICONTROL 준비]**. [이메일 준비 방법 알아보기](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. 전자 메일을 보낼 준비가 되면 **[!UICONTROL 보내기]** 버튼(또는 **[!UICONTROL 예약된 대로 보내기]** 전송을 예약한 경우) 및 전송을 확인합니다.

1. 전송 프로세스 중에 진행 상황을 추적하고 통계를 이 화면에서 직접 실시간으로 볼 수 있습니다.

   ![](assets/sent-mail.png)

   을 클릭하여 전송에 대한 세부 정보에 액세스할 수도 있습니다 **[!UICONTROL 로그]** 버튼을 클릭합니다. [게재 로그를 모니터링하는 방법 알아보기](../monitor/delivery-logs.md)

1. 이메일이 전송되면 추가 분석을 위해 전용 보고서에 액세스할 수 있는 **[!UICONTROL 보고]** 버튼을 클릭합니다.

![](assets/reports.png)
