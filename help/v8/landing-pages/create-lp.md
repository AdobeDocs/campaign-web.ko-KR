---
title: 랜딩 페이지 만들기
description: Campaign 웹에서 랜딩 페이지를 구성하고 게시하는 방법을 알아봅니다
feature: Landing Pages
badge: label="제한 공개"
source-git-commit: 5c3f02d4c95951693ac73de4a6e8810e1b662e53
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 22%

---

# 랜딩 페이지 만들기 및 게시 {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="랜딩 페이지 만들기 및 관리"
>abstract="Adobe Campaign을 사용하면 기본 제공 템플릿을 기반으로 획득, 구독/구독 취소 및 차단 목록 사용 사례를 관리할 수 있는 온라인 웹 페이지로 사용자를 안내하기 위해 랜딩 페이지를 만들고 디자인하고 공유할 수 있습니다."

Adobe Campaign을 사용하면 랜딩 페이지를 만들고, 디자인하고, 공유할 수 있습니다. 마케팅 캠페인의 맥락에서 랜딩 페이지는 방문자가 이메일, SMS, 푸시 게재 또는 웹 사이트에서 링크를 클릭한 후 리디렉션되는 독립 실행형 웹 페이지입니다. Adobe Campaign에는 관리할 4개의 템플릿이 포함되어 있습니다 **acquisition**, **구독**, **구독 취소**, 및 **차단 목록** 활용 사례.

## 랜딩 페이지 액세스 {#access-landing-pages}

랜딩 페이지 목록에 액세스하려면 다음을 선택합니다. **[!UICONTROL 캠페인 관리]** > **[!UICONTROL 랜딩 페이지]** 왼쪽 메뉴에서

![](assets/lp-inventory.png)

다음 **[!UICONTROL 랜딩 페이지]** 인벤토리는 생성된 모든 품목을 표시합니다. 다음을 사용하여 필터링할 수 있습니다. **필터 표시** 단추를 클릭합니다. 결과를 특정 항목으로 제한할 수 있습니다 [폴더](../get-started/permissions.md#folders) 드롭다운 목록을 사용하거나 [쿼리 모델러](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Campaign 웹의 클라이언트 콘솔에서 만든 랜딩 페이지는 표시하거나 편집할 수 없습니다. 다음에서 자세히 알아보기 [Campaign 콘솔 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

랜딩 페이지를 복제하거나 삭제할 수 있습니다. 랜딩 페이지 옆에 있는 세 점을 클릭하여 원하는 작업을 선택합니다.

## 랜딩 페이지 만들기 {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="랜딩 페이지 속성 정의"
>abstract="레이블과 같은 속성 필드를 입력하고 필요한 경우 스키마를 수정합니다. 내부 이름을 편집하고, 랜딩 페이지가 저장되는 폴더를 변경하고, 설명을 제공할 수도 있습니다."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="페이지 콘텐츠 정의"
>abstract="이 랜딩 페이지의 일부인 각 페이지의 콘텐츠를 편집합니다."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="랜딩 페이지 일정 예약"
>abstract="랜딩 페이지의 시작 날짜와 종료 날짜를 정의할 수 있습니다. 페이지가 만료되면 **만료** 페이지가 표시됩니다."


>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="기본 페이지의 설정 정의"
>abstract="사용자가 이메일 또는 웹 사이트 등 랜딩 페이지 링크를 클릭하면 기본 페이지가 바로 표시됩니다."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="구독 랜딩 페이지 설정"
>abstract="고객은 구독 페이지를 통해 서비스를 구독할 수 있습니다."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. 다음에서 **[!UICONTROL 랜딩 페이지]** 인벤토리, 클릭 **[!UICONTROL 랜딩 페이지 만들기]**.

   ![](assets/lp-create-button.png)

1. 템플릿 선택:
   * **[!UICONTROL 고객 확보]**: 프로필 데이터를 캡처하고 업데이트할 수 있는 랜딩 페이지의 기본 템플릿입니다.
   * **[!UICONTROL 구독]**: 이 템플릿을 사용하여 서비스 구독을 제공합니다.
   * **[!UICONTROL 구독 취소]**: 이 템플릿은 구독자에게 전송된 이메일에서 서비스에 연결될 수 있으며 구독자가 이 서비스의 구독을 취소하도록 허용합니다.
   * **[!UICONTROL 차단 목록]**: 이 템플릿은 Campaign에서 더 이상 프로필에 연락하지 않으려는 경우에 사용해야 합니다. 차단 목록에 추가하다 관리에 대해 자세히 알아보기

   ![](assets/lp-templates.png)

1. 클릭 **[!UICONTROL 만들기]**.

1. 레이블과 같은 속성 필드를 채웁니다. 기본적으로 랜딩 페이지는 **[!UICONTROL 웹 애플리케이션]** 폴더를 삭제합니다. 에서 원하는 위치로 이동하여 변경할 수 있습니다. **[!UICONTROL 추가 옵션]**. [폴더 작업 방법 알아보기](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. 다음에서 **[!UICONTROL 데이터 미리 로드]** 섹션에는 기본적으로 아래 두 가지 옵션이 선택되어 있습니다.

   * 다음 **[!UICONTROL 양식에 참조된 데이터로 미리 채우기]** 옵션을 사용하면 양식의 입력 및 병합 필드와 일치하는 데이터를 자동으로 미리 로드할 수 있습니다.

   * 다음 **[!UICONTROL ID가 없는 경우 미리 로드 건너뛰기]** 프로필을 업데이트하지 않으려면 옵션을 선택해야 합니다. 이 경우 입력한 각 프로필은 양식 승인 후 데이터베이스에 추가됩니다. 이 옵션은 양식이 웹 사이트에 게시되는 경우 등에 사용됩니다.

1. 다음에서 **[!UICONTROL 페이지]** 섹션에서 **[!UICONTROL 콘텐츠 편집]** 이 랜딩 페이지에 디자인할 각 페이지의 단추입니다. 각 페이지의 콘텐츠는 이미 사전에 채워져 있습니다. 필요에 따라 편집합니다. [자세히 알아보기](lp-content.md)

   ![](assets/lp-pages.png)

1. 다음 **[!UICONTROL 미리 로드된 레코드 업데이트]** 기본적으로 옵션이 선택되어 있습니다. 랜딩 페이지를 통해 데이터베이스에 저장된 프로필을 업데이트하려면 미리 로드 상자를 사용할 수 있습니다. 미리 로드 상자를 사용하여 데이터베이스에서 업데이트할 레코드를 찾는 방법을 표시할 수 있습니다. 랜딩 페이지의 현재 컨텍스트에 있는 필드 중에서 데이터베이스에서 해당 프로필을 찾는 데 사용할 필드를 선택할 수도 있습니다.

   ![](assets/lp-storage-schedule.png)

1. 랜딩 페이지의 시작 날짜와 종료 날짜를 정의할 수 있습니다. 선택 **[!UICONTROL 예약 활성화]** 날짜를 설정합니다. 페이지가 만료되면 **[!UICONTROL 만료]** 페이지가 표시됩니다.

1. 클릭 **[!UICONTROL 검토 및 게시]**.

모든 페이지를 구성하고 디자인한 후에는 다음 작업을 수행할 수 있습니다 [테스트](#test-landing-page) 및 [게시](#publish-landing-page) 랜딩 페이지입니다.

## 랜딩 페이지 테스트 {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="랜딩 페이지 시뮬레이션"
>abstract="Campaign Web 사용자 인터페이스에서 랜딩 페이지의 미리보기를 보거나 새 웹 브라우저 탭에서 열 수 있습니다."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="랜딩 페이지 미리보기 및 테스트"
>abstract="랜딩 페이지 설정 및 콘텐츠가 정의되면 테스트 프로필을 사용하여 미리보기할 수 있습니다."

랜딩 페이지 설정 및 콘텐츠를 정의하고 나면 테스트 프로필을 사용하여 미리 볼 수 있습니다. 를 삽입한 경우 [개인화된 콘텐츠](../personalization/gs-personalization.md), 테스트 프로필 데이터를 사용하여 이 콘텐츠가 랜딩 페이지에 표시되는 방식을 확인할 수 있습니다.

>[!CAUTION]
>
>메시지를 미리 보고 증명을 보내려면 테스트 프로필을 사용할 수 있어야 합니다. 방법 알아보기 [테스트 프로필 만들기](../audience/test-profiles.md).

1. 랜딩 페이지 인터페이스에서 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하여 테스트 프로필 선택에 액세스합니다.

   ![](assets/lp-simulate-content.png)

1. 다음에서 **[!UICONTROL 시뮬레이트]** 화면에서 하나 이상의 테스트 프로필을 선택합니다.

   테스트 프로필을 선택하는 단계는 메시지를 테스트할 때와 동일합니다. 자세한 내용은 [미리 보기 및 테스트](../preview-test/preview-test.md) 섹션.

1. 선택 **[!UICONTROL 미리보기 열기]** 랜딩 페이지를 테스트합니다.

   ![](assets/lp-open-preview.png)

1. 랜딩 페이지의 미리보기가 새 탭에서 열립니다. 개인화된 요소는 선택한 테스트 프로필 데이터로 대체됩니다.

   ![](assets/lp-preview.png)

1. 다른 테스트 프로필을 선택하여 랜딩 페이지의 각 변형에 대한 렌더링을 미리 봅니다.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## 랜딩 페이지 게시 {#publish-landing-page}

랜딩 페이지가 준비되면 이를 게시하여 메시지에 사용할 수 있도록 할 수 있습니다.

랜딩 페이지가 게시되면 다음과 함께 랜딩 페이지 목록에 추가됩니다. **[!UICONTROL 게시됨]** 상태. 이제 라이브이며 사용할 준비가 되었습니다.

![](assets/lp-published.png)

게시되면 다음을 복사하여 붙여 넣을 수 있습니다. **[!UICONTROL 랜딩 페이지 URL]** 웹 브라우저에 페이지 맨 위에 표시됩니다.

로그 및 특정 보고서를 통해 랜딩 페이지의 영향을 모니터링할 수 있습니다.