---
audience: end-user
title: 테스트 이메일 전송
description: 테스트 이메일 정의 및 전송 방법 알아보기
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="알파"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 39%

---

# 테스트 이메일 전송 {#send-test-emails}

**[!UICONTROL Adobe Campaign]** 을(를) 사용하면 메시지를 주요 대상자에게 보내기 전에 테스트할 수 있습니다.

테스트 이메일 전송은 이메일 캠페인을 검증하고 잠재적인 문제를 식별하는 중요한 단계입니다.

테스트 수신자는 링크, 옵트아웃 링크, 이미지 및 미러 페이지와 같은 다양한 요소를 확인할 수 있을 뿐만 아니라 렌더링, 콘텐츠, 개인화 설정 및 이메일 구성에서 오류를 감지할 수 있습니다.

## 테스트 수신자 선택 {#test-recipients}

두 가지 유형의 수신자에게 테스트 이메일을 전송할 수 있습니다.

* **테스트 프로필** - 데이터베이스에서 추가적인 가상 수신자인 시드 주소로 테스트 이메일을 보냅니다. 에서 만들 수 있습니다. [!DNL Campaign] 콘솔을 **[!UICONTROL 리소스]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 시드 주소]** 폴더를 삭제합니다. 다음에서 자세히 알아보기 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* **주 대상에서 대체** - 기존 프로필을 가장하는 동안 테스트 이메일을 특정 이메일 주소로 보냅니다. 이렇게 하면 수신자와 같은 이메일을 경험할 수 있으므로 프로필이 받을 메시지를 정확하게 파악할 수 있습니다.

전자 메일 테스트의 수신자를 선택하려면 아래 단계를 따르십시오.

1. 이메일 액세스 [콘텐츠 편집](../content/edit-content.md) 화면 또는 [이메일 디자이너](../content/get-started-email-designer.md)을(를) 클릭하고 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

1. 다음을 클릭합니다. **[!UICONTROL 테스트]** 단추를 클릭합니다.

   ![](assets/simulate-test-button.png)

1. **[!UICONTROL 모드]** 드롭다운 목록을 사용하면 테스트 이메일을 받는 수신자의 유형을 선택할 수 있습니다.

   * **테스트 프로필** 가상 수신자를 타겟팅하려면

   * **주 대상에서 대체** 기존 프로필의 데이터를 표시하는 동안 특정 이메일 주소로 테스트를 보냅니다.

   ![](assets/simulate-profile-mode.png)

   >[!NOTE]
   >
   >기본적으로 **[!UICONTROL 테스트 프로필 사용]** 모드 가 선택되었습니다. 콘텐츠 시뮬레이션 화면에서 이메일을 미리 볼 프로필을 이미 선택했다면 해당 프로필이 테스트 수신자로 미리 선택되어 있습니다. 선택을 취소하거나 수신자를 추가할 수 있습니다.

1. 대체 프로필로 테스트 이메일을 보내려면 다음을 선택합니다. **[!UICONTROL 대상에서 대체]** 을 클릭하고 다음 단계를 수행합니다.

   1. **[!UICONTROL 주소 추가]** 버튼을 클릭하고 테스트 이메일을 수신하는 이메일 주소를 지정합니다.

      원하는 모든 이메일 주소를 입력할 수 있습니다. 이에 따라 사용자가 아님에도 모든 사용자에게 테스트 이메일을 보낼 수 있습니다. [!DNL Adobe Campaign].

   1. 대용으로 사용할 대상에서 프로필을 선택합니다. 다음 작업을 수행할 수도 있습니다 [!DNL Adobe Campaign] 대상에서 임의 프로필을 선택합니다. 선택한 프로필의 프로필 데이터가 테스트 이메일에 표시됩니다.

   1. 수신자를 확인하고 작업을 반복하여 필요한 만큼 주소를 추가합니다.

      ![](assets/simulate-profile-substitute.png)

1. 테스트 수신자를 선택하면 다음과 같은 작업을 수행할 수 있습니다. [테스트 이메일 보내기](#send-test).

   >[!NOTE]
   >
   >테스트 전자 메일의 수신자에게 최종 전자 메일 메시지를 보내려면 **[!UICONTROL 기본 대상에 테스트 모집단 포함]** 옵션을 선택합니다.

## 테스트 이메일 전송 {#send-test}

선택한 수신자에게 테스트 이메일을 보내려면 아래 단계를 따르십시오.

1. 클릭 **[!UICONTROL 테스트 이메일 보내기]**.

1. 전송을 확인합니다.

   ![](assets/simulate-send-test.png)

1. 게재 콘텐츠를 완료할 때까지 필요한 만큼 테스트 이메일을 전송합니다.

이 작업이 완료되면 다음을 수행할 수 있습니다. [이메일 준비 및 보내기](../monitor/prepare-send.md) 주 타겟으로

## 전송된 테스트 이메일에 액세스 {#access-proofs}

테스트 이메일을 전송한 다음에는 **[!UICONTROL 테스트 이메일 로그 보기]** 버튼으로 전용 로그에 액세스할 수 있습니다.

이러한 로그를 사용하면 선택한 게재에 전송된 모든 테스트 이메일에 액세스하고 해당 전송과 관련된 특정 통계를 시각화할 수 있습니다. [게재 로그 모니터링 방법 알아보기](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

에서 전송된 테스트 이메일에 액세스할 수도 있습니다. [게재 목록](../msg/gs-messages.md)다른 게재와 마찬가지로

![](assets/simulate-deliveries-list.png)
