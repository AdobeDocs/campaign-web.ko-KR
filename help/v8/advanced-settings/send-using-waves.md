---
audience: end-user
title: 웨이브를 사용하여 보내기
description: Campaign 웹에서 게재 설정에 대해 자세히 알아보기
feature: Email
exl-id: d4cd5fe5-f9ac-44ac-a961-ae45131aeb3e
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 13%

---

# 예약된 일괄 처리를 사용하여 보내기 {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="게재를 여러 배치로 분할"
>abstract="동시에 많은 양의 메시지를 보내는 대신, 게재를 여러 배치로 분할하는 예약된 일괄 처리를 정의합니다. 동일한 크기의 여러 예약된 일괄 처리를 구성하거나, 다른 예약된 일괄 처리가 전송되도록 캘린더를 설정할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="각 예약된 일괄 처리의 크기 정의"
>abstract="추가하는 모든 예약된 일괄 처리의 크기를 입력해야 합니다. 숫자 값(각 예약된 일괄 처리의 메시지 수) 또는 백분율(0~100%)을 입력하십시오."

로드 밸런싱을 위해 이메일 게재를 여러 배치로 나눌 수 있습니다. 두 예약된 일괄 처리 수와 전체 게재 대비 배치 수 및 배치 비율을 구성하고 예약된 일괄 처리 간격을 구성합니다.

>[!NOTE]
>
>크기와 두 연속 예약된 예약된 예약된 일괄 처리 사이의 지연 시간만 정의할 수 있습니다. 각 웨이브에 대한 수신자 선택 기준은 조정할 수 없습니다.

웨이브를 사용하여 게재를 보내려면 아래 단계를 따르십시오.

1. [게재 설정](delivery-settings.md#retries)을 엽니다.

1. **[!UICONTROL 배달]** 섹션으로 이동합니다.

1. **[!UICONTROL 다중 웨이브를 사용하여 보내기]** 옵션을 선택하십시오.

1. 웨이브를 구성하려면 다음 중 하나를 수행할 수 있습니다.

   * [동일한 크기의 예약된 일괄 처리 예약](#waves-same-size)
   * [캘린더에 따라 일괄 처리 예약](#waves-calendar)

1. 평소대로 게재를 준비하고 보내십시오. [자세히 알아보기](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >마지막 전파가 [유효성](delivery-settings.md#validity) 탭에 정의된 배달 기한을 초과하지 않도록 하십시오. 그렇지 않으면 일부 메시지가 전송되지 않을 수 있습니다. 특정 유형화 제어 규칙인 **[!UICONTROL 예약된 일괄 처리 확인]**&#x200B;은(는) 게재 유효성 제한 전에 마지막 일괄 처리가 계획되도록 합니다. [Campaign v8(클라이언트 콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=ko)에서 제어 규칙에 대해 자세히 알아보세요.
   >
   >마지막 웨이브를 구성할 때 재시도 시간도 충분히 허용해야 합니다. [자세히 알아보기](delivery-settings.md#retries)

1. 전송을 모니터링하려면 [게재 로그](../monitor/delivery-logs.md)(으)로 이동하세요. 이미 처리된 웨이브로 전송된 게재(**[!UICONTROL 전송됨]** 상태)와 나머지 웨이브로 전송할 게재(**[!UICONTROL 보류 중]** 상태)를 볼 수 있습니다.

## 동일한 크기의 예약된 일괄 처리 예약 {#waves-same-size}

이 옵션을 선택하면 모든 물결의 크기가 같고(마지막 물결 제외) 각 물결 사이의 지연 시간은 항상 동일합니다.

![크기가 같은 파동의 예](assets/waves-same-size.png){zoomable="yes"}

* 게재를 분할할 모든 웨이브의 크기를 지정합니다. 백분율이나 숫자 값을 입력할 수 있습니다. 마지막 웨이브만 나머지 메시지 수를 포함해야 하므로 크기가 달라질 수 있습니다.

  예를 들어 **[!UICONTROL 예약된 일괄 처리 크기]** 필드에 **[!UICONTROL 30%]**&#x200B;을(를) 입력하면 처음 세 예약된 일괄 처리는 배달에 포함된 모든 메시지의 30%를 나타내고 네 번째 예약된 일괄 처리는 나머지 10%를 나타냅니다.

* **[!UICONTROL 간격]** 섹션에서 연속되는 두 예약된 일괄 처리 시작 사이의 지연 시간을 지정하십시오. 예를 들어 **[!UICONTROL 2일]**&#x200B;을 입력하면 첫 번째 물결이 즉시 시작되고 두 번째 물결이 이틀 후에 시작되며 세 번째 물결이 4일 후에 시작됩니다.

동일한 크기의 예약된 일괄 처리를 사용하는 한 가지 일반적인 사용 사례는 콜센터와 관련된 것입니다. 전화 충성도 캠페인을 관리할 때 조직에서는 구독자에게 연락하는 호출 수를 처리하는 데 제한이 있습니다.

웨이브를 사용하여 메시지 수를 콜센터의 일일 처리 용량인 하루에 20개로 제한할 수 있습니다.

이렇게 하려면 **[!UICONTROL 같은 크기의 예약된 예약된 예약된 예약된 예약된 예약된 예약된 일괄 처리]** 옵션을 선택하십시오. 예약된 일괄 처리 크기로 **[!UICONTROL 20]**&#x200B;을(를) 입력하고 **[!UICONTROL 간격]** 필드에 **[!UICONTROL 1일]**&#x200B;을(를) 입력합니다.

![콜센터 처리를 위한 웨이브의 예](assets/waves-call-center.png){zoomable="yes"}

## 캘린더에 따라 일괄 처리 예약 {#waves-calendar}

이 옵션을 선택하는 경우 전송할 각 웨이브의 시작 날짜/시간과 각 웨이브의 크기를 정의합니다.

* **[!UICONTROL 시작]** 필드에서 연속되는 두 예약된 일괄 처리 시작 사이의 지연 시간을 지정합니다.

* **[!UICONTROL Size]** 열에 고정 숫자 또는 백분율을 입력합니다.

필요한 만큼 웨이브를 추가합니다. 요구 사항에 따라 순서를 변경합니다.

>[!NOTE]
>
>백분율을 사용하는 경우 모든 파동의 합계는 100%를 초과할 수 없습니다.

아래 예에서, 제1 웨이브는 게재에 포함된 총 메시지 수의 25%를 나타내며 즉시 시작한다. 다음 두 파동은 배달을 완료하고 6시간 간격으로 시작하도록 설정된다.

![일정으로 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 일괄 작업의 예](assets/waves-calendar.png){zoomable="yes"}

캘린더에 따라 여러 웨이브를 사용하는 일반적인 사용 사례 중 하나는 램프 업 프로세스 도중입니다.

새로운 플랫폼을 사용해 이메일을 보낼 때 인터넷 서비스 제공자(ISP)는 인지되지 않은 IP 주소를 의심하게 된다. 대량의 이메일이 갑자기 전송되면 ISP는 해당 이메일을 스팸으로 표시하는 경우가 많습니다.

스팸으로 표시되지 않도록 하기 위해 웨이브를 사용하여 전송된 볼륨을 점진적으로 늘립니다. 이렇게 하면 시작 단계가 원활하게 발전하고 잘못된 주소의 전체 비율을 줄일 수 있습니다.

이렇게 하려면 **[!UICONTROL 일정에 따라 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 예약된 일괄 처리]** 옵션을 사용합니다. 예를 들어 첫 번째 물결을 10%로 설정하고, 두 번째 물결을 15%로 설정하고, 세 번째 물결을 20%로 설정하는 식입니다.

![램프 업 프로세스용 웨이브의 예](assets/waves-ramp-up.png){zoomable="yes"}