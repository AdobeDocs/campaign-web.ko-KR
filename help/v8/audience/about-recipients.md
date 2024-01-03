---
title: 프로필 모니터링 및 관리
description: Campaign 웹에서 프로필을 모니터링하고 관리하는 방법을 알아봅니다.
badge: label="제한 공개"
source-git-commit: e61878f325575377865186fb9cb63b831ac843fd
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 8%

---

# 프로필 모니터링 및 관리 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="프로필 360 보기"
>abstract="새 프로필을 만들고 강력한 보고서와 도구를 통해 프로필을 모니터링합니다. 프로필의 속성, 상호 작용 및 로그에 액세스합니다. 필터링 옵션을 사용하여 프로필 목록을 탐색하고 프로필을 편집 및 업데이트합니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="릴리스 정보 참조"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="프로필"
>abstract="프로필은 Adobe Campaign에서 보낸 메시지를 수신하도록 대상으로 지정된 개인입니다. 사용 권한에 따라 이 목록에서 프로필의 세부 사항을 볼 수 있습니다. 필터링 옵션을 사용하여 이 목록을 찾아볼 수 있습니다. 프로필의 작은 속성 세트를 편집하고 업데이트할 수 있습니다."

## 프로필 시작 {#gs}

Adobe Campaign 웹의 프로필은 데이터베이스에 저장된 개인으로서 게재 대상을 만들고 콘텐츠에 개인화 데이터를 추가하는 주요 구성 요소 역할을 합니다. 최종 대상자에게 전송되기 전에 게재를 테스트하도록 설계된 테스트 프로필과 같은 다양한 유형의 프로필이 데이터베이스에 저장됩니다. [테스트 프로필 작업 방법 알아보기](test-profiles.md)

Campaign 클라이언트 콘솔에서만 프로필을 추가할 수 있습니다. 하지만 Adobe Campaign 웹에서는 **프로필** 왼쪽 탐색 레일의 항목. 다음에서 액세스할 수도 있습니다 **탐색기** 보기 - 폴더, 하위 폴더를 찾아보고 만들며 관련 사용 권한을 확인할 수 있습니다.

검색 필드를 사용하여 프로필 목록을 필터링하거나 **필터 표시** 단추를 클릭합니다.

![](assets/profiles-list.png)

>[!NOTE]
>
>사용 권한에 따라 데이터베이스에 저장된 프로필의 전체 목록에 액세스하지 못할 수도 있습니다. [이 섹션](../get-started/permissions.md)에서 권한에 대해 자세히 알아보십시오.

## 프로필 속성 액세스 및 편집 {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="기본 세부 정보"
>abstract="이 섹션에서는 프로필의 기본 세부 정보에 대한 통찰력을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="연락처 정보"
>abstract="이 섹션에서는 프로필의 연락처 정보에 대한 통찰력을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title= "Address"
>abstract="이 섹션에서는 프로필의 우편 주소 및 주소 품질에 대한 통찰력을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="계정 세부 정보"
>abstract="이 섹션에서는 프로필의 계정 세부 정보에 대한 통찰력을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="수신자 더 이상 연락하지 않음"
>abstract="이 섹션에서는 프로필의 연락처 환경 설정에 대한 통찰력을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="사용자 정의 필드"
>abstract="사용자 지정 필드는 인스턴스에 대해 구성된 요구 사항에 맞게 조정된 특정 속성입니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="기타"
>abstract="이 섹션에서는 추가 기본 속성을 제공합니다. 정보를 수정하려면 해당 필드에서 직접 변경하고 **저장** 화면의 오른쪽 상단에 있는 단추입니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="수신자 구독 목록"
>abstract="이 탭에는 프로필이 구독하는 모든 서비스가 나열됩니다."

프로필 세부 정보에 액세스하려면 프로필 목록에서 해당 이름을 클릭합니다.

![](assets/profiles-details.png)

이 화면에서 프로필의 자세한 정보에 액세스할 수 있습니다.

* 다음 **[!UICONTROL 세부 사항]** 탭에서는 프로필의 기본 제공 및 사용자 지정 특성을 찾아볼 수 있습니다. 속성을 편집하려면 원하는 필드를 변경하고 **[!UICONTROL 저장]** 단추를 클릭합니다.
* 다음 **[!UICONTROL 구독]** 탭은 프로필이 구독되는 서비스에 대한 정보를 제공합니다. [구독 서비스 작업 방법 알아보기](manage-services.md)
* 다음 **[!UICONTROL 로그]** 화면 오른쪽 상단에 있는 버튼을 사용하면 전송, 제외 및 추적 로그를 통해 프로필의 상호 작용 내역뿐만 아니라 프로필에 제공된 제안을 볼 수 있습니다.
