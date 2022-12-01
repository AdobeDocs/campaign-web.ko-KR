---
audience: end-user
title: 이메일 준비 및 보내기
description: Campaign v8 웹 설명서
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 2%

---

# 이메일 준비 및 보내기 {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="이메일 준비 및 보내기"
>abstract="이메일을 준비하는 방법과 KPI 보내기에 대한 자세한 내용을 알아봅니다."

>[!NOTE]
>
>이 설명서는 개발 중이며 자주 업데이트됩니다. 이 컨텐츠의 최종 버전은 2023년 1월에 준비될 예정입니다.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## 보내기 준비

준비 중에 대상 모집단을 계산하고 대상에 포함된 각 프로필에 대해 생성된 메시지 콘텐츠를 생성합니다. 준비가 완료되면 즉시 또는 예약된 날짜와 시간에 메시지를 보낼 수 있습니다. 분석 중에 사용되는 검증 규칙은 다음과 같습니다 [섹션](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. 을(를) 클릭합니다. **준비** 오른쪽 상단 모서리에 있는 단추.

1. 준비 진행률이 표시됩니다. 타겟팅된 모집단의 크기에 따라 이 작업은 시간이 좀 걸릴 수 있습니다.

   >[!NOTE]
   >
   >언제든지 **준비 중지** 버튼을 클릭합니다. 준비 단계 동안 메시지가 전송되지 않습니다. 따라서 어떤 것이든 영향을 주지 않고 이 작업을 시작하거나 중지할 수 있습니다.

1. 준비가 완료되면 을(를) 확인합니다. **타깃팅됨**, **게재하려면** 및 **제외하려면** KPI. 전송할 메시지 수가 예상과 일치하지 않는 경우 대상을 수정하고 준비를 다시 시작하십시오.

1. 을(를) 클릭합니다. **로그** 버튼을 클릭하고 오류가 없는지 확인합니다. 모든 유효성 검사 단계, 경고 및 오류가 나열됩니다. 색상 아이콘은 메시지 유형을 보여줍니다.

   * 회색 아이콘은 유용한 메시지를 나타냅니다.
   * 노란색 아이콘은 중요하지 않은 처리 오류를 나타냅니다.
   * 빨간색 아이콘은 게재를 보낼 수 없는 중요한 오류를 나타냅니다.

1. 변경한 후 준비를 다시 시작합니다.

준비가 완료되면 메시지를 보낼 수 있습니다. 자세한 내용은 보내기 확인을 참조하십시오.


## 메시지 보내기

준비가 완료되면 아래 절차에 따라 메시지를 보내십시오.

1. 을(를) 클릭합니다. **보내기 단추** 오른쪽 상단 모서리에서 을(를) 확인하고 확인합니다.

1. 전송 진행 상태가 3개의 KPI와 함께 표시됩니다. 전달, 열기, 클릭 수.

1. 확인 단추를 눌러 전송을 완료합니다.

로그

>[!NOTE]
>
>메시지를 예약하면 전송 시간이 되었을 때 전송됩니다. 메시지 예약에 대한 자세한 정보는 이 섹션을 참조하십시오.

