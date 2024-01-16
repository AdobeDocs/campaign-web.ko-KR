---
title: 프로필 모니터링 및 관리
description: Campaign 웹에서 프로필을 모니터링하고 관리하는 방법을 알아봅니다.
badge: label="제한 공개"
source-git-commit: 9c72d73b5279a01492ea3ccd295e513e91f0c050
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 44%

---

# 프로필 모니터링 및 관리 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="프로필 자세히 살펴보기"
>abstract="새로운 프로필을 만들고, 강력한 보고서와 도구를 통해 모니터링합니다. 프로필 속성, 상호 작용 및 로그에 액세스합니다. 필터링 옵션을 사용하여 프로필 목록을 찾아보고 프로필을 편집 및 업데이트합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="릴리스 정보 참조"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="프로필 자세히 살펴보기"
>abstract="새로운 프로필을 만들고, 강력한 보고서와 도구를 통해 모니터링합니다. 프로필 속성, 상호 작용 및 로그에 액세스합니다. 필터링 옵션을 사용하여 프로필 목록을 찾아보고 프로필을 편집 및 업데이트합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="릴리스 정보 참조"

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="프로필"
>abstract="프로필은 Adobe Campaign에서 보낸 메시지를 수신하도록 대상으로 지정된 개인입니다. 권한에 따라 이 목록에서 프로필의 세부 정보를 볼 수 있습니다. 필터링 옵션을 사용하여 이 목록을 찾아볼 수 있습니다. 일부 프로필 속성을 편집하고 업데이트할 수 있습니다."

## 프로필 시작 {#gs}

Adobe Campaign 웹의 프로필은 데이터베이스에 저장된 개인으로서 의 주요 구성 요소 역할을 합니다 [대상자 만들기](create-audience.md) 게재 및 [개인화 추가](../personalization/personalize.md) 데이터를 콘텐츠에 추가합니다.

다음과 같은 다른 유형의 프로필이 데이터베이스에 저장됩니다. **[!UICONTROL 테스트 프로필]**: 최종 대상자에게 전송되기 전에 게재를 테스트하도록 설계되었습니다. [자세히 알아보기](test-profiles.md)

Adobe Campaign 클라이언트 콘솔에서만 프로필을 만들 수 있습니다. - [방법 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/create-profiles.html){target="_blank"}. 하지만 Adobe Campaign 웹에서 액세스하고 편집할 수 있습니다. **[!UICONTROL 고객 관리]** > **프로필** 왼쪽 탐색 레일의 항목.

>[!NOTE]
>
>사용 권한에 따라 데이터베이스에 저장된 프로필의 전체 목록에 액세스하지 못할 수도 있습니다. [권한에 대해 자세히 알아보기](../get-started/permissions.md).

* 다음을 필터링할 수 있습니다. **[!UICONTROL 프로필]** 다음에서 사용할 수 있는 검색 필드 또는 필터를 사용하여 나열: **필터 표시** 단추를 클릭합니다. 결과를 특정 항목으로 제한할 수 있습니다 [폴더](../get-started/permissions.md#folders) 드롭다운 목록을 사용하거나 [쿼리 모델러](../query/query-modeler-overview.md).

  ![](assets/profiles-list-filters.png)

* 프로파일을 삭제하려면 다음 목록에서 해당 옵션을 선택합니다 **[!UICONTROL 추가 작업]** 메뉴 아래의 제품에서 사용할 수 있습니다.

* 프로필을 편집하려면 목록에서 원하는 항목을 클릭합니다. [자세히 알아보기](#access)

다음을 통해 프로필에 액세스할 수도 있습니다. **[!UICONTROL 탐색기]** 보기, 에서 **[!UICONTROL 프로필 및 타겟]** > **[!UICONTROL 수신자]** 노드.

여기에서 폴더 또는 하위 폴더를 탐색, 생성 및 관리하고 관련 권한을 확인할 수 있습니다. [폴더 만들기 방법 알아보기](../get-started/permissions.md#folders)

![](assets/profiles-explorer-folder.png)

다음에서 **[!UICONTROL 탐색기]** 보기 필터, 삭제 및 [편집](#access) 프로필.

## 프로필 속성 액세스 및 편집 {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="기본 세부 정보"
>abstract="이 섹션에서는 프로필의 기본 세부 정보에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="연락처 정보"
>abstract="이 섹션에서는 프로필의 연락처 정보에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="주소"
>abstract="이 섹션에서는 프로필의 우편 주소와 주소 품질에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="계정 세부 정보"
>abstract="이 섹션에서는 프로필의 계정 세부 정보에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="수신자 더 이상 연락하지 않음"
>abstract="이 섹션에서는 프로필의 연락처 환경 설정에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="사용자 정의 필드"
>abstract="사용자 정의 필드는 필요에 맞춰 인스턴스에 대해 구성된 특정 속성입니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="기타"
>abstract="이 섹션에서는 기본 제공되는 추가 속성을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="수신자 구독 목록"
>abstract="이 탭에는 프로필에서 구독하는 모든 서비스가 나열됩니다."

프로필의 세부 정보에 액세스하여 편집하려면 아래 단계를 따르십시오.

1. 다음으로 이동 **[!UICONTROL 고객 관리]** > **[!UICONTROL 프로필]** 및 를 클릭하고 **[!UICONTROL 프로필]** 목록을 표시합니다.

   ![](assets/profiles-list-select.png)

1. 프로필에 대한 자세한 정보가 표시됩니다.

   다음 **[!UICONTROL 세부 사항]** 탭에서는 프로필의 기본 제공 및 사용자 지정 특성을 찾아볼 수 있습니다. 속성을 편집하려면 원하는 필드를 변경하고 **[!UICONTROL 저장]** 단추를 클릭합니다.

   ![](assets/profile-details.png)

   1. 기본적으로 프로필은 **[!UICONTROL 수신자]** 폴더를 삭제합니다. 원하는 위치로 이동하여 변경할 수 있습니다. [폴더 작업 방법 알아보기](../get-started/permissions.md#folders)

      ![](assets/profile-folder.png)

   1. 다음에서 **[!UICONTROL 연락처 정보]** 섹션에서 이메일 주소 및 기타 관련 데이터를 업데이트할 수 있습니다. 프로필 레이블 뒤에 대괄호 사이에 이메일 주소가 표시됩니다.

      ![](assets/profile-address.png)

   1. 다음 확인: **[!UICONTROL 더 이상 연락하지 않음]** 옵션을 선택하고 필요한 경우 업데이트합니다. 이러한 옵션 중 하나를 선택하면 프로파일이 [차단 목록]에 표시됩니다. 예를 들어 수신자가 뉴스레터에서 구독 취소 링크를 클릭한 경우 이 정보가 연락처 데이터에 추가됩니다. 해당 수신자는 더 이상 선택한 채널을 타겟팅하지 않습니다. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

      ![](assets/profile-no-longer-contact.png)

   1. 있는 경우 **[!UICONTROL 사용자 정의 필드]**, 필요에 따라 값을 업데이트할 수 있습니다. 사용자 지정 필드는 다음에 추가된 추가 속성입니다. **[!UICONTROL 프로필]** Adobe Campaign 콘솔을 통한 스키마. [자세히 알아보기](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

      ![](assets/profile-custom-fields.png)

1. 다음을 클릭합니다. **[!UICONTROL 구독]** 탭으로 이동하여 프로필이 구독되는 서비스에 대한 정보에 액세스합니다. [구독 서비스에 대해 자세히 알아보기](manage-services.md)

   ![](assets/profile-subscriptions.png)

1. 다음을 클릭합니다. **[!UICONTROL 로그]** 전송, 제외 및 추적 로그를 통해 프로필의 상호 작용 기록을 볼 수 있는 화면 오른쪽 상단에 있는 버튼입니다. [게재 로그에 대해 자세히 알아보기](../monitor/delivery-logs.md)

   프로필에 제공된 오퍼를 검토할 수도 있습니다. **[!UICONTROL 제안]** 탭. [오퍼에 대해 자세히 알아보기](../msg/offers.md)

   ![](assets/profile-logs.png)
