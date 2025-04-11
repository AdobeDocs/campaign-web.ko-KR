---
product: campaign
title: 게재 템플릿 사용
description: Campaign 웹에서 게재 템플릿을 만들고 사용하는 방법을 알아봅니다
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 11%

---

# 게재 템플릿 사용 {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="게재 템플릿"
>abstract="디자인 프로세스를 가속화하고 향상시키려면 게재 템플릿을 만들어 캠페인 전반에서 사용자 지정 콘텐츠 및 설정을 재사용합니다. 이 기능은 창의적인 모양과 느낌을 표준화하여 캠페인을 더 빨리 실행하고 시작할 수 있습니다."

디자인 프로세스를 가속화하고 향상시키려면 게재 템플릿을 만들어 캠페인 전반에서 사용자 지정 콘텐츠 및 설정을 재사용합니다. 이 기능은 창의적인 모양과 느낌을 표준화하여 캠페인을 더 빨리 실행하고 시작할 수 있습니다.

템플릿에는 다음이 포함됩니다.

* 템플릿의 **폴더** 및 **실행 폴더**&#x200B;입니다. 폴더는 게재 템플릿이 저장되는 위치입니다. 실행 폴더는 이 템플릿을 기반으로 생성된 게재가 저장되는 폴더입니다.
* [유형화](../advanced-settings/delivery-settings.md#typology),
* 발신자 주소,
* [컨트롤 그룹](../audience/control-group.md)을(를) 포함한 [대상자](../audience/about-recipients.md),
* 사용자 지정 [콘텐츠](../email/edit-content.md),
* [개인화된 필드](../personalization/personalize.md) 및 [조건부 콘텐츠](../personalization/conditions.md),
* [미러 페이지](../email/mirror-page.md) 및 구독 취소 링크 [링크](../email/message-tracking.md),
* 리소스 유효성, 재시도 매개 변수 또는 격리 설정 등 다른 게재 속성입니다.

>[!NOTE]
>
>게재 템플릿은 [콘텐츠 템플릿](../email/create-email-templates.md)과(와) 다르며, 이를 통해 기본 제공되는 샘플 이메일 템플릿 중 하나를 사용하여 이메일 콘텐츠만 재사용하고 콘텐츠 작성을 시작할 수 있습니다.

## 게재 템플릿 액세스 및 관리 {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="게재 템플릿 작업"
>abstract="게재 템플릿을 사용하여 향후 캠페인 전체에서 사용할 수 있도록 게재 설정을 만들고 저장합니다. 처음부터 게재 템플릿을 만들거나, 기존 템플릿을 복제하거나, 게재를 템플릿으로 변환합니다."

콘텐츠 템플릿 목록에 액세스하려면 왼쪽 메뉴에서 **[!UICONTROL 캠페인 관리]** > **[!UICONTROL 게재]**&#x200B;를 선택하고 **템플릿** 탭으로 이동합니다.

![게재 메뉴의 템플릿 탭](assets/templates-tab.png){zoomable="yes"}

현재 환경에서 만든 모든 템플릿이 표시됩니다.

채널 및 폴더별로 콘텐츠 템플릿을 필터링할 수 있습니다. 게재 속성을 사용하여 규칙을 작성하여 고급 필터를 설정할 수도 있습니다. [쿼리 모델러에 대해 자세히 알아보기](../audience/../query/query-modeler-overview.md)

![템플릿 필터링 옵션](assets/templates-filters.png){zoomable="yes"}

템플릿을 편집하려면 목록에서 원하는 항목을 클릭합니다. 여기에서:

* 콘텐츠, 속성, 대상자 및 여기에 첨부된 모든 오퍼를 수정합니다.
* 템플릿을 테스트합니다. [자세히 알아보기](#test-template)

![템플릿 편집](assets/templates-edition.png){zoomable="yes"}

템플릿을 삭제하거나 [복제](#copy-an-existing-template)하려면 **[!UICONTROL 추가 작업]** 메뉴(**[!UICONTROL 템플릿]** 목록 또는 템플릿 편집 화면)에서 해당 작업을 선택하십시오.

![템플릿에 대한 추가 작업 메뉴](assets/templates-more-actions.png){zoomable="yes"}

>[!NOTE]
>
>템플릿을 편집하거나 삭제할 때 이 템플릿을 사용하여 만든 게재는 영향을 받지 않습니다.

## 게재 템플릿 만들기 {#create-a-delivery-template}

게재 템플릿을 만들려면 다음 작업을 수행할 수 있습니다.

* 기존 템플릿 복제 - [자세히 알아보기](#copy-an-existing-template)
* 기존 게재를 템플릿으로 변환 - [자세히 알아보기](#convert-an-existing-delivery)
* 처음부터 게재 템플릿 만들기 - [자세히 알아보기](#create-a-new-template)

### 기존 게재 템플릿 복제 {#copy-an-existing-template}

Campaign에는 이메일, 푸시 및 SMS와 같은 각 채널에 대한 기본 제공 템플릿이 포함되어 있습니다. 게재 템플릿을 만드는 가장 쉬운 방법은 기본 제공 템플릿을 복제하고 사용자 지정하는 것입니다.

>[!NOTE]
>
>사용자 지정 템플릿을 복제할 수도 있습니다.

게재 템플릿을 복제하려면 다음 단계를 따르십시오.

1. **게재** 왼쪽 메뉴에서 **템플릿** 탭으로 이동합니다. [자세히 알아보기](#access-manage-templates)
1. 원하는 템플릿 이름의 오른쪽에 있는 **[!UICONTROL 추가 작업]** 단추를 클릭하고 **[!UICONTROL 복제]**&#x200B;를 선택합니다.

   목록에서 템플릿을 선택하고 템플릿 편집 화면에서 이 옵션을 선택할 수도 있습니다.

1. 복제를 확인합니다.

   ![템플릿 복제용 확인 대화 상자](assets/templates-duplicate-confirm.png){zoomable="yes"}

1. 새 템플릿 대시보드가 중앙 화면에 열립니다. 필요에 따라 템플릿 설정을 편집합니다.

   ![중복된 템플릿 대시보드](assets/templates-duplicated-item.png){zoomable="yes"}

1. 템플릿을 저장하고 검토하려면 **[!UICONTROL 검토]** 단추를 클릭하십시오. 모든 설정을 편집하고, 삭제하고, 복제할 수 있습니다.

   ![템플릿 검토 화면](assets/templates-review-screen.png){zoomable="yes"}

1. 필요한 경우 템플릿 렌더링을 테스트합니다. [자세히 알아보기](#test-template)

새 템플릿이 [**템플릿** 목록](#access-manage-templates)에 추가됩니다. 이제 새 게재를 만들면 선택할 수 있습니다.

### 게재를 템플릿으로 변환 {#convert-an-existing-delivery}

모든 게재를 템플릿으로 변환하여 나중에 반복 게재 작업을 수행할 수 있습니다.

게재를 템플릿으로 저장하려면 다음 단계를 수행합니다.

1. **[!UICONTROL 캠페인 관리]** > **[!UICONTROL 게재]** 메뉴로 이동합니다.
1. **[!UICONTROL 찾아보기]** 탭에서 원하는 배달 이름 오른쪽에 있는 **[!UICONTROL 추가 작업]** 단추를 클릭하고 **[!UICONTROL 템플릿으로 복사]**&#x200B;를 선택합니다.

   ![게재를 템플릿으로 복사하는 옵션](assets/templates-convert-delivery.png){zoomable="yes"}

   목록에서 템플릿을 선택하고 템플릿 편집 화면에서 이 옵션을 선택할 수도 있습니다.

1. 복제를 확인합니다.

1. 새 템플릿 대시보드가 중앙 화면에 열립니다. 필요에 따라 템플릿 설정을 편집합니다.

1. 템플릿을 저장하고 검토하려면 **[!UICONTROL 검토]** 단추를 클릭하십시오. 모든 설정을 편집하고, 삭제하고, 복제할 수 있습니다.

1. 필요한 경우 템플릿 렌더링을 테스트합니다. [자세히 알아보기](#test-template)

새 템플릿이 [**템플릿** 목록](#access-manage-templates)에 추가됩니다. 이제 새 게재를 만들면 선택할 수 있습니다.

### 새 게재 템플릿 만들기 {#create-a-new-template}

>[!NOTE]
>
>구성 오류를 방지하려면 Adobe에서는 새 템플릿을 만드는 대신 [기본 제공 템플릿을 복제](#copy-an-existing-template)하고 속성을 사용자 지정하는 것이 좋습니다.

게재 템플릿을 처음부터 구성하려면 다음 단계를 따르십시오.

1. **게재** 왼쪽 메뉴에서 **템플릿** 탭으로 이동합니다. [자세히 알아보기](#access-manage-templates)
1. **[!UICONTROL 템플릿 만들기]** 단추를 클릭합니다.

   ![템플릿 만들기 단추](assets/templates-create-button.png){zoomable="yes"}

1. 템플릿에 사용할 채널을 선택합니다.
1. 해당 채널의 기본 제공 게재 템플릿은 기본적으로 자체 템플릿을 작성하는 데 사용됩니다. 필요한 경우 선택한 채널 오른쪽에 있는 전용 버튼을 사용하여 다른 템플릿을 선택합니다.

   ![새 템플릿에 대한 채널 선택](assets/templates-channel-browse.png){zoomable="yes"}


1. **[!UICONTROL 템플릿 만들기]** 단추를 다시 클릭합니다.

1. 선택한 채널에 따라 템플릿 속성, [대상](../audience/add-audience.md) 및 콘텐츠를 정의합니다.

   >[!NOTE]
   >
   >아래 섹션에서 게재 채널 및 각 콘텐츠를 디자인하는 방법에 대해 자세히 알아보십시오.
   >
   > * [이메일 채널](../email/create-email.md)
   > * [푸시 알림 채널](../push/gs-push.md)
   > * [SMS 채널](../sms/create-sms.md)

1. 또한 전자 메일 템플릿의 경우 화면 오른쪽 상단의 **[!UICONTROL 설정]** 단추를 통해 유형화 규칙 및 대상 매핑과 같은 고급 설정에 액세스할 수 있습니다. [자세히 알아보기](../advanced-settings/delivery-settings.md)

1. 템플릿을 저장하고 검토하려면 **[!UICONTROL 검토]** 단추를 클릭하십시오. 모든 설정을 편집하고, 삭제하고, 복제할 수 있습니다.

1. 필요한 경우 템플릿 렌더링을 테스트합니다. [자세히 알아보기](#test-template)

새 템플릿이 [**템플릿** 목록](#access-manage-templates)에 추가됩니다. 이제 새 게재를 만들면 선택할 수 있습니다.

## 게재 템플릿 테스트 {#test-template}

처음부터 만들거나 기존 콘텐츠에서 만든 모든 게재 템플릿의 렌더링을 테스트할 수 있습니다. 이렇게 하려면 다음 단계를 수행합니다.

1. **[!UICONTROL 캠페인 관리]** > **[!UICONTROL 게재]** 메뉴를 통해 **템플릿** 탭으로 이동하여 템플릿을 선택합니다. [자세히 알아보기](#access-manage-templates)

1. 화면 오른쪽 상단의 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

   ![콘텐츠 시뮬레이션 단추](assets/templates-simulate-button.png){zoomable="yes"}

1. 하나 이상의 테스트 프로필을 선택하여 이메일 렌더링을 확인합니다. 데이터베이스에서 실제 프로필을 선택할 수도 있습니다. [테스트 프로필에 대해 자세히 알아보기](../audience/test-profiles.md)

1. 다른 프로필 간에 전환하여 선택한 프로필에 따라 개인화된 메시지 표현을 가져옵니다. 확대/축소 수준을 조정하고 데스크탑 또는 모바일 보기를 선택할 수도 있습니다.

[콘텐츠 미리보기에 대해 자세히 알아보기](../preview-test/preview-content.md)

   ![시뮬레이션된 콘텐츠 미리 보기](assets/templates-stimulate.png){zoomable="yes"}

1. 템플릿 편집 화면으로 돌아가려면 창을 닫습니다.

>[!NOTE]
>
>이메일 렌더링을 사용하거나 게재 템플릿에서 증명을 보낼 수 없습니다.