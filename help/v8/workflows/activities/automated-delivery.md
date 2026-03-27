---
audience: end-user
title: 자동화된 게재 워크플로우 활동
description: 자동화된 게재 워크플로우 활동을 사용하는 방법을 알아봅니다
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 3%

---

# 자동화된 게재 {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="자동화된 게재 활동"
>abstract="이제 워크플로우 팔레트에서 자동화된 게재 워크플로우 활동을 사용할 수 있습니다. 이를 사용하여 워크플로우 내에서 직접 게재 작업(준비, 증명 보내기, 준비 및 시작 등)을 만들거나 실행할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="릴리스 정보 참조"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="자동화된 게재 활동"
>abstract="**자동화된 게재** 활동은 자동화에 사용됩니다. 워크플로우에서 게재를 만들거나 다시 사용한 다음 수행할 작업(준비, 준비 및 시작, 증명 보내기 등)을 선택하십시오. 워크플로우 외부에서 만든 기존의 명시적 게재를 선택하거나 활동이 실행될 때마다 템플릿에서 새 게재를 만들 수 있습니다."

**자동화된 게재** 활동을 사용하면 워크플로우 내에서 직접 게재 작업을 만들고, 구성하고, 실행할 수 있습니다. 일정에 따라 또는 자동화된 흐름의 일부로 사전 정의된 게재를 실행하려는 경우 또는 활동이 실행될 때마다 템플릿에서 새 게재를 생성하려는 경우 사용합니다.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. -->

이 활동을 구성하려면 다음 단계를 수행합니다.

1. 게재 설정을 정의합니다. [자세히 보기](#delivery-settings)
1. 수행할 작업을 선택하십시오. [자세히 보기](#action-to-execute)
1. 전환 설정, [자세히 보기](#transition-to-execute)
1. 수정 스크립트를 정의합니다. [자세히 보기](#script)

## 게재 설정 정의 {#delivery-settings}

활동을 구성할 때 게재의 출처를 선택합니다. 이 섹션에서는 다음 두 가지 옵션을 사용할 수 있습니다.

![자동화된 게재를 보여 주는 스크린샷](../assets/automated-delivery.png){zoomable="yes"}

* 독립 실행형 게재 또는 캠페인에서 생성된 게재와 같은 기존 게재에 대해 작업하려면 **명시적 게재**&#x200B;을(를) 선택합니다. **배달 선택** 단추를 사용하여 배달을 선택하세요. 워크플로우가 실행되고 이 활동에 도달할 때마다 **동일한** 게재에 작동합니다. 실행당 새 게재가 만들어지지 않습니다. 활동은 동일한 게재를 재사용합니다. 이 기능은 예를 들어 일정에 따라 또는 승인 단계 후에 준비하거나 반복해서 전송하려는 단일 게재가 있을 때 유용합니다.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* 활동이 실행될 때마다 **새로 만들기** 게재를 만들려면 **새로 만들기, 템플릿에서 만들기**&#x200B;를 선택하십시오. **템플릿 선택** 단추를 사용하여 게재 템플릿을 선택하십시오. 각 실행은 해당 템플릿을 기반으로 새 게재를 생성합니다. 각 워크플로우 실행으로 인해 고유의 게재가 생성되어야 하는 경우(예: 실행당 하나의 이메일) 사용합니다.

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>고급 사용 사례에 사용되는 **전환에 지정됨** 및 **스크립트로 계산됨** 옵션은 클라이언트 콘솔에서만 구성할 수 있습니다. [Campaign v8 설명서](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}를 참조하세요.

## 수행할 작업 선택 {#action-to-execute}

이 섹션에서 활동이 게재와 함께 수행하는 작업을 선택합니다. 다음 옵션을 사용할 수 있습니다.

![자동화된 게재에서 실행할 작업을 보여 주는 스크린샷](../assets/automated-delivery2.png){zoomable="yes"}

* **저장**: 게재를 분석하거나 보내지 않고 게재를 만들고 저장합니다.
* **대상 예상**: 게재 대상을 계산하여 잠재적(첫 번째 분석 단계)을 평가합니다.
* **준비**: 전체 분석(대상 계산 및 콘텐츠 준비)을 실행합니다. 게재가 전송되지 않습니다.
* **증명 보내기**: 게재 증명을 보냅니다.
* **준비 및 시작**: 전체 분석(대상 계산 및 콘텐츠 준비)을 실행하고 게재를 보냅니다.

## 전환 설정 {#transition-to-execute}

이 섹션에서는 활동 후에 전환을 생성할지 여부를 선택할 수 있습니다. 다음 옵션을 사용할 수 있습니다.

![자동 게재에서 전환을 보여 주는 스크린샷](../assets/automated-delivery3.png){zoomable="yes"}

* **아웃바운드 전환을 생성합니다**: 활동이 완료되면 아웃바운드 전환을 생성합니다.
* **전환 레이블**: 캔버스에서 전환에 표시되는 레이블을 사용자 지정할 수 있습니다.
* **프로세스 오류**: 오류 처리를 위한 추가 전환을 추가합니다.

## 수정 스크립트 정의 {#script}

스크립트를 사용하여 활동의 동작(예: 활동 레이블과 같은 게재 매개 변수)을 변경할 수 있습니다. 이 활동에 대한 사용자 지정 논리가 필요한 경우 사용하십시오.

**스크립트 만들기**&#x200B;를 클릭하고 편집기에서 수정 논리를 작성하십시오.

## 관련 항목 {#related}

* [워크플로 활동 정보](about-activities.md)
* [지속적인 게재](continuous-delivery.md)
* [이메일, SMS, 푸시, DM 활동](channels.md)
* [게재 템플릿](../../msg/delivery-template.md)
