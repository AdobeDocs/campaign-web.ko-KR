---
audience: end-user
title: 플랜 및 프로그램
description: Adobe Campaign에서 계획 및 프로그램을 만들고 구성하는 방법에 대해 알아봅니다
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 10%

---

# 플랜 및 프로그램 {#plan-and-programs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="플랜 및 프로그램"
>abstract="이제 Campaign Web 사용자 인터페이스에서 마케팅 플랜 및 프로그램에 대한 폴더 계층 구조를 구성할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ko-KR" text="릴리스 정보 참조"

Adobe Campaign을 사용하면 마케팅 플랜 및 프로그램에 대한 폴더 계층 구조를 구성할 수 있습니다.

Adobe 이를 보다 효율적으로 구성하려면 다음 계층을 권장합니다. `>` 프로그램 `>` 캠페인 계획

* **계획**&#x200B;에는 여러 프로그램이 포함될 수 있습니다. 일정 기간 동안의 전략적 목표를 정의합니다.
* **프로그램**&#x200B;에는 캠페인, 워크플로우 및 랜딩 페이지뿐만 아니라 다른 프로그램도 포함될 수 있습니다.
* **campaign**&#x200B;에는 게재, 워크플로우 및 랜딩 페이지가 포함될 수 있습니다.

## 플랜 만들기 및 구성 {#create-plan}

플랜을 만들려면 폴더 유형이 **[!UICONTROL 플랜]**&#x200B;인 폴더를 만들어야 합니다. [폴더 만들기에 대해 자세히 알아보기](../get-started/work-with-folders.md).

![](assets/plan_create.png){zoomable="yes"}

플랜의 **[!UICONTROL 폴더 설정]**(으)로 이동하여 관리하십시오.

![](assets/plan_settings.png){zoomable="yes"}

**[!UICONTROL 사용자 지정 옵션]**&#x200B;을(를) 정의하고 플랜 예약 날짜를 설정할 수 있습니다.

![](assets/plan_options.png){zoomable="yes"}

**[!UICONTROL 사용자 지정 옵션]**&#x200B;을 관리하려면:

1. **[!UICONTROL 스키마]** 찾아보기
1. 필터에서 **[!UICONTROL 편집 가능]** 스키마 선택
1. **[!UICONTROL 사용자 지정 세부 정보 편집]**&#x200B;의 아이콘을 클릭합니다.

![](assets/plan_edit.png){zoomable="yes"}

다음을 구성할 수 있습니다.

![](assets/plan_customfields.png){zoomable="yes"}

## 프로그램 만들기 및 구성

플랜에 프로그램을 만들려면([플랜 만들기에 대해 자세히 알아보기](#create-plan)) 플랜에 있는 폴더 유형 **[!UICONTROL 프로그램]**&#x200B;을(를) 사용하여 폴더를 만들어야 합니다. [폴더 만들기에 대해 자세히 알아보기](../get-started/work-with-folders.md).

![](assets/program_create.png){zoomable="yes"}

관리하려면 프로그램의 **[!UICONTROL 폴더 설정]**(으)로 이동하십시오.

![](assets/program_settings.png){zoomable="yes"}

**[!UICONTROL 사용자 지정 옵션]**&#x200B;을 정의하고 프로그램의 예약 날짜를 설정할 수 있습니다.

![](assets/program_options.png){zoomable="yes"}

**[!UICONTROL 사용자 지정 옵션]**&#x200B;을 관리하려면:

1. **[!UICONTROL 스키마]** 찾아보기
1. 필터에서 **[!UICONTROL 편집 가능]** 스키마 선택
1. **[!UICONTROL 사용자 지정 세부 정보 편집]**&#x200B;의 아이콘을 클릭합니다.

![](assets/program_edit.png){zoomable="yes"}

이를 구성할 수 있습니다.

![](assets/program_customfields.png){zoomable="yes"}

## 캠페인을 프로그램에 연결하는 방법

두 가지 방법으로 캠페인을 프로그램에 연결할 수 있습니다.

### 방법 #1 : 이미 프로그램이 있고 여기에 연결된 캠페인을 만들려고 합니다

새 캠페인을 프로그램에 연결하려면 프로그램에서 직접 캠페인을 만듭니다.

![](assets/program_campaign_create.png){zoomable="yes"}

**[!UICONTROL 폴더]** 설정은 프로그램의 경로로 자동 정리됩니다.

![](assets/program_campaign_folder.png){zoomable="yes"}

### 방법 #2 : 이미 기존 캠페인이 있으며 이를 기존 프로그램에 연결하려고 합니다

프로그램에 연결할 캠페인의 **[!UICONTROL 설정]** 단추로 이동합니다.

![](assets/campaign_settings.png){zoomable="yes"}

**[!UICONTROL 속성]**&#x200B;에서 **[!UICONTROL 폴더]** 설정의 **[!UICONTROL 폴더]** 아이콘을 클릭하여 **[!UICONTROL 프로그램]** 폴더를 선택하세요.

![](assets/campaign_folder.png){zoomable="yes"}

**[!UICONTROL 프로그램]** 폴더를 선택하고 **[!UICONTROL 확인]** 단추를 클릭한 다음 **[!UICONTROL 저장 및 닫기]** 단추를 클릭합니다.

![](assets/campaign_linked.png){zoomable="yes"}

이제 캠페인이 프로그램에 나열됩니다.

![](assets/campaign_in_program.png){zoomable="yes"}
