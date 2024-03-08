---
audience: end-user
title: 대상자 모니터링 및 관리
description: Adobe Campaign 웹에서 대상자를 모니터링하고 관리하는 방법 알아보기
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 23%

---

# 대상자 모니터링 및 관리 {#monitor-manage}

## 대상자란 무엇입니까? {#what}

대상자는 게재의 주요 타겟인 메시지를 받는 프로필입니다. 대상자의 유형은 게재 템플릿에 정의된 대상 매핑에 따라 다릅니다. 에서 게재 템플릿에 대해 자세히 알아보기 [이 페이지](../msg/delivery-template.md).

대상자의 모집단을 정의하려면 다음을 수행할 수 있습니다.

* [새 대상 만들기](create-audience.md) 다음에서 **[!UICONTROL 대상]** 메뉴,
* [기존 대상자 선택](add-audience.md) 클라이언트 콘솔에 목록으로 만들어지거나 Adobe Experience Platform에서 가져옴
* [새 대상 작성](../query/query-modeler-overview.md) 필터링 기준을 정의하고 결합하여 쿼리 모델러로
* [외부 파일의 대상자 사용](file-audience.md). 이 옵션은 독립형 이메일 게재에만 사용할 수 있으며 캠페인 게재에는 사용할 수 없습니다.

대상자를 타깃팅할 때 다음을 정의할 수도 있습니다. **컨트롤 그룹** 대상자의 일부에 메시지를 보내지 않도록 하고 캠페인의 영향을 측정합니다. [컨트롤 그룹을 설정하는 방법 알아보기](control-group.md)

>[!NOTE]
>
>캠페인 워크플로우의 컨텍스트에서 메시지를 보낼 때 대상자는 특정 대상에 정의됩니다 **대상자 작성** 워크플로우 활동. 이 컨텍스트에서는 이메일 게재용 파일에서 대상자를 로드할 수 없으며, 대상자는 이 전용 활동에서만 정의됩니다. 캠페인 워크플로우에서 게재 대상을 정의하는 방법을 알아봅니다. [이 섹션](../workflows/activities/build-audience.md)

## 대상자 모니터링 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="속성"
>abstract="여기에서 원본, 스토리지 폴더 또는 상태 등 대상자 속성에 대한 요약을 확인할 수 있습니다. 대상자를 만드는 데 사용된 워크플로를 열려면 **마지막 워크플로** 섹션의 링크를 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="대상자 크기"
>abstract="여기서 대상자 내의 총 프로필 수를 확인할 수 있습니다. 대상자 결과를 업데이트하고 다시 계산하려면 ‘계산’ 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="대상자 오류"
>abstract="대상자 데이터를 사용할 수 없습니다. 워크플로 실행이 종료될 때까지 기다려 주십시오."

Campaign 웹에서 사용할 수 있는 대상자 목록은 **[!UICONTROL 대상]** 메뉴 아래의 제품에서 사용할 수 있습니다.

![](assets/audiences-list.png){zoomable=&quot;yes&quot;}

대상은 여러 소스에서 발생할 수 있습니다. 다음 **[!UICONTROL 원본]** 열은 지정된 대상이 만들어진 위치를 나타냅니다.

* **[!UICONTROL Adobe Campaign]**: 이러한 대상은 Adobe Campaign V8 콘솔에서 만들어집니다. 다음에서 자세히 알아보기 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** 이러한 대상은 Adobe Experience Platform 내에서 생성되며 Adobe 소스 및 대상 통합을 사용하여 Campaign 웹에 통합됩니다. 에서 이 통합을 설정하는 방법에 대해 알아봅니다. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

  ➡️ [비디오에서 이 기능 살펴보기](#video)

* **[!UICONTROL Adobe Campaign WebUI]**: 이러한 대상자는 Campaign 웹 대상자 워크플로우를 사용하여 만들어집니다. [대상자를 만드는 방법 알아보기](create-audience.md)

대상자에 대한 자세한 내용을 보려면 목록에서 대상자를 여십시오. 대상자 속성이 대상자에 포함된 프로필 수와 함께 표시됩니다. 다음을 사용하여 언제든지 대상자 수를 새로 고칠 수 있습니다. **[!UICONTROL 계산]** 단추를 클릭합니다.

다음 **[!UICONTROL 데이터]** 탭에서는 대상의 일부인 프로필을 표시할 수 있습니다. 열을 더 추가하여 이 보기를 사용자 지정하거나 고급 필터를 활용하여 표시된 데이터를 구체화할 수 있습니다.

![](assets/audiences-details.png){zoomable=&quot;yes&quot;}

대상을 복제하거나 삭제하려면 **[!UICONTROL 추가 작업]** 버튼은 대상자 이름 옆의 대상자 목록 또는 대상자 세부 사항 화면 내에서 사용할 수 있습니다.

## 방법 비디오 {#video}

Adobe Campaign 웹 사용자 인터페이스에서 Experience Platform 대상을 사용할 대상을 만드는 방법을 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Adobe 소스 및 대상 통합을 설정하는 방법에 대한 자세한 내용은에서 확인할 수 있습니다 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.
