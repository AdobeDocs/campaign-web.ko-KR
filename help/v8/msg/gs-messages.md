---
audience: end-user
title: Campaign v8 Web에서 메시지 및 게재 시작하기
description: Campaign Web으로 게재 작업을 수행하고 메시지를 전송하는 방법 알아보기
badge: 레이블=“Alpha” 유형=“Positive”
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 29%

---

# 메시지 시작{#gs-messages}


Adobe Campaign을 사용하면 이메일, SMS 및 푸시 알림을 비롯한 크로스 채널 캠페인을 전송하고, 다양한 전용 보고서를 사용하여 캠페인의 효과를 측정할 수 있습니다. 이러한 메시지는 게재를 통해 디자인되고 전송되며 각 수신자에 대해 개인화할 수 있습니다. 이러한 게재는 독립 실행형이거나 마케팅 캠페인의 컨텍스트에 포함될 수 있습니다.

Adobe Campaign v8에는 다음과 같은 게재 채널이 포함되어 있습니다.

* **이메일 채널**: 이메일 게재를 사용하면 개인화된 이메일을 대상 모집단으로 보낼 수 있습니다. 에서 이메일을 만들고 보내는 방법 알아보기 [이 페이지](../email/create-email.md).

* **SMS 채널**: 모바일 채널 게재는 개인화된 SMS를 대상 모집단으로 보낼 수 있습니다.  에서 SMS를 만들고 보내는 방법 알아보기 [이 페이지](../sms/create-sms.md).

* **모바일 앱 채널**:모바일 앱 게재를 사용하면 iOS 및 Android 시스템에 알림을 전송할 수 있습니다.  에서 푸시 알림을 만들고 전송하는 방법 알아보기 [이 페이지](../push/gs-push.md).

## 게재 만들기 {#create-delivery}

에서 독립 실행형 게재를 만들 수 있습니다. **[!UICONTROL 게재]** 왼쪽 메뉴에서 또는 마케팅 캠페인의 컨텍스트에서 게재를 만듭니다. **[!UICONTROL 캠페인]** 왼쪽 메뉴.

>[!BEGINTABS]

>[!TAB 독립 실행형 게재 만들기]

독립 실행형 게재를 만들려면 다음 단계를 수행하십시오.

1. 다음으로 이동 **[!UICONTROL 게재]** 왼쪽 탐색 메뉴에서 **[!UICONTROL 게재 만들기]** 단추를 클릭합니다.

   ![](assets/create-a-delivery.png)

1. 게재할 채널을 선택합니다. 다음 섹션에서 게재 채널 및 게재 콘텐츠를 정의하는 방법에 대해 자세히 알아보십시오.

   * [이메일 채널](../email/create-email.md)
   * [푸시 알림 채널](../push/gs-push.md)
   * [SMS 채널](../sms/create-sms.md)

1. 기본 타겟 및 컨트롤 그룹에 대한 게재 대상을 정의합니다. 에서 대상자에 대해 자세히 알아보기 [이 섹션](../audience/about-audiences.md).
1. 메시지 콘텐츠를 정의합니다.
1. (선택 사항) 배달 일정을 정의합니다. 일정이 정의되지 않은 경우 다음을 클릭하면 메시지가 즉시 전송됩니다. **[!UICONTROL 보내기]** 단추를 클릭합니다.
1. 다음을 클릭합니다.  **[!UICONTROL 검토 및 보내기]** 단추를 클릭하여 설정을 확인합니다.
1. 사용  **[!UICONTROL 콘텐츠 시뮬레이션]** 버튼을 클릭하여 게재 및 개인화 설정을 테스트합니다. 에서 메시지 시뮬레이션에 대해 자세히 알아보기 [이 섹션](../preview-test/preview-test.md).
1. 다음을 클릭합니다.  **[!UICONTROL 준비]** 대상 모집단을 계산하고 메시지를 생성하는 단추입니다. 준비 단계는 몇 분 정도 걸릴 수 있습니다. 준비가 완료되면 메시지를 보낼 준비가 되었습니다. 오류가 발생한 경우 **로그** 경고 및 경고를 확인합니다.
1. 결과를 확인하고  **[!UICONTROL 보내기]** 단추를 클릭하여 메시지 전송을 시작합니다.
1. 메시지가 전송되면 **보고서** 섹션을 참조하십시오. 에서 게재 보고서에 대해 자세히 알아보기 [이 섹션](../reporting/delivery-reports.md).

>[!TAB 캠페인에서 게재 만들기]

캠페인에서 게재를 만들려면 다음 단계를 수행합니다.

1. 캠페인을 만들거나 기존 캠페인을 엽니다. 자세히 알아보기 [마케팅 캠페인](../campaigns/gs-campaigns.md).
1. 워크플로우를 만들거나 기존 워크플로우를 엽니다.
1. 추가 및 구성 **[!UICONTROL 대상자 작성]** 활동을 클릭하고 `+`단추를 클릭합니다.

   ![](assets/add-delivery-in-wf.png)

   다음 **[!UICONTROL 대상자 작성]** 활동에 자세히 설명되어 있습니다. [이 섹션](../workflows/activities/build-audience.md).

1. 게재 활동 선택: **[!UICONTROL 이메일]**, **[!UICONTROL SMS]**, **[!UICONTROL 푸시 알림(Android)]** 또는 **[!UICONTROL 푸시 알림(iOS)]**. 워크플로우의 게재 채널 활동과 여기에서 게재 콘텐츠를 정의하는 방법에 대해 자세히 알아보십시오 [섹션](../workflows/activities/about-activities.md#channel).
1. 워크플로우를 시작하고 로그를 확인합니다.

워크플로우를 만들지 않고 캠페인에 게재를 추가할 수도 있습니다. 이렇게 하려면 **[!UICONTROL 게재]** 캠페인의 탭을 클릭하고 **[!UICONTROL 게재 만들기]** 단추를 클릭합니다.

![](assets/new-campaign-delivery.png)

구성 단계는 독립형 게재와 유사합니다.

캠페인을 구성하고 캠페인에 속한 게재를 관리하는 방법에 대한 자세한 내용은 다음을 참조하십시오. [이 섹션](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## 개인화 추가{#personalization}

Adobe Campaign에서 제공하는 메시지는 다양한 방식으로 개인화할 수 있습니다. [개인화 기능에 대해 자세히 알아보기](../personalization/personalize.md).

Campaign을 사용하여 다이내믹 콘텐츠를 만들고 개인화된 메시지를 보낼 수 있습니다. 개인화 기능을 결합하여 메시지를 개선하고 사용자 정의 사용자 경험을 만들 수 있습니다.

다음과 같은 작업을 수행하여 메시지 콘텐츠를 개인화할 수 있습니다.

* 동적 **개인화 필드** 삽입

   개인화 필드는 메시지의 첫 번째 수준 개인화에 사용됩니다. 개인화 편집기에서 데이터베이스에서 사용 가능한 모든 필드를 선택할 수 있습니다. 게재의 경우 수신자, 메시지 또는 게재와 관련된 모든 필드를 선택할 수 있습니다. 이러한 개인화 속성은 메시지의 제목 줄이나 본문에 삽입할 수 있습니다. [자세히 알아보기](../personalization/personalize.md)

* 미리 정의된 **콘텐츠 블록** 삽입

   Campaign에는 게재에 삽입할 수 있는 특정 렌더링이 포함된 개인화 블록 세트가 제공됩니다. 예를 들어 로고, 인사말 메시지 또는 메시지 미러 페이지에 대한 링크를 추가할 수 있습니다. 콘텐츠 블록은 개인화 편집기의 전용 항목에서 사용할 수 있습니다. [자세히 알아보기](../personalization/personalize.md#ootb-content-blocks)

* 만들기 **조건부 콘텐츠**

   예를 들어 수신자의 프로필을 기반으로 동적 개인화를 추가하도록 조건부 콘텐츠를 구성합니다. 특정 조건이 참일 때 텍스트 블록 및/또는 이미지가 삽입됩니다. [자세히 알아보기](../personalization/conditions.md)

* 추가 **개인화된 오퍼**

   수신자 위치, 현재 날씨 또는 마지막 구매 주문에 따라 메시지 콘텐츠에 개인화된 오퍼를 삽입합니다.


## 게재 미리 보기 및 테스트

메시지 콘텐츠가 정의되면 미리 보기하여 메시지 렌더링을 제어하고 테스트 프로필로 개인화 설정을 확인할 수 있습니다. [자세히 알아보기](../preview-test/preview-test.md)


## 게재 및 추적 로그{#gs-tracking-logs}

메시지를 게재한 후 마케팅 캠페인이 효율적이고 고객에게 도달하는지 확인하는 데 있어 게재 모니터링은 중요한 단계입니다. 게재 후 모니터링은 물론 게재 실패와 검역된 메시지가 어떻게 관리되는지 파악할 수 있습니다.

## 게재 복제{#delivery-duplicate}

게재 목록 또는 게재 대시보드에서 기존 게재의 사본을 만들 수 있습니다.

게재 목록에서 게재를 복제하려면 다음 단계를 수행합니다.

1. 복제할 게재 이름 옆의 오른쪽에 있는 세 점 버튼을 클릭합니다.
1. 선택  **[!UICONTROL 복제]**.
1. 복제 확인: 새 게재 대시보드가 중앙 화면에 열립니다.


대시보드에서 게재를 복제하려면 다음 단계를 따르십시오.

1. 게재를 열고  **[!UICONTROL ...자세히]** 화면의 맨 위 섹션에 있는 단추입니다.
1. 선택  **[!UICONTROL 복제]**.
1. 복제 확인: 중앙 화면에서 새 게재가 현재 게재를 대체합니다.
