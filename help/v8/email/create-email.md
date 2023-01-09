---
audience: end-user
title: 첫 번째 이메일 만들기
description: Campaign v8 웹 설명서
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 4bc12928a6dac79d09f918a0bc34e3f98d9984d3
workflow-type: tm+mt
source-wordcount: '1174'
ht-degree: 2%

---

# 첫 번째 이메일 보내기 {#first-email}

>[!NOTE]
>
>이 설명서는 개발 중이며 자주 업데이트됩니다. 이 컨텐츠의 최종 버전은 2023년 1월에 준비될 예정입니다.

이 사용 사례에서는 첫 번째 이메일을 만드는 방법을 설명합니다. 은 및 골드 충성도 고객에게 특정 날짜에 전자 메일 전송을 예약하려고 합니다. 이 이메일은 사전 정의된 템플릿을 사용하여 디자인되며 프로필의 속성을 사용한 개인화를 포함합니다.

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

1. 에서 새 게재를 만듭니다. **[!UICONTROL 게재]** 메뉴 아래의 제품에서 사용할 수 있습니다.

1. 을(를) 선택합니다 **[!UICONTROL 이메일]** 채널과 사용할 템플릿을 클릭한 다음 **[!UICONTROL 만들기]**.

   >[!NOTE]
   >
   >템플릿은 다시 사용하기 위해 템플릿으로 저장된 특정 게재 구성입니다. 게재 템플릿은 Adobe Campaign 콘솔에서 관리 사용자가 구성합니다. [게재 템플릿으로 작업하는 방법 알아보기](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-delivery-templates/about-templates.html?lang=ko){target=&quot;_blank&quot;}

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

   또한 고급 설정(유형화 규칙, 타겟 매핑 등)은 게재 이름 옆에 있는 버튼을 통해 을(를) 사용할 수 있습니다. 템플릿은 이메일을 만들 때 선택한 템플릿에서 미리 정의됩니다. 필요한 경우 편집할 수 있습니다.

## 이메일 콘텐츠 만들기 {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="이메일 디자이너를 사용하여 이메일 콘텐츠를 디자인하는 방법을 알아보십시오."
>abstract="콘텐츠를 디자인하는 방법 알아보기"

이 사용 사례에서는 사전 정의된 템플릿을 사용하여 이메일을 디자인하려고 합니다. 전자 메일 콘텐츠를 구성하는 방법에 대한 자세한 내용은 [이 섹션](../content/edit-content.md).

1. 을(를) 클릭합니다. **[!UICONTROL 컨텐츠 편집]** 전자 메일 콘텐츠 만들기를 시작하는 단추입니다.

   이 화면에서 이메일 콘텐츠를 구성하고 이메일 디자이너를 사용하여 디자인할 수 있습니다.

   ![](assets/edit-content.png)

1. 이메일의 제목을 지정하고 표현식 편집기를 사용하여 개인화합니다. [콘텐츠를 개인화하는 방법 알아보기](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. 을(를) 클릭합니다. **[!UICONTROL 이메일 본문 편집]** 전자 메일 콘텐츠를 만들고 디자인하는 단추입니다.

   이메일 콘텐츠를 만드는 데 사용할 방법을 선택합니다. 이 예에서는 기존 디자인 템플릿을 사용하려고 합니다.

   ![](assets/import-html.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. 템플릿을 선택하면 이메일 디자이너에 표시되며, 필요한 경우 편집하고 개인화를 추가할 수 있습니다.

   이 예제에서는 이메일 제목에 개인화를 추가하려고 합니다. 이렇게 하려면 구성 요소 블록을 선택한 다음 를 클릭합니다. **[!UICONTROL 개인화 추가]**.

   ![](assets/add-perso.png)

1. 콘텐츠가 준비되면 저장한 다음 화살표를 클릭하여 이메일 만들기 화면으로 돌아갑니다.

   ![](assets/save-content.png)

## 대상자 정의 {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="대상자 정의"
>abstract="마케팅 메시지에 가장 적합한 대상을 선택합니다. Campaign v8 인스턴스나 Adobe Experience Platform에서 이미 정의된 기존 대상을 선택하거나, 세그먼트 빌더로 새 대상을 만들도록 선택할 수 있습니다."

이 사용 사례에서는 기존 대상자에게 이메일을 보내려고 합니다. 대상 작업 방법에 대한 자세한 내용은 [이 섹션](../audience/about-audiences.md).

1. 을(를) 클릭합니다. **[!UICONTROL 대상 선택]** 그런 다음 타깃팅할 기존 대상자를 선택합니다.

   이 예에서는 은 및 골드 충성도 포인트 수준에 속하는 고객을 타깃팅하는 기존 대상을 사용하려고 합니다.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >목록에서 사용할 수 있는 대상은 Campaign V8 인스턴스나 대상/소스 통합이 인스턴스에 구성된 경우 Adobe Experience Platform에서 가져옵니다.
   >
   >대상/소스 통합을 사용하면 Experience Platform 세그먼트를 Adobe Campaign에 보내고, 캠페인 게재 및 추적 로그를 Adobe Experience Platform에 보낼 수 있습니다. [Campaign과 Adobe Experience Platform을 함께 사용하는 방법 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html)

1. 대상자를 선택하면 추가 규칙을 사용하여 타겟을 세분화할 수 있습니다.

   타겟팅되지 않은 프로필의 동작과 비교하여 이메일 수신자의 동작을 분석하도록 컨트롤 그룹을 설정할 수도 있습니다. [컨트롤 그룹 작업 방법 알아보기](../audience/control-group.md)

## 전송을 예약합니다 {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="전송을 예약합니다"
>abstract="보내는 날짜와 시간을 정의합니다. 마케팅 메시지에 가장 적합한 시간을 선택하면 공개 비율을 최대화할 수 있습니다."

전자 메일 전송을 예약하려면 를 클릭합니다. **[!UICONTROL 활성화]** 그런 다음 전송할 날짜와 시간을 지정합니다.

기본적으로 **[!UICONTROL 보내기 전 확인]** 옵션이 활성화되어 있으면 즉, 지정된 날짜 및 시간에 이메일을 보낼 수 있도록 전송을 확인해야 합니다. 확인 없이 예약된 날짜 및 시간에 이메일을 보낼 수 있도록 하려면 이 옵션을 비활성화합니다.

![](assets/schedule.png)

## 이메일 미리 보기 및 테스트 {#preview-test}

전자 메일이 준비되면 전송을 시작하기 전에 미리 보고 테스트할 수 있습니다.

이 사용 사례에서는 이메일을 미리 보고 기존 프로필을 사용하여 증명을 보내려고 합니다.

전자 메일을 미리 보고 테스트하는 방법에 대한 추가 정보는 [이 섹션](../preview-test/preview-test.md).

1. 클릭 **[!UICONTROL 보낼 검토]**. 구성된 모든 속성, 대상 및 예약과 함께 전자 메일의 미리 보기가 표시됩니다. 수정 단추를 사용하여 이러한 요소를 편집할 수 있습니다.

1. 을(를) 클릭합니다. **[!UICONTROL 컨텐츠 시뮬레이션]** 버튼을 클릭하여 이메일을 미리 보고 증명을 보냅니다.

   ![](assets/review-email.png)

1. 왼쪽 영역에서 이메일을 미리 보는 데 사용할 프로필을 선택합니다.

1. 선택한 프로필에 따라 오른쪽 창에 이메일 미리 보기가 표시됩니다. 여러 개의 프로필을 추가한 경우 각 프로필 간을 전환하여 해당 이메일을 미리 볼 수 있습니다.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. 전자 메일 증명을 보내려면 **[!UICONTROL 테스트]** 버튼을 클릭한 다음 증명을 받을 프로필을 선택합니다.

   <!--TO REPLACE WITH SUBSTITUTION PROFILE-->In this example, we want to send the proofs to a specific test profile, which is a seed address that is not part of the target. [Learn how to work with seed addresses](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/about-seed-addresses.html){target="_blank"}

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >타겟팅된 프로필 중 일부를 가장하고 원하는 이메일 주소로 증명 메시지를 보내 메시지를 테스트할 수도 있습니다. [증명을 보내는 방법을 알아봅니다](../preview-test/preview-test.md)

1. 클릭 **[!UICONTROL 테스트 전자 메일 보내기]** 그런 다음 전송을 확인합니다.

   증명을 보내고 나면 **[!UICONTROL 테스트 전자 메일 로그 보기]** 버튼을 클릭합니다.

## 이메일 보내기 및 모니터링 {#prepare-send}

전자 메일을 검토하고 테스트하면 준비 작업을 시작하고 보낼 수 있습니다.

1. 클릭 **[!UICONTROL 준비]** 메시지 준비를 시작하려면 다음을 수행하십시오. [이메일 준비 방법 알아보기](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. 전자 메일을 보낼 준비가 되면 **[!UICONTROL 보내기]** 그런 다음 전송을 확인합니다.

   통계와 함께 실시간으로 전송을 추적할 수 있습니다. 또한 **[!UICONTROL 로그]** 버튼을 사용하면 전자 메일 전송에 대한 세부 정보에 액세스할 수 있습니다. [게재 로그를 모니터링하는 방법 알아보기](../monitor/delivery-logs.md)
   ![](assets/logs.png)

1. 전자 메일이 전송되면 전용 전자 메일에 액세스할 수 있습니다 [보고서](../reporting/reports.md) 추가 분석 목적으로 사용됩니다.

   ![](assets/reports.png)
