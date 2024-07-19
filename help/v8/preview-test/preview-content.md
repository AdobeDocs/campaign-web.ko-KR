---
audience: end-user
title: 게재 콘텐츠 미리 보기
description: Campaign 웹 사용자 인터페이스를 사용하여 게재 콘텐츠를 미리 보는 방법 알아보기
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---


# 메시지 콘텐츠 미리보기 {#preview-content}

[!DNL Campaign] 콘텐츠 시뮬레이션 기능을 사용하여 메시지를 보내기 전에 메시지 콘텐츠를 미리 봅니다. 이를 통해 개인화를 제어하고 수신자에게 표시되는 방식을 확인할 수 있습니다.

게재 콘텐츠를 미리 보려면 아래 단계를 따르십시오.

1. 게재의 콘텐츠 편집 화면 또는 [전자 메일 Designer](../email/get-started-email-designer.md)(으)로 이동합니다.

1. **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭합니다.

   ![](assets/simulate-button.png){zoomable="yes"}

1. 콘텐츠를 미리 보는 데 사용할 프로필을 선택합니다. 이렇게 하려면 **[!UICONTROL 테스트 프로필 추가]** 단추(전자 메일 및 SMS)나 **[!UICONTROL 구독자 추가]** 단추(푸시 알림)를 클릭합니다.

1. 프로필과 테스트 프로필을 결합하여 이메일 또는 SMS 메시지를 미리 볼 수 있습니다.

   * **[!UICONTROL 테스트 프로필]** 탭에는 데이터베이스에 추가된 가상 수신자인 모든 테스트 프로필이 나열됩니다. [테스트 프로필 작업 방법 알아보기](../audience/test-profiles.md)

   * **[!UICONTROL 프로필]** 탭에는 데이터베이스에 저장된 모든 프로필이 나열됩니다. [프로필 작업 방법 알아보기](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable="yes"}

1. 테스트 프로필 또는 프로필 목록을 검색할 때 필터를 사용하여 검색을 구체화할 수 있습니다. 예를 들어 **[!UICONTROL 잠재 고객]** 상태인 모든 테스트 프로필을 찾는 규칙을 정의할 수 있습니다. [쿼리 모델러를 사용하여 규칙을 추가하는 방법을 알아봅니다](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. 선택을 확인하려면 **[!UICONTROL 선택]**&#x200B;을 클릭하세요.

   게재 콘텐츠 미리 보기가 **[!UICONTROL 시뮬레이션]** 화면의 오른쪽 창에 표시됩니다. 개인화된 요소는 왼쪽 창에서 선택한 프로필의 데이터로 바뀝니다.

   ![](assets/simulate-preview.png){zoomable="yes"}

1. 여러 프로필을 추가한 경우 목록에서 전환하여 해당 게재 콘텐츠를 미리 볼 수 있습니다. 왼쪽 창의 해당 단추를 사용하여 테스트 프로필을 더 추가하고 선택을 취소할 수도 있습니다.

1. 전자 메일 게재의 경우 **[!UICONTROL 확대/축소 수준]**&#x200B;을 조정하고 오른쪽 상단의 전용 아이콘을 사용하여 데스크톱 또는 모바일 장치에서 콘텐츠를 미리 볼 수 있습니다.

1. **[!UICONTROL 시뮬레이션]** 화면에서 다음을 수행할 수도 있습니다.
   * 유효성 검사를 위해 특정 받는 사람에게 증명 보내기 - [자세히 알아보기](test-deliveries.md)
   * 보낸 증명 로그 액세스 - [자세히 알아보기](test-deliveries.md#access-test-deliveries)
   * 전자 메일 전용 인기 있는 전자 메일 클라이언트의 메시지 콘텐츠 렌더링을 확인하세요. - [자세히 알아보기](email-rendering.md)



