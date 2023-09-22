---
audience: end-user
title: 대상자 만들기 및 관리
description: Adobe Campaign 웹에서 대상자를 만들고 관리하는 방법 알아보기
badge: label="Beta"
source-git-commit: ab445f332b62baa98f9f9e84a80cc336cd88efe0
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 1%

---


# 대상자 만들기 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="대상자"
>abstract="이 화면에서 게재의 타겟팅할 수 있는 모든 대상자 목록에 액세스할 수 있습니다. 클릭 **만들기** 과 같은 다양한 워크플로우 활동을 사용하여 시각적 캔버스로 새 대상자를 만들려면 **분할** 또는 **제외**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="대상자 설정"
>abstract="대상자의 이름과 추가 옵션을 입력한 다음 **대상자 만들기** 단추를 클릭합니다."

Campaign 웹을 사용하면 시각적 워크플로우 캔버스로 새로운 대상을 만들 수 있습니다. 처음부터 시작하여 간단한 대상을 만드는 것을 넘어 워크플로우 활동을 활용하여 대상을 세분화할 수도 있습니다. 예를 들어 여러 대상을 하나의 대상으로 결합하거나, 외부 속성으로 대상을 보강하거나, 선택한 규칙에 따라 대상을 여러 대상으로 나눌 수 있습니다.

워크플로우를 만들면 결과 대상자가 기존 대상자와 함께 Campaign 데이터베이스 내에 자동으로 저장됩니다. 그런 다음 이러한 대상을 캠페인 또는 독립 실행형 게재에서 타기팅할 수 있습니다.

## 첫 번째 대상자 만들기 {#create}

대상자를 만들려면 다음 단계를 수행합니다.

1. 다음 위치로 이동 **[!UICONTROL 대상]** 메뉴를 클릭하고 **[!UICONTROL 대상자 만들기]** 오른쪽 상단 모서리에 있는 단추입니다.
1. 대상자에 대한 레이블을 제공합니다.
1. 확장 **[!UICONTROL 추가 옵션]** 섹션을 통해 고급 대상 매개 변수를 구성합니다.

   기본적으로 대상자는 **[!UICONTROL 프로필 및 타겟]** / **[!UICONTROL 목록]** explorer 메뉴. 를 사용하여 기본 저장소 위치를 변경할 수 있습니다. **[!UICONTROL 폴더]** 필드.

   ![](assets/audiences-settings.png)

1. 대상자 설정을 구성한 후 **[!UICONTROL 대상자 만들기]** 단추를 클릭합니다. 두 개의 기본 활동을 특징으로 하는 워크플로 캔버스가 표시됩니다.

   * **[!UICONTROL 대상자 작성]**: 대상자를 만들고 워크플로우의 기반으로 사용할 수 있도록 하는 워크플로우의 시작점입니다.

   * **[!UICONTROL 대상자 저장]**: 워크플로우의 마지막 단계를 나타내므로 워크플로우 결과를 새 대상자로 저장할 수 있습니다.

1. 를 엽니다. **[!UICONTROL 대상자 작성]** 활동에 액세스하고 규칙 빌더를 사용하여 데이터베이스에 포함된 데이터를 필터링하여 대상에 포함할 모집단을 정의합니다. [대상자 빌드 활동을 구성하는 방법 알아보기](../workflows/activities/build-audience.md)

1. 워크플로우에 타겟팅된 모집단에서 추가 작업을 수행하려면 필요한 만큼 활동을 추가하고 함께 연결합니다. 워크플로우 활동 구성 방법에 대한 자세한 내용은 [워크플로우 설명서](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >채널 활동은 대상자 워크플로우에서 사용할 수 없습니다.

   ![](assets/audience-creation-canvas.png)

1. 구성 **[!UICONTROL 대상자 저장]** 활동으로 워크플로우에서 업스트림으로 계산한 모집단을 저장하는 방법을 지정합니다. [대상자 저장 활동을 구성하는 방법 알아보기](../workflows/activities/save-audience.md)

1. 워크플로우가 준비되면 **[!UICONTROL 시작]** 실행할 수 있습니다.

워크플로는에 저장됩니다. **[!UICONTROL 워크플로]** 목록을에서 액세스할 수 있는 동안 **[!UICONTROL 대상]** 목록을 표시합니다.

## 대상 워크플로우 예 {#example}

아래 예제는 뉴욕에 거주하는 여성 고객을 타겟팅하고 최신 구매 내역(요가 또는 러닝 기어)에 따라 두 개의 새 대상을 만들도록 구성된 대상 워크플로우를 보여 줍니다.

![](assets/audiences-example.png)

1. 다음 **[!UICONTROL 대상자 작성]** 활동은 뉴욕에 사는 모든 여성 프로필을 타겟으로 합니다.
1. 다음 **[!UICONTROL 데이터 보강]** 활동은 구매 테이블의 정보를 통해 고객을 강화하여 고객이 구매한 제품 유형을 식별합니다.
1. 다음 **[!UICONTROL 분할]** 활동은 고객의 최신 구매를 기준으로 워크플로우를 두 개의 경로로 나눕니다.
1. 다음 **[!UICONTROL 대상자 저장]** 각 경로의 끝에 있는 활동은 각 경로에서 계산된 모집단을 포함하여 데이터베이스에 두 개의 새 대상을 만듭니다.

## 대상자 모니터링 및 관리 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="대상 오류"
>abstract="대상 데이터를 사용할 수 없습니다. 워크플로우 실행이 종료될 때까지 기다려 주십시오."

Campaign 웹에서 사용할 수 있는 대상자 목록은 **[!UICONTROL 대상]** 메뉴 아래의 제품에서 사용할 수 있습니다.

![](assets/audiences-list.png)

대상은 여러 소스에서 발생할 수 있습니다. 다음 **[!UICONTROL 원본]** 열은 지정된 대상이 만들어진 위치를 나타냅니다.

* **[!UICONTROL Adobe Campaign]**: 이러한 대상은 Adobe Campaign V8 콘솔에서 만들어집니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** 이러한 대상은 Adobe Experience Platform 내에서 생성되며 Adobe 소스 및 대상 통합을 사용하여 Campaign 웹에 통합됩니다. 에서 이 통합을 설정하는 방법에 대해 알아봅니다. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign WebUI]**: 이러한 대상자는 Campaign 웹 대상자 워크플로우를 사용하여 만들어집니다. [대상자를 만드는 방법 알아보기](create-audience.md)

대상자에 대한 자세한 내용을 보려면 목록에서 대상자를 여십시오. 대상자 속성이 대상자에 포함된 프로필 수와 함께 표시됩니다. 다음을 사용하여 언제든지 대상자 수를 새로 고칠 수 있습니다. **[!UICONTROL 계산]** 단추를 클릭합니다.

다음 **[!UICONTROL 데이터]** 탭에서는 대상의 일부인 프로필을 표시할 수 있습니다. 열을 더 추가하여 이 보기를 사용자 지정하거나 고급 필터를 활용하여 표시된 데이터를 구체화할 수 있습니다.

![](assets/audiences-details.png)

대상을 복제하거나 삭제하려면 **[!UICONTROL 추가 작업]** 버튼은 대상자 이름 옆의 대상자 목록 또는 대상자 세부 사항 화면 내에서 사용할 수 있습니다.
