---
audience: end-user
title: 구독 서비스 작업
description: Adobe Campaign 웹에서 구독 서비스에 액세스하고, 만들고, 관리하는 방법을 알아봅니다
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: e82c19df7faecbb75521bca54e32b1ba84ea1f81
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 28%

---

# 구독 서비스 만들기 및 관리 {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="서비스 만들기 및 관리"
>abstract="Adobe Campaign을 사용하면 뉴스레터와 같은 서비스를 생성 및 모니터링하고 이러한 서비스에 대한 구독 또는 구독 취소를 확인할 수 있습니다. 구독은 이메일 및 SMS 게재에만 적용됩니다."

Adobe Campaign 웹을 사용하여 뉴스레터와 같은 서비스를 관리 및 생성하고, 이러한 서비스의 구독 또는 구독 취소를 확인하십시오.

예를 들어 특정 제품 카테고리, 테마 또는 웹 사이트 영역에 대한 뉴스레터, 다양한 유형의 경고 메시지 구독 및 실시간 알림과 같은 여러 서비스를 동시에 정의할 수 있습니다.

>[!NOTE]
>
>구독은 이메일 및 SMS 게재에만 적용됩니다.

## 구독 서비스 액세스 {#access-services}

플랫폼에서 사용할 수 있는 구독 서비스에 액세스하려면 아래 단계를 따르십시오.

1. **[!UICONTROL 고객 관리]**&#x200B;에서 왼쪽 탐색 레일의 **[!UICONTROL 구독 서비스]** 메뉴로 이동합니다.

   ![고객 관리 아래 왼쪽 탐색 레일에 구독 서비스 메뉴를 표시하는 스크린샷](assets/service-list.png){zoomable="yes"}

1. 모든 기존 구독 서비스 목록이 표시됩니다. [쿼리 모델러](../query/query-modeler-overview.md)를 사용하여 서비스를 검색하고 채널, 폴더 또는 규칙을 추가할 수 있습니다.

   ![채널, 폴더 및 규칙에 대한 필터가 있는 구독 서비스 목록을 표시하는 스크린샷](assets/service-filters.png){zoomable="yes"}

1. 기존 서비스를 편집하려면 해당 이름을 클릭합니다.

1. 서비스 이름 옆에 있는 세 점 아이콘을 사용하여 서비스를 삭제하거나 복제합니다.<!--so all subscribers are unsubscribed - need to mention?-->

## 첫 구독 서비스 만들기 {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="서비스 속성 정의"
>abstract="구독 서비스의 레이블을 입력하고 서비스 유효 기간과 같은 추가 옵션을 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="확인 메시지 선택"
>abstract="사용자가 서비스를 구독하거나 구독 취소하면 확인 메시지를 전송할 수 있습니다. 확인 메시지에 사용할 템플릿을 선택합니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="기본 랜딩 페이지"
>abstract="이 서비스와 연결된 기본 랜딩 페이지를 선택합니다."

구독 서비스를 만들려면 아래 단계를 수행하십시오.

1. **[!UICONTROL 구독 서비스 만들기]** 단추를 선택하십시오.

   ![구독 서비스 만들기 단추를 보여주는 스크린샷](assets/service-create-button.png){zoomable="yes"}

1. 채널 선택: **[!UICONTROL 이메일]** 또는 **[!UICONTROL SMS]**.

1. 서비스 속성에서 레이블을 입력하고 필요에 따라 **[!UICONTROL 추가 옵션]**&#x200B;을(를) 정의합니다.

   ![레이블 및 추가 옵션이 있는 서비스 속성 섹션을 보여 주는 스크린샷](assets/service-create-properties.png){zoomable="yes"}

1. 기본적으로 서비스는 **[!UICONTROL 서비스 및 구독]** 폴더에 저장됩니다. 원하는 위치로 이동하여 변경할 수 있습니다. [폴더 작업 방법 알아보기](../get-started/permissions.md#folders)

1. 기본적으로 구독은 무제한입니다.

   **[!UICONTROL 무제한 유효 기간]** 옵션을 비활성화하여 서비스 유효 기간을 정의하십시오. 유효 기간이 종료되면:
   * 더 이상 이 서비스를 구독할 수 있는 프로필이 없습니다.
   * 이 서비스의 모든 구독자는 자동으로 구독 취소됩니다.

   ![구독 서비스에 대한 유효 기간 설정을 보여 주는 스크린샷](assets/service-create-validity-period.png){zoomable="yes"}

1. 사용자가 서비스를 구독하거나 구독 취소하면 확인 메시지를 전송할 수 있습니다. 사용 사례에 따라 해당 메시지에 사용할 템플릿을 선택합니다. 이러한 템플릿은 **[!UICONTROL 구독]** 대상 매핑으로 구성해야 합니다. [자세히 알아보기](#create-confirmation-message)

   ![확인 메시지 템플릿 선택을 보여 주는 스크린샷](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. **[!UICONTROL 저장 및 검토]**&#x200B;를 클릭합니다. 새 서비스가 **[!UICONTROL 구독 서비스]** 목록에 추가되었습니다.

1. 이 서비스와 연결된 기본 구독 및 구독 취소 랜딩 페이지를 선택합니다.

   ![구독 서비스에 대한 기본 랜딩 페이지 설정을 보여 주는 스크린샷](assets/service-create-default-lp.png){zoomable="yes"}

   완료되면, [메일에 링크 삽입](../email/message-tracking.md)할 때 **[!UICONTROL 구독 링크]** 또는 **[!UICONTROL 구독 취소 링크]**&#x200B;를 선택하세요. 해당 링크를 클릭하면 서비스에서 참조한 구독 또는 구독 취소 랜딩 페이지로 이동합니다. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

   ![구독 및 구독 취소 링크 설정을 보여 주는 스크린샷](assets/service-create-default-lp-link.png){zoomable="yes"}

1. 변경 사항을 저장하고 검토합니다.

이제 다음을 수행할 수 있습니다.

* 이 서비스에 가입자를 수동으로 추가하고 프로필 가입을 취소합니다. [자세히 알아보기](../audience/manage-subscribers.md)

* 고객을 랜딩 페이지를 통해 이 서비스에 가입하도록 초대합니다. [자세히 알아보기](../landing-pages/lp-use-cases.md#lp-subscription)

* 이 서비스의 구독자에게 메시지를 보냅니다. [방법 알아보기](../msg/send-to-subscribers.md)

## 확인 메시지 만들기 {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="구독 게재 템플릿 선택"
>abstract="서비스를 구독하는 사용자에게 확인 메시지를 보내려면 정의된 대상 없이 **[!UICONTROL 구독]** 대상 매핑을 기반으로 특정 게재 템플릿을 선택해야 합니다."

>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="구독 취소 게재 템플릿 선택"
>abstract="서비스 구독을 취소하는 사용자에게 확인 메시지를 보내려면 정의된 대상 없이 **[!UICONTROL 구독]** 대상 매핑을 기반으로 특정 게재 템플릿을 선택해야 합니다."

서비스를 구독하거나 구독을 취소하는 사용자에게 확인 메시지를 보내려면 정의된 대상 없이 **[!UICONTROL 구독]** 대상 매핑으로 게재 템플릿을 만드십시오. 아래의 단계를 수행하십시오.

1. 구독 확인을 위한 게재 템플릿을 만듭니다. [템플릿을 만드는 방법 알아보기](../msg/delivery-template.md)

1. 이 게재의 대상자를 선택하지 마십시오. 대신 게재 **[!UICONTROL 설정]**&#x200B;에 액세스하고 [대상자](../advanced-settings/delivery-settings.md#audience) 탭으로 이동한 다음 목록에서 **[!UICONTROL 구독]** 대상 매핑을 선택합니다.

   ![게재 템플릿에 대한 대상 매핑 선택을 보여 주는 스크린샷](assets/service-confirmation-template-mapping.png){zoomable="yes"}

   >[!NOTE]
   >
   >**[!UICONTROL 구독]** 대상 매핑을 선택하지 않으면 구독자에게 확인 메시지가 표시되지 않습니다. [이 섹션](../audience/targeting-dimensions.md)에서 대상 매핑에 대해 자세히 알아보세요.

1. 게재 템플릿의 콘텐츠를 편집하고 저장하고 닫습니다.

   ![게재 템플릿에 대한 콘텐츠 편집기를 보여 주는 스크린샷](assets/service-confirmation-template.png){zoomable="yes"}

   >[!NOTE]
   >
   >[전자 메일 채널](../email/create-email.md) 및 [SMS 채널](../sms/create-sms.md) 섹션에서 게재 채널 및 게재 콘텐츠를 정의하는 방법에 대해 자세히 알아보세요.

1. 구독 취소 확인을 위한 게재 템플릿을 만들려면 위의 단계를 반복하십시오.

이제 [구독 서비스를 만드는 중](#create-service)에 이러한 메시지를 선택할 수 있습니다. 해당 서비스를 구독하거나 구독 취소하는 사용자는 선택한 확인 메시지를 받게 됩니다.

## 구독 서비스 모니터링 {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="구독자 수"
>abstract="이 서비스의 총 구독자 수를 확인하려면 **계산**&#x200B;을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="총 구독자 수"
>abstract="주요 성과 지표(KPI)는 구독자 기반에 대한 포괄적인 보기를 제공하여 이 서비스를 구독한 개인의 총 수를 보여 줍니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="해당 기간의 구독 수"
>abstract="드롭다운 목록을 사용하여 기간을 변경하고 선택한 기간 동안의 구독 및 구독 취소 수를 확인합니다."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="구독의 전반적인 진화"
>abstract="이 그래프는 구독, 구독 취소, 숫자 변화, 충성도 비율 등 기간별 분류를 보여 줍니다."

SMS 및 이메일 채널에 대한 구독 서비스의 효과를 측정하려면 주어진 서비스에 대한 로그 및 보고서에 액세스합니다.

1. **[!UICONTROL 구독 서비스]** 목록에서 기존 서비스를 선택하십시오. 총 구독자 수를 가져오려면 **[!UICONTROL 계산]**&#x200B;을 클릭하세요.

   ![총 구독자 수 계산을 보여 주는 스크린샷](assets/service-logs-subscribers-count.png){zoomable="yes"}

1. 서비스 대시보드에서 **[!UICONTROL 로그]**&#x200B;를 선택하여 이 서비스의 구독자 목록을 봅니다.

   전체 가입자 수, 각 수신자의 이름과 주소, 가입 또는 가입 해지 시 확인이 가능하다. 필터링할 수도 있습니다.

   ![구독자 세부 정보가 포함된 로그 섹션을 보여 주는 스크린샷](assets/service-logs.png){zoomable="yes"}

1. 서비스 대시보드에서 **[!UICONTROL 보고서]**&#x200B;를 선택합니다. 다음 지표를 확인하십시오.

   * **[!UICONTROL 총 구독자 수]**&#x200B;가 표시됩니다.

   * 선택한 기간 동안의 구독 및 구독 취소 수를 봅니다. 드롭다운 목록을 사용하여 시간 범위를 변경합니다.

     ![구독 및 구독 취소 데이터가 있는 보고서 섹션을 보여 주는 스크린샷](assets/service-reports.png){zoomable="yes"}

   * **[!UICONTROL 구독의 전체 진화]** 그래프는 구독, 구독 취소, 숫자 진화 및 충성도 비율을 포함하여 기간별 분류를 표시합니다.<!--what is Registered?-->

1. **[!UICONTROL 다시 로드]** 단추를 사용하여 추적 워크플로우의 실행 및 일정에서 최신 값을 검색합니다.