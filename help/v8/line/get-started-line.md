---
audience: end-user
title: LINE 메시지 시작
description: Adobe Campaign 웹 사용자 인터페이스를 사용하여 LINE 메시지를 만들고 보내는 방법 알아보기
feature: Line App
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: d9d413df-4e9e-4906-bbbc-28c06c2ccf59
    internal-label: LINE App
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 12%
---
# LINE 메시지 시작 {#get-started-line}

LINE은 모든 모바일 디바이스와 PC에서 사용할 수 있는 무료 인스턴트 메시지, 음성 및 영상 통화용 애플리케이션입니다. Adobe Campaign을 사용하여 LINE 메시지를 보낼 수 있습니다. 독립 실행형 게재 또는 워크플로우에서 다른 채널과 함께 LINE을 사용합니다.

![모바일 장치에서 받은 LINE 메시지의 예](assets/line-message.png)

* **[!UICONTROL 게재]**: SMS 또는 푸시와 유사한 왼쪽 레일의 **[!UICONTROL 게재]** 메뉴에서 독립 실행형 LINE 게재를 만듭니다. [자세히 알아보기](send-line.md).

* **[!UICONTROL 워크플로]**: 워크플로 캔버스에서 **[!UICONTROL LINE]** 채널 활동을 추가하고 게재 템플릿을 선택한 다음 게재 대시보드에서 콘텐츠 및 설정을 정의합니다. [이 섹션](../workflows/activities/channels.md)에서 채널 활동에 대해 자세히 알아보세요.

  >[!NOTE]
  >
  >**[!UICONTROL LINE]** 채널 활동에 피드를 제공하는 **[!UICONTROL 대상자 빌드]** 활동에서 타깃팅 차원을 **[!UICONTROL 방문자 구독]**(으)로 변경하십시오. 사이드 패널에서 **[!UICONTROL 모든 스키마 표시]**&#x200B;를 사용하도록 설정해야 합니다. 이 타겟팅 차원이 설정되면 게재 템플릿 선택기를 사용할 수 있습니다.
