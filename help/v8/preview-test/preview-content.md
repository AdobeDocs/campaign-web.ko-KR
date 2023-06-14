---
audience: end-user
title: 게재 콘텐츠 미리 보기
description: Campaign 웹 UI를 사용하여 게재 콘텐츠를 미리 보는 방법 알아보기
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="알파"
source-git-commit: 890141a65fcacd0362acda49ff4066961d5ea371
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 10%

---


# 게재 콘텐츠 미리 보기 {#preview-content}

사용 [!DNL Campaign] 콘텐츠 시뮬레이션 기능으로 메시지를 보내기 전에 메시지 콘텐츠를 미리 볼 수 있습니다. 이를 통해 개인화를 제어하고 수신자에게 표시되는 방식을 확인할 수 있습니다.

게재 콘텐츠를 미리 보려면 아래 단계를 따르십시오.

1. 게재의 콘텐츠 편집 화면으로 이동합니다.

   <!--email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).-->

1. 다음을 클릭합니다. **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

   ![](assets/simulate-button.png)

1. 개인화된 콘텐츠를 미리 보는 데 사용할 프로필을 선택하려면 다음을 사용합니다.

   * **[!UICONTROL 테스트 프로필 추가]** 이메일 및 SMS 게재 미리 보기

   * **[!UICONTROL 구독자 추가]** 푸시 알림 미리 보기용

1. 테스트 프로필과 프로필을 결합하여 이메일 또는 SMS 메시지를 미리 볼 수 있습니다.

   * **[!UICONTROL 테스트 프로필]** 탭에는 모든 시드 주소가 나열됩니다. 시드 주소는 데이터베이스의 추가 및 가상 수신자입니다.

     >[!NOTE]
     >
     >테스트 프로필은 [!DNL Campaign] 콘솔을 **[!UICONTROL 리소스]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 시드 주소]** 폴더를 삭제합니다. 다음에서 자세히 알아보기 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * **[!UICONTROL 프로필]** 탭에는 콘솔의 **[!UICONTROL 프로필 및 대상]** 폴더에 저장된 모든 수신자가 나열됩니다. [!DNL Campaign] [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. 클릭 **[!UICONTROL 선택]** 을 클릭하여 선택 항목을 확인합니다.

   게재 콘텐츠 미리보기가 의 오른쪽 창에 표시됩니다. **[!UICONTROL 시뮬레이트]** 화면. 개인화된 요소는 왼쪽 창에서 선택한 프로필의 데이터로 바뀝니다.

   ![](assets/simulate-preview.png)

1. 여러 프로필을 추가한 경우 목록에서 전환하여 해당 게재 콘텐츠를 미리 볼 수 있습니다. 왼쪽 창의 해당 단추를 사용하여 테스트 프로필을 더 추가하고 선택을 취소할 수도 있습니다.

1. 이메일 게재의 경우 다음을 조정할 수 있습니다. **[!UICONTROL 확대/축소 레벨]** 오른쪽 상단의 전용 아이콘을 사용하여 데스크탑 또는 모바일 디바이스에서 콘텐츠를 미리 볼 수 있습니다.

1. 다음에서 **[!UICONTROL 시뮬레이트]** 화면 또한 다음 작업을 수행할 수 있습니다.
   * 유효성 검사를 위해 특정 수신자에게 테스트 게재 보내기 - [자세히 알아보기](proofs.md)
   * 전송된 테스트 게재의 로그에 액세스 - [자세히 알아보기](proofs.md#access-proofs)
   * 이메일의 경우, 방문 빈도가 높은 이메일 클라이언트의 메시지 콘텐츠 렌더링 을 확인합니다. [자세히 알아보기](email-rendering.md)



