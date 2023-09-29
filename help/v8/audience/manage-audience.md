---
audience: end-user
title: 대상자 모니터링 및 관리
description: Adobe Campaign 웹에서 대상자를 모니터링하고 관리하는 방법 알아보기
badge: label="Beta"
source-git-commit: 21436695f6f4bc9e99bb7983e4705cbbe40f07eb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 8%

---


# 대상자 모니터링 및 관리 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="대상자 오류"
>abstract="대상자 데이터를 사용할 수 없습니다. 워크플로 실행이 종료될 때까지 기다려 주십시오."

Campaign 웹에서 사용할 수 있는 대상자 목록은 **[!UICONTROL 대상]** 메뉴 아래의 제품에서 사용할 수 있습니다.

![](assets/audiences-list.png)

대상은 여러 소스에서 발생할 수 있습니다. 다음 **[!UICONTROL 원본]** 열은 지정된 대상이 만들어진 위치를 나타냅니다.

* **[!UICONTROL Adobe Campaign]**: 이러한 대상은 Adobe Campaign V8 콘솔에서 만들어집니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** 이러한 대상은 Adobe Experience Platform 내에서 생성되며 Adobe 소스 및 대상 통합을 사용하여 Campaign 웹에 통합됩니다. 에서 이 통합을 설정하는 방법에 대해 알아봅니다. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>Campaign에서 Adobe Experience Platform 대상을 사용하려면 Adobe 소스 및 대상과의 통합을 구성해야 합니다. 을(를) 참조하십시오 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL Adobe Campaign WebUI]**: 이러한 대상자는 Campaign 웹 대상자 워크플로우를 사용하여 만들어집니다. [대상자를 만드는 방법 알아보기](create-audience.md)

대상자에 대한 자세한 내용을 보려면 목록에서 대상자를 여십시오. 대상자 속성이 대상자에 포함된 프로필 수와 함께 표시됩니다. 다음을 사용하여 언제든지 대상자 수를 새로 고칠 수 있습니다. **[!UICONTROL 계산]** 단추를 클릭합니다.

다음 **[!UICONTROL 데이터]** 탭에서는 대상의 일부인 프로필을 표시할 수 있습니다. 열을 더 추가하여 이 보기를 사용자 지정하거나 고급 필터를 활용하여 표시된 데이터를 구체화할 수 있습니다.

![](assets/audiences-details.png)

대상을 복제하거나 삭제하려면 **[!UICONTROL 추가 작업]** 버튼은 대상자 이름 옆의 대상자 목록 또는 대상자 세부 사항 화면 내에서 사용할 수 있습니다.