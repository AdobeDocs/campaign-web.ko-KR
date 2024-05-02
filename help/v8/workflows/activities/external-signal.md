---
audience: end-user
title: 외부 신호 활동 사용
description: 외부 신호 워크플로우 활동을 사용하는 방법 알아보기
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 3%

---

# 외부 신호 {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="외부 신호"
>abstract="다음 **외부 신호** 활동을 사용하면 다른 워크플로우 또는 API 호출에서 워크플로우 실행을 트리거할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="외부 신호 매개변수"
>abstract="외부 신호 매개변수"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="종료 트리거"
>abstract="종료 트리거"

다음 **외부 신호** 활동은 입니다. **흐름 제어** 활동. 다른 워크플로우 또는 API 호출에서 워크플로우 실행을 트리거할 수 있습니다.

>[!NOTE]
>
>이 페이지에서는 을(를) 구성하는 주요 단계를 설명합니다. **[!UICONTROL 외부 신호]** campaign 웹 사용자 인터페이스의 활동으로 다른 워크플로우 또는 API 호출에서 트리거합니다. 워크플로우를 트리거하는 방법, 모범 사례 및 Campaign API로 작업하는 방법에 대한 자세한 내용은 [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

다음 단계에 따라 **외부 신호** 활동 및 그 실행 트리거:

1. 추가 **외부 신호** 활동을 워크플로우에 추가합니다.

1. 워크플로우의 구성을 완료하고 실행을 시작합니다. 다음 **[!UICONTROL 외부 신호]** 활동이 &quot;보류 중&quot;으로 표시되며 트리거되기를 기다립니다.

   ![](../assets/external-signal-pending.png)

1. 아래 정보를 검색하십시오.

   * 다음 **워크플로우의 내부 이름**&#x200B;레이블 옆에 표시되는 변수입니다.

     +++보기 예

     ![](../assets/external-signal-workflow-name.png)

+++

   * 다음 **외부 신호 활동 이름**: 워크플로우에 표시됩니다. **[!UICONTROL 실행 옵션]**.

     +++보기 예

     ![](../assets/external-signal-name.png)

+++

1. 워크플로우를 트리거하려면 다음을 실행해야 합니다. `PostEvent` JavaScript 함수. 이 함수를 사용하면 선택한 값과 함께 변수를 전달하고 트리거된 워크플로우에서 활용할 수 있습니다.

   다음 `PostEvent` 함수는 다른 워크플로우 또는 API 호출에서 실행할 수 있습니다.

   * 를 트리거하려면 **[!UICONTROL 외부 신호]** 워크플로우의 활동으로, 다음에서 PostEvent 함수를 실행합니다. **[!UICONTROL 초기화 스크립트]** 창에서 액세스할 수 있습니다. **[!UICONTROL 실행 옵션]**. 의 경우 **[!UICONTROL JavaScript 코드]** 활동, 활동의 스크립트에서 함수를 실행합니다.

     구문은 다음과 같습니다.

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++보기 예

   이 예제에서는 내부 이름이 &quot;WKF12345&quot;인 워크플로우에 추가된 &quot;signal1&quot; 외부 신호 활동을 트리거합니다. 또한 값이 &quot;123456&quot;인 &quot;customID&quot;라는 변수를 전달하고 있습니다.

   ![](../assets/external-signal-sample.png)

+++

   * 를 트리거하려면 **[!UICONTROL 외부 신호]** API 호출의 활동은 Campaign API 설명서에 자세히 설명된 단계를 따릅니다. [정적 을 사용하는 방법 알아보기 `PostEvent` 방법](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
