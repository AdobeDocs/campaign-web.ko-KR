---
audience: end-user
title: 테스트 게재 보내기
description: 테스트 게재를 정의하고 전송하는 방법을 알아봅니다
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="알파"
source-git-commit: 7c9388d5a406779f91180835e39e6dd2408d8a90
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 4%

---

# 테스트 게재 보내기 {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="미리보기 모드"
>abstract="기본 대상에 테스트 모집단을 포함하여 메시지를 미리 보고 테스트합니다."

**[!UICONTROL Adobe Campaign]** 을(를) 사용하면 메시지를 주요 대상자에게 보내기 전에 테스트할 수 있습니다.

테스트 게재를 전송하는 것은 캠페인을 확인하고 잠재적 문제를 식별하는 중요한 단계입니다.

테스트 수신자는 링크, 옵트아웃 링크, 이미지 또는 미러 페이지와 같은 다양한 요소를 확인할 수 있을 뿐만 아니라 렌더링, 콘텐츠, 개인화 설정 및 게재 구성의 오류를 감지할 수 있습니다.

## 테스트 수신자 선택 {#test-recipients}



>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="테스트 모집단"
>abstract="테스트 모집단 모드를 선택합니다."



사용 중인 채널에 따라 세 가지 유형의 수신자에게 테스트 메시지를 보낼 수 있습니다.

* [테스트 프로필](#test-profiles) - 보내기 **이메일 및 SMS 테스트** 데이터베이스의 추가 수신자인 시드 주소로 변경할 수 있습니다.

  에서 만들 수 있습니다. [!DNL Campaign] 콘솔을 **[!UICONTROL 리소스]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 시드 주소]** 폴더를 삭제합니다. 다음에서 자세히 알아보기 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* [주 대상에서 대체](#substitution-profiles) - 보내기 **이메일 및 SMS 테스트** 기존 프로필을 가장하는 동안 특정 이메일 주소 또는 전화 번호에 연결할 수 있습니다.

  이를 통해 수신자와 마찬가지로 메시지를 경험하여 프로필에서 수신할 콘텐츠를 정확하게 표현할 수 있습니다.

* [구독자](#subscribers) - 보내기 **푸시 알림 테스트** 데이터베이스에 추가된 가상 구독자에 대해 설명합니다.

  테스트 프로필과 마찬가지로 [!DNL Campaign] 콘솔을 **[!UICONTROL 리소스]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 시드 주소]** 폴더를 삭제합니다. 다음에서 자세히 알아보기 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

테스트 게재의 수신자를 선택하려면 사용할 프로필 유형에 따라 아래 단계를 수행합니다.

### 테스트 프로필 {#test-profiles}


1. 이메일 또는 SMS 게재의 콘텐츠 편집 화면으로 이동한 다음 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

1. 다음을 클릭합니다. **[!UICONTROL 테스트]** 단추를 클릭합니다.

   >[!NOTE]
   >
   >이미 다음 프로필을 선택한 경우: [게재 미리 보기](preview-content.md)왼쪽 창에 나열됩니다.

   ![](assets/simulate-test-button-email.png)

1. 다음에서 **[!UICONTROL 모드]** 드롭다운 목록에서 선택 **[!UICONTROL 테스트 프로필]** 테스트 이메일 또는 SMS 게재를 수신할 가상 수신자를 타겟팅하려면 다음을 수행하십시오.

   ![](assets/simulate-profile-mode.png)

1. 이미 다음 프로필을 선택한 경우: [메시지 미리 보기](preview-content.md) 콘텐츠 시뮬레이션 화면에서 해당 프로필은 테스트 수신자로 미리 선택됩니다. 다음을 사용하여 선택 항목을 지우고 수신자를 추가할 수 있습니다. **[!UICONTROL 테스트 프로필 추가]** 단추를 클릭합니다.

   >[!NOTE]
   >
   >기본적으로 **[!UICONTROL 테스트 프로필 사용]** 모드 가 선택되었습니다.

1. 테스트 게재의 수신자에게 최종 메시지를 보내려면 **[!UICONTROL 기본 대상에 테스트 모집단 포함]** 옵션을 선택합니다.

1. 테스트 프로필을 선택하면 다음과 같은 작업을 수행할 수 있습니다. [테스트 게재 보내기](#send-test).

### 대체 프로필 {#substitution-profiles}

의 기존 프로필에서 데이터를 표시하는 동안 특정 이메일 주소 또는 전화번호에 테스트 이메일 또는 SMS를 보내려면 [!DNL Campaign] 데이터베이스, 대체 프로파일을 사용합니다.

1. 테스트를 보내기 전에 게재 대상을 정의했는지 확인하십시오. [자세히 알아보기](../audience/about-audiences.md)

1. 이메일 또는 SMS 게재의 콘텐츠 편집 화면으로 이동한 다음 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

1. 다음을 클릭합니다. **[!UICONTROL 테스트]** 단추를 클릭합니다.

   ![](assets/simulate-test-button-email.png)

1. 다음에서 **[!UICONTROL 모드]** 드롭다운 목록에서 선택 **[!UICONTROL 주 대상에서 대체]** 기존 프로필의 데이터를 표시하는 동안 특정 이메일 주소 또는 전화번호에 테스트를 보냅니다.

   >[!CAUTION]
   >
   >다음을 선택하지 않은 경우 [대상자](../audience/about-audiences.md) 게재를 위해 **[!UICONTROL 주 대상에서 대체]** 옵션이 회색으로 표시되고 대체 프로필을 선택할 수 없습니다.

1. 다음을 클릭합니다. **[!UICONTROL 주소 추가]** 버튼을 클릭하고 테스트 게재를 받을 이메일 주소 또는 전화 번호를 지정합니다.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >이메일 주소 또는 전화 번호를 입력할 수 있습니다. 이렇게 하면 의 사용자가 아닌 수신자에게도 테스트 게재를 보낼 수 있습니다. [!DNL Adobe Campaign].

1. 대용으로 사용할 데이터베이스에서 프로필을 선택합니다. 다음 작업을 수행할 수도 있습니다 [!DNL Adobe Campaign] 임의 프로필을 선택합니다. 선택한 프로필의 프로필 데이터가 테스트 게재에 표시됩니다.

1. 수신자를 확인하고 작업을 반복하여 이메일 주소 또는 전화 번호를 필요한 만큼 추가합니다.

   ![](assets/simulate-profile-substitute.png)

1. 테스트 게재의 수신자에게 최종 메시지를 보내려면 **[!UICONTROL 기본 대상에 테스트 모집단 포함]** 옵션을 선택합니다.

1. 대체 프로파일을 선택하면 다음 작업을 수행할 수 있습니다. [테스트 게재 보내기](#send-test).

### 구독자 {#subscribers}

푸시 알림 작업 시 테스트 게재는 구독자에게만 전송할 수 있습니다. 이를 선택하려면 아래 단계를 따르십시오.

1. 게재의 콘텐츠 편집 화면으로 이동한 다음 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

1. 다음을 클릭합니다. **[!UICONTROL 테스트]** 단추를 클릭합니다.

   ![](assets/simulate-test-button-push.png)

1. 다음에 대한 구독자를 이미 선택한 경우: [게재 미리 보기](preview-content.md) 콘텐츠 시뮬레이션 화면에서 이러한 프로필은 테스트 구독자로 미리 선택됩니다.

   전용 버튼을 사용하여 선택 사항을 지우고 가입자를 추가할 수 있습니다.

   ![](assets/simulate-test-subscribers.png)

1. 테스트 구독자에게 최종 푸시 알림을 보내려면 **[!UICONTROL 기본 대상에 테스트 모집단 포함]** 옵션을 선택합니다.

1. 구독자를 선택하면 다음 작업을 수행할 수 있습니다. [테스트 게재 보내기](#send-test).

## 테스트 게재 보내기 {#send-test}

선택한 수신자에게 테스트 게재를 보내려면 아래 단계를 따르십시오.

1. 다음을 클릭합니다. **[!UICONTROL 테스트 보내기]** 단추를 클릭합니다.

1. 전송을 확인합니다.

   ![](assets/simulate-send-test.png)

1. 게재 콘텐츠를 완료할 때까지 필요한 만큼 테스트를 전송합니다.

완료되면 게재를 준비하고 기본 타겟으로 보낼 수 있습니다. 아래 전용 섹션에서 자세한 내용을 살펴보십시오.

* [이메일 보내기](../monitor/prepare-send.md)
* [푸시 알림 보내기](../push/send-push.md#send-push)
* [SMS 게재 보내기](../sms/send-sms.md#send-sms)

## 전송된 테스트 게재 액세스 {#access-proofs}

테스트 게재가 전송되면 **[!UICONTROL 테스트 로그 보기]** 단추를 클릭합니다.

이러한 로그를 사용하여 선택한 게재에 대해 전송된 모든 테스트에 액세스하고 해당 전송과 관련된 특정 통계를 시각화할 수 있습니다. [게재 로그 모니터링 방법 알아보기](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

다음 위치에서 전송된 테스트에 액세스할 수도 있습니다 [게재 목록](../msg/gs-messages.md)다른 게재와 마찬가지로

![](assets/simulate-deliveries-list.png)
