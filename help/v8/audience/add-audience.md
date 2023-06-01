---
audience: end-user
title: 기존 대상자 선택
description: 대상자 선택 방법 알아보기
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: d4645689ebaa5439a01b2f558f398cbeb79089a7
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 95%

---


# 기존 대상자 선택 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="기존 대상자 선택"
>abstract="대상자는 Adobe Campaign v8 Console에서 정의됩니다. Adobe Experience Platform 통합을 사용할 수 있는 경우 Platform에서 정의된 대상자를 확인할 수도 있습니다."

이 섹션에서는 이메일 게재의 대상 모집단을 정의할 때 기존 대상자를 선택하는 방법에 대해 설명합니다.

이외에 수행할 수 있는 작업은 다음과 같습니다.

* 새 대상을 작성합니다. [자세히 알아보기](segment-builder.md)
* 외부 파일에서 대상자를 로드합니다. [자세히 알아보기](file-audience.md)
* Adobe Experience Platform 대상자 사용 [자세히 알아보기](aep-audience.md)


메시지의 기존 대상자를 선택하려면 아래 단계를 따르십시오.

1. 게재 생성 도우미의 **대상자** 섹션에서 **[!UICONTROL 대상자 선택]** 버튼을 클릭합니다.

   ![](assets/create-audience.png)

1. 기존 대상자를 사용하려면 **[!UICONTROL 대상자 선택]**&#x200B;을 선택합니다. 이 이메일에서 사용할 새 대상자를 만들려면 **직접 만들기**&#x200B;를 선택합니다. 이 [섹션](segment-builder.md)을 참조하십시오.

   이 화면에는 Adobe Campaign 콘솔 또는 Adobe Experience Platform에서 정의된 기존의 모든 대상자가 표시됩니다.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Adobe Experience Platform 대상자를 활용하려면 대상과의 통합을 구성해야 합니다. [대상 설명서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html)를 참조하십시오{target="_blank"}.

1. 대상자를 선택하고 **선택**&#x200B;을 클릭합니다.

1. 대상자를 세분화하려면 **규칙 편집**&#x200B;을 클릭합니다.

   ![](assets/create-audience3.png)

1. 규칙 빌더를 사용하면 추가 필터를 사용하거나 다른 대상자를 결합하여 대상자를 보강할 수 있습니다. 이 [섹션](segment-builder.md)을 참조하십시오.

   ![](assets/create-audience4.png)

1. **저장**&#x200B;을 클릭합니다.

캠페인의 영향을 측정하기 위해 컨트롤 그룹을 설정할 수도 있습니다. 컨트롤 그룹은 메시지를 받지 않습니다. 그러면 메시지를 받은 모집단과 메시지를 받지 않은 연락처의 동작을 비교할 수 있습니다. 이 [섹션](control-group.md)을 참조하십시오.