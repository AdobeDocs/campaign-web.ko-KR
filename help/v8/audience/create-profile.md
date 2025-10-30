---
title: 프로필 만들기
description: Campaign 웹에서 프로필을 만드는 방법을 알아봅니다.
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 46%

---

# 프로필 만들기 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="기본 세부 정보"
>abstract="이 섹션은 프로필의 기본 세부 사항에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="연락처 정보"
>abstract="이 섹션에서는 프로필의 연락처 정보에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="주소"
>abstract="이 섹션은 프로필의 우편 주소 및 주소 품질에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="계정 세부 정보"
>abstract="이 섹션은 프로필의 계정 세부 사항에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="더 이상 연락하지 않음"
>abstract="이 섹션에서는 프로필의 연락 환경 설정에 대한 인사이트를 제공합니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="사용자 정의 필드"
>abstract="사용자 정의 필드는 필요에 맞춰 인스턴스에 대해 구성된 특정 속성입니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="기타"
>abstract="이 섹션에서는 기본 제공되는 추가 속성을 제공합니다. 정보를 수정하려면 해당 필드 내에서 직접 변경한 다음 화면 오른쪽 상단에 있는 **저장** 버튼을 클릭합니다."

프로필을 만들려면 다음 단계를 수행합니다.

1. **[!UICONTROL 고객 관리]** > **[!UICONTROL 프로필]**(으)로 이동한 다음 화면 오른쪽 상단의 **[!UICONTROL 프로필 만들기]** 단추를 클릭합니다.

1. 프로필에 사용할 수 있는 속성 목록이 아래 표에 설명된 다른 섹션으로 구성되어 표시됩니다.

   ![섹션으로 구성된 프로필에 사용할 수 있는 특성 목록을 보여 주는 스크린샷](assets/create-profile.png){zoomable="yes"}

   | 속성 섹션 | 설명 |
   |  ---  |  ---  |
   | **기본 세부 정보** | 프로필의 이름 또는 생년월일 등 프로필에 대한 기본 정보.<br/>기본적으로 프로필은 **[!UICONTROL 받는 사람]** 폴더에 저장됩니다. 원하는 위치로 이동하여 변경할 수 있습니다. [폴더 작업 방법 알아보기](../get-started/permissions.md#folders) |
   | **연락처 정보** | 이메일 주소 또는 전화번호 등 프로필의 연락처 정보. |
   | **주소** | 프로필의 우편 주소입니다. 이 섹션에서는 주소 품질에 대한 평가도 제공합니다. &#39;성&#39;, &#39;구/군/시&#39; 및 &#39;우편 번호&#39; 필드를 지정한 경우 프로필 주소는 유효한 것으로 간주됩니다. |
   | **계정 세부 정보** | 상태 또는 계정 번호와 같은 프로필 계정에 대한 정보. |
   | **더 이상 연락하지 않음** | 프로필의 연락처 기본 설정입니다. 이러한 옵션 중 하나를 선택하면 프로파일이 차단 목록에 추가하다에 표시됩니다.<br/>예를 들어 받는 사람이 뉴스레터에서 구독 취소 링크를 클릭한 경우 이 정보가 연락처 데이터에 추가됩니다. 이러한 수신자는 더 이상 선택한 채널을 타겟팅하지 않습니다. [Adobe Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=ko){target="_blank"}에서 격리 관리에 대해 자세히 알아보세요. |
   | **사용자 정의 필드** | 사용자 정의 필드가 구성된 경우 이 섹션에 표시됩니다. 사용자 지정 필드는 Adobe Campaign 콘솔을 통해 **[!UICONTROL 프로필]** 스키마에 추가된 추가 특성입니다. 자세한 내용은 [Adobe Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=ko){target="_blank"}를 참조하세요 |
   | **기타** | 추가 기본 제공 속성. |

1. 프로필을 구성한 후 **[!UICONTROL 만들기]**&#x200B;를 클릭하여 데이터베이스에 저장합니다.

   저장한 후 언제든지 프로필 목록에서 프로필을 열어 편집할 수 있습니다. [프로필의 세부 정보를 탐색하는 방법을 알아봅니다](profile-view.md).