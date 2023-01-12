---
audience: end-user
title: 대상자 추가
description: Campaign v8 웹 설명서
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 4%

---

# 대상자 선택 {#add-audience}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="기존 대상 선택"
>abstract="대상은 Adobe Campaign v8 콘솔에서 정의됩니다. 사용 가능한 Adobe Experience Platform 통합이 있는 경우 플랫폼 정의 대상도 볼 수 있어야 합니다."

이 섹션에서는 이메일 게재의 대상 모집단을 정의할 때 기존 대상자를 선택하는 방법을 설명합니다. 새 대상을 만들려면 이 항목을 참조하십시오 [섹션](segment-builder.md).

1. 에서 **Audience** 게재 만들기 도우미의 섹션에서 **[!UICONTROL 대상 선택]** 버튼을 클릭합니다.

   ![](assets/create-audience.png)

1. 선택 **[!UICONTROL 대상 선택]** 기존 대상자를 사용하려면 이 이메일에 사용할 새 대상자를 만들려면 을(를) 선택합니다 **직접 만들기**. 다음을 참조하십시오 [섹션](segment-builder.md).

   이 화면에는 Adobe Campaign 콘솔 또는 Adobe Experience Platform에서 정의된 모든 기존 대상이 표시됩니다.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Adobe Experience Platform 대상을 활용하려면 대상과의 통합을 구성해야 합니다. 자세한 내용은 [대상 설명서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=ko).

1. 대상자를 선택하고 을(를) 클릭합니다. **선택**.

1. 클릭 **규칙 편집** 대상을 세분화하려면 다음을 수행하십시오.

   ![](assets/create-audience3.png)

1. 규칙 빌더를 사용하면 추가 필터나 다른 대상을 결합하여 대상을 보강할 수 있습니다. 다음 보기 [섹션](segment-builder.md).

   ![](assets/create-audience4.png)

1. **저장**&#x200B;을 클릭합니다.

캠페인의 영향을 측정하도록 컨트롤 그룹을 설정할 수도 있습니다. 컨트롤 그룹이 메시지를 받지 않습니다. 이렇게 하면 메시지를 받은 모집단 행동과 그렇지 않은 연락처의 동작을 비교할 수 있습니다. 자세한 내용은 [섹션](control-group.md).