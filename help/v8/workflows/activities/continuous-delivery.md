---
audience: end-user
title: 연속 게재 워크플로우 활동 사용
description: 연속 게재 워크플로우 활동을 사용하는 방법을 알아봅니다
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 3%

---

# 지속적인 게재 {#continuous-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="지속적인 게재 활동"
>abstract="이제 기존 게재에 새 수신자를 추가할 수 있습니다. 이 게재 유형은 매번 새 게재를 만들 필요가 없으므로 필요에 따라 전송되는 낮은 볼륨 경고 또는 알림에 대해 보다 효율적입니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ko" text="릴리스 정보 참조"

**연속 게재** 활동을 사용하면 기존 게재에 새 수신자를 추가할 수 있습니다. 이 게재 유형은 매번 새 게재를 만들 필요가 없으므로 필요에 따라 전송되는 낮은 볼륨 경고 또는 알림에 대해 보다 효율적입니다.

연속 게재는 단일 게재 인스턴스를 만듭니다. 모든 게재 로그(broadLog) 및 추적 로그는 이 하나의 게재를 참조하므로 모니터링 및 보고를 단순화합니다.

## 연속 게재 활동 구성 {#configure}

1. **연속 게재** 활동을 워크플로우 캔버스에 추가합니다.

   연속 게재 활동을 보여 주는 ![스크린샷](../assets/continuous-delivery.png){zoomable="yes"}

1. 활동에 대한 사용자 지정 **[!UICONTROL 레이블]**&#x200B;을(를) 입력하십시오(선택 사항). 기본적으로 &quot;연속 게재&quot;라는 레이블이 지정됩니다.

1. **[!UICONTROL 템플릿]** 필드 옆에 있는 검색 아이콘을 클릭하여 게재 템플릿을 선택합니다. 템플릿(표준 게재 아님)만 선택할 수 있습니다. 템플릿은 게재 채널, 콘텐츠 및 구성을 정의합니다.

1. **[!UICONTROL 타깃팅 옵션]**&#x200B;에서 대상 모집단을 정의하는 방법을 선택하십시오.

   * **[!UICONTROL 인바운드 이벤트에 의해 지정됨]**: 대상은 인바운드 전환(빌드 대상 또는 증분 쿼리와 같은 업스트림 활동)에서 가져옵니다. 가장 일반적인 옵션입니다.

   * **[!UICONTROL 게재 템플릿에 지정됨]**: 대상이 템플릿 자체에 정의되어 있습니다.

   * **[!UICONTROL 입력 이벤트에 지정된 파일]**: 워크플로우를 통해 전달된 파일을 통해 대상이 제공됩니다.

연속 게재 활동은 자동으로 아웃바운드 전환을 생성하여 워크플로우를 계속합니다.

## 관련 항목 {#related}

* [워크플로 활동 정보](about-activities.md)
* [이메일, SMS, 푸시, DM 활동](channels.md)
* [게재 템플릿](../../msg/delivery-template.md)
