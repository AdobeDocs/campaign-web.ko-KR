---
title: Campaign에서 테스트 프로필 만들기
description: Adobe Campaign에서 테스트 프로필을 만들고 관리하는 방법 알아보기
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 14%

---

# 테스트 프로필 만들기 및 관리 {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="테스트 프로필 만들기"
>abstract="테스트 프로필은 메시지를 보내기 전에 개인화 및 렌더링을 미리 보고 테스트할 수 있도록 해 주는 추가 수신자입니다. 메시지 내용을 미리 볼 때 테스트 프로필을 선택하고 테스트 프로필에 교정쇄를 보내 메시지 내용과 설정을 제어하고 검증할 수 있습니다."

테스트 프로필은 증명을 보내고 메시지 콘텐츠와 설정을 확인하는 데 사용됩니다. 이러한 프로필은 메시지를 보내기 전에 개인화 및 렌더링을 미리 보고 테스트할 수 있는 추가 수신자입니다. 메시지 콘텐츠를 미리 볼 때 테스트 프로필을 선택하고 테스트 프로필에 증명을 전송하여 메시지 콘텐츠와 설정을 제어하고 확인할 수 있습니다.

➡️ [비디오에서 이 기능 살펴보기](#video)

<!--Learn more about test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

테스트 프로필에 증명을 보내는 단계는 [이 섹션](../preview-test/test-deliveries.md#test-profiles)에 자세히 설명되어 있습니다.

>[!NOTE]
>
>* 테스트 프로필은 클라이언트 콘솔에서 시드 주소로 만들어집니다.
>
>* 다음 게재 통계에 대한 보고서에서 테스트 프로필이 자동으로 제외됩니다. **[!UICONTROL 클릭 수]**, **[!UICONTROL 열기 수]**, **[!UICONTROL 구독 취소 수]**.

## 테스트 프로필 액세스 및 관리 {#access-test-profiles}

테스트 프로필 목록에 액세스하려면 왼쪽 메뉴에서 **[!UICONTROL 고객 관리]** > **[!UICONTROL 프로필]**&#x200B;을 선택하고 **[!UICONTROL 테스트 프로필]** 탭을 클릭하십시오.

![테스트 프로필 목록 보기](assets/test-profile-list.png){zoomable="yes"}

* 드롭다운 목록을 사용하여 특정 [폴더](../get-started/permissions.md#folders)를 필터링하거나 [쿼리 모델러](../query/query-modeler-overview.md)를 사용하여 규칙을 추가할 수 있습니다.

  ![테스트 프로필 목록 필터](assets/test-profile-list-filters.png){zoomable="yes"}

* 테스트 프로필을 복제하고 필요에 따라 업데이트할 수 있습니다. 테스트 프로필을 편집하는 단계는 [테스트 프로필을 만드는 단계](#create-test-profile)와 동일합니다.

* 테스트 프로필을 삭제하려면 **[!UICONTROL 추가 작업]** 메뉴에서 해당 옵션을 선택하십시오.

  ![테스트 프로필 옵션 삭제](assets/test-profile-list-delete.png){zoomable="yes"}

* 테스트 프로필을 편집하려면 목록에서 원하는 항목을 클릭합니다. 테스트 프로필을 편집하는 단계는 [테스트 프로필을 만드는 단계](#create-test-profile)와 동일합니다.

**[!UICONTROL 리소스]** > **[!UICONTROL 캠페인 관리]** > **[!UICONTROL 시드 주소]** 노드에서 **[!UICONTROL 탐색기]** 보기를 통해 테스트 프로필에 액세스할 수도 있습니다.

여기에서 폴더 또는 하위 폴더를 탐색, 생성 및 관리하고 관련 권한을 확인할 수 있습니다. [폴더를 만드는 방법 알아보기](../get-started/permissions.md#folders)

![테스트 프로필 폴더 보기](assets/test-profiles-folders.png){zoomable="yes"}

**[!UICONTROL 탐색기]** 보기에서 테스트 프로필을 필터링, 삭제, 편집 및 [만들기](#create-test-profile)할 수도 있습니다.

## 테스트 프로필 만들기 {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="테스트 프로필 추가 데이터"
>abstract="데이터 관리 워크플로에서 생성되고 특정 값을 할당하려는 게재에 사용되는 개인화 데이터를 입력합니다."

테스트 프로필을 만들려면 아래 단계를 수행합니다.

1. **[!UICONTROL 고객 관리]** > **[!UICONTROL 프로필]**(으)로 이동한 다음 **[!UICONTROL 테스트 프로필]** 탭을 선택합니다.

1. **[!UICONTROL 테스트 프로필 만들기]** 단추를 클릭합니다.

   ![테스트 프로필 만들기 단추](assets/test-profile-create.png){zoomable="yes"}

1. 필요에 따라 테스트 프로필 세부 사항을 입력합니다. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![테스트 프로필 세부 정보 양식](assets/test-profile-details.png){zoomable="yes"}

   >[!NOTE]
   >
   >**[!UICONTROL 레이블]** 필드는 사용자가 정의한 이름과 성으로 자동으로 채워집니다.

1. 기본적으로 테스트 프로필은 **[!UICONTROL 시드 주소]** 폴더에 저장됩니다. 원하는 위치로 이동하여 변경할 수 있습니다. [폴더 작업 방법 알아보기](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. **[!UICONTROL 연락처 정보]** 섹션에서 전자 메일 주소 및 기타 관련 데이터를 입력합니다. 이메일 주소는 테스트 프로필 레이블 뒤에 대괄호 사이에 표시됩니다.

   ![연락처 정보 섹션](assets/test-profile-address.png){zoomable="yes"}

1. **[!UICONTROL 더 이상 연락하지 않음]** 확인란을 선택하면 테스트 프로필이 차단 목록에 추가하다에 표시됩니다. 이러한 수신자는 더 이상 채널(이메일, SMS 등)을 타겟팅하지 않습니다.

1. **[!UICONTROL 추가 데이터]** 탭에서 데이터 관리 워크플로우에서 만든 게재에 사용되는 개인화 데이터를 입력하고 특정 값을 할당할 데이터를 입력합니다. [워크플로에 대해 자세히 알아보기](../workflows/gs-workflows.md)

   ![추가 데이터 탭](assets/test-profile-additional-data.png){zoomable="yes"}

   추가 대상 데이터가 **[!UICONTROL 데이터 보강]** 워크플로우 활동에서 &#39;@&#39;으로 시작하는 별칭으로 정의되었는지 확인하십시오. 그렇지 않으면 게재 활동의 시드 주소와 함께 이 필드를 제대로 사용할 수 없습니다. [데이터 보강 활동에 대해 자세히 알아보기](../workflows/activities/enrichment.md)

1. **[!UICONTROL 저장]** 단추를 클릭합니다.

방금 만든 테스트 프로필을 이제 증명 전송에 사용할 준비가 되었습니다. [자세히 알아보기](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## 사용 방법 비디오 {#video}

Campaign 웹 사용자 인터페이스를 사용하여 테스트 프로필을 만들고 관리하는 방법을 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3442844?quality=12)