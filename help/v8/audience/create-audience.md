---
audience: end-user
title: 대상자 만들기
description: Adobe Campaign 웹에서 대상자를 만드는 방법을 알아봅니다
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 16%

---

# 대상자 만들기 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="대상자"
>abstract="이 화면에서 워크플로 또는 독립 실행형 게재에서 타겟팅할 수 있는 모든 대상자 목록에 액세스할 수 있습니다. 시각적 캔버스에 새 대상자를 만들려면 **만들기**&#x200B;를 클릭하십시오.<br/><br/>처음부터 시작하여 간단한 대상자를 만드는 것 외에도 워크플로 활동을 활용하여 대상자를 세분화할 수도 있습니다. 예를 들어 여러 대상자를 하나로 결합하거나, 외부 속성으로 대상자를 강화하거나, 선택한 규칙에 따라 여러 대상자로 나눌 수 있습니다."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Campaign 웹을 사용하면 시각적 워크플로우 캔버스로 새로운 대상을 만들 수 있습니다. 처음부터 시작하여 간단한 대상자를 만드는 것 외에도 워크플로 활동을 활용하여 대상자를 세분화할 수도 있습니다. 예를 들어 여러 대상자를 하나로 결합하거나, 외부 속성으로 대상자를 강화하거나, 선택한 규칙에 따라 여러 대상자로 나눌 수 있습니다.

워크플로우를 만들면 결과 대상자가 기존 대상자와 함께 Campaign 데이터베이스 내에 자동으로 저장됩니다. 그런 다음 워크플로우 또는 독립 실행형 게재에서 이러한 대상을 타기팅할 수 있습니다.

다음 **[!UICONTROL 원본]** 열은 대상자의 출처를 나타냅니다. **[!UICONTROL Adobe Campaign]** 대상자는 Adobe Campaign v8 콘솔 또는 웹 사용자 인터페이스로 만들어졌지만 **[!UICONTROL Adobe Experience Platform:]** 대상은 Adobe Experience Platform 내에서 만들어지고 Adobe 소스 및 대상 통합을 사용하여 Campaign에 통합되었습니다.

➡️ [비디오에서 이 기능 살펴보기](#video)

## 첫 번째 대상자 만들기 {#create}

대상자를 만들려면 다음 단계를 수행합니다.

1. 다음 위치로 이동 **[!UICONTROL 대상]** 메뉴를 클릭하고 **[!UICONTROL 대상자 만들기]** 오른쪽 상단 모서리에 있는 단추입니다.

1. 새 워크플로우가 자동으로 만들어지므로 활동을 결합하여 대상을 생성할 수 있습니다. 기본적으로 캔버스에는 두 개의 기본 활동이 포함되어 있습니다.

   * &quot;쿼리&quot; **[!UICONTROL 대상자 작성]** 활동은 워크플로우의 시작점이며, 이를 통해 대상자를 만들고 워크플로우의 기반으로 사용할 수 있습니다.

   * &quot;새 대상&quot; **[!UICONTROL 대상자 저장]** 활동은 워크플로우의 마지막 단계를 나타내므로 결과를 새 대상자로 저장할 수 있습니다.

   ![](assets/create-audience-blank.png){zoomable=&quot;yes&quot;}

   >[!IMPORTANT]
   >
   >대상자 워크플로는에 저장됩니다. **워크플로** 메뉴, 다른 Campaign 워크플로우와 함께 사용할 수 있습니다. 대상자를 빌드하도록 특별히 설계되었으며 세로 캔버스로 식별할 수 있습니다.

1. 가독성을 높이려면 워크플로 설정에서 워크플로 이름을 변경하는 것이 좋습니다. **레이블** 필드. [워크플로우 설정 구성 방법 알아보기](../workflows/workflow-settings.md)

1. 를 엽니다. **[!UICONTROL 대상자 작성]** 활동에 참여하고 쿼리 모델러를 사용하여 데이터베이스에 포함된 데이터를 필터링하여 대상자에 포함할 모집단을 정의합니다. [대상자 빌드 활동을 구성하는 방법 알아보기](../workflows/activities/build-audience.md)

1. 워크플로우에 타겟팅된 모집단에서 추가 작업을 수행하려면 필요한 만큼 활동을 추가하고 함께 연결합니다. 워크플로우 활동 구성 방법에 대한 자세한 내용은 [워크플로우 설명서](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >채널 활동은 대상자 워크플로우에서 사용할 수 없습니다.

   ![](assets/audience-creation-canvas.png){zoomable=&quot;yes&quot;}

1. 구성 **[!UICONTROL 대상자 저장]** 활동으로 워크플로우에서 업스트림으로 계산한 모집단을 저장하는 방법을 지정합니다. [대상자 저장 활동을 구성하는 방법 알아보기](../workflows/activities/save-audience.md)

1. 워크플로우가 준비되면 **[!UICONTROL 시작]** 실행할 수 있습니다.

워크플로는에 저장됩니다. **[!UICONTROL 워크플로]** 목록을에서 액세스할 수 있는 동안 **[!UICONTROL 대상]** 에 정의된 레이블이 있는 목록 **대상자 저장** 활동. 에서 대상자를 모니터링하고 관리하는 방법 알아보기 [이 섹션](manage-audience.md)

이제 이 대상을 게재의 주요 대상으로 사용할 수 있습니다. [자세히 알아보기](add-audience.md)

## 대상 워크플로우 예 {#example}

아래 예제는 뉴욕에 거주하는 여성 고객을 타겟팅하고 최신 구매 내역(요가 또는 러닝 기어)에 따라 두 개의 새 대상을 만들도록 구성된 대상 워크플로우를 보여 줍니다.

![](assets/audiences-example.png){zoomable=&quot;yes&quot;}

1. 다음 **[!UICONTROL 대상자 작성]** 활동은 뉴욕에 사는 모든 여성 프로필을 타겟으로 합니다.
1. 다음 **[!UICONTROL 데이터 보강]** 활동은 구매 테이블의 정보를 통해 고객을 강화하여 고객이 구매한 제품 유형을 식별합니다.
1. 다음 **[!UICONTROL 분할]** 활동은 고객의 최신 구매를 기준으로 워크플로우를 두 개의 경로로 나눕니다.
1. 다음 **[!UICONTROL 대상자 저장]** 각 경로의 끝에 있는 활동은 각 경로에서 계산된 모집단을 포함하여 데이터베이스에 두 개의 새 대상을 만듭니다.

## 대상자 편집 {#edit}

필요한 경우 해당 워크플로우를 다시 실행하여 워크플로우에서 생성된 대상자를 수정할 수 있습니다. 이를 통해 손쉽게 대상 데이터를 새로 고치거나 필요에 따라 쿼리를 조정하여 대상을 세분화할 수 있습니다.

1. 다음 위치로 이동 **대상** 을 클릭하고 편집할 대상을 엽니다.
1. 다음에서 **개요** 탭, **마지막 워크플로우** 섹션은 대상자를 생성하는 데 사용되는 워크플로우에 대한 링크를 제공합니다. 워크플로우에 액세스하려면 클릭합니다.
1. 원하는 대로 변경하고 **시작** 단추를 클릭하여 워크플로우를 다시 실행합니다. 완료되면 워크플로우로 인한 대상자가 최신 워크플로우 결과로 자동 업데이트됩니다.

기본적으로 대상 워크플로우를 다시 실행하면 대상의 전체 콘텐츠가 새 데이터로 대체되므로 이전 데이터가 손실됩니다.

기존 대상 결과를 바꾸지 않으려면 **대상자 저장** 요구 사항에 맞는 활동. 예를 들어 **대상 레이블** 새 결과를 새 대상에 저장하거나 이전 데이터를 지우는 일 없이 기존 대상 콘텐츠에 새 결과를 추가하는 필드. [대상자 저장 활동을 구성하는 방법 알아보기](../workflows/activities/save-audience.md)

![](assets/edit-audience-save.png){zoomable=&quot;yes&quot;}

## 사용법 비디오 {#video}

대상을 빌드 및 관리하고, 게재할 대상을 선택하고, 컨트롤 그룹을 정의하는 방법에 대해 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)
