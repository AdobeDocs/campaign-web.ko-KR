---
audience: end-user
title: Adobe Experience Platform 대상자 사용
description: Adobe Experience Platform에서 대상자를 사용하는 방법 알아보기
badge: label="제한 공개"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 703196ad2bb504eb1d50008af110f952d8045eaa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 28%

---

# Adobe Experience Platform 대상자 사용{#aep-audience}

Adobe Campaign 관리 Cloud Service 대상 및 소스 커넥터를 사용하면 Adobe Campaign과 Adobe Experience Platform 간의 원활한 통합을 수행할 수 있습니다.

Adobe Experience Platform 대상자를 만들어 클라이언트 콘솔에서 사용할 수 있게 되면 캠페인 대상자가 메시지를 개인화하고 전송하는 것과 동일한 방식으로 사용할 수 있습니다.

>[!NOTE]
>
>Campaign에서 Adobe Experience Platform 대상을 사용하려면 Adobe 소스 및 대상과의 통합을 구성해야 합니다. 을(를) 참조하십시오 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

게재 대상자를 선택하기 위해 다음을 수행할 수도 있습니다.

* 새 대상을 작성합니다. [자세히 알아보기](../query/query-modeler-overview.md)
* 외부 파일에서 대상자를 로드합니다. [자세히 알아보기](file-audience.md)
* 기존 캠페인 대상자를 사용합니다. [자세히 알아보기](add-audience.md)

게재할 Adobe Experience Platform 대상을 선택하려면 아래 단계를 따르십시오.

1. 게재 생성 도우미의 **대상자** 섹션에서 **[!UICONTROL 대상자 선택]** 버튼을 클릭합니다.

   ![](assets/create-audience.png)

1. 기존 대상자를 사용하려면 **[!UICONTROL 대상자 선택]**&#x200B;을 선택합니다. 이 이메일에서 사용할 새 대상자를 만들려면 **직접 만들기**&#x200B;를 선택합니다. 이 [섹션](../query/query-modeler-overview.md)을 참조하십시오.

   이 화면에는 현재 폴더에 대해 Adobe Campaign 클라이언트 콘솔에 정의된 모든 기존 대상자가 표시됩니다. Adobe Experience Platform에서 대상을 선택하려면 `AEP Audiences folder` 을 클릭합니다.

   ![](assets/select-audience-folder.png)

   다음과 같이 대상의 출처를 기준으로 필터링하는 규칙을 정의할 수도 있습니다.

   필터 섹션에서 필터링 옵션에 액세스하여 대상자 목록을 세분화할 수 있습니다. 이렇게 하려면 다음을 클릭하십시오. **규칙 추가** 대상자 목록에 대한 고급 필터를 만들 수 있는 쿼리 모델러에 액세스합니다. [쿼리 모델러를 사용하는 방법 알아보기](../query/query-modeler-overview.md)

   ![](assets/filter-on-aep-audience.png)

1. 대상자를 선택하고 **선택**&#x200B;을 클릭합니다.

1. 대상자를 세분화하려면 **규칙 편집**&#x200B;을 클릭합니다.

   ![](assets/refine-audience.png)

1. 쿼리 모델러를 사용하면 추가 필터로 대상자를 보강하거나 서로 다른 대상자를 결합하여 대상자를 보강할 수 있습니다. 이 [섹션](../query/query-modeler-overview.md)을 참조하십시오.

1. **저장**&#x200B;을 클릭합니다.
