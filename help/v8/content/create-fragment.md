---
audience: end-user
title: 콘텐츠 조각 만들기
description: 콘텐츠 조각을 만드는 방법 알아보기
exl-id: 8f37e9e6-3085-4a68-9746-8ca34cfa4242
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 21%

---

# 콘텐츠 조각 만들기 {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="자신만의 콘텐츠 조각 정의"
>abstract="조각 속성과 만들고자 하는 조각의 유형을 정의합니다. 그런 다음 이메일 디자이너나 표현식 편집기를 사용하여 조각의 내용을 구성할 수 있습니다."

<!-- pas vu dans l'UI-->

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="조각 속성"
>abstract="조각의 레이블을 입력합니다. 필요한 경우 조각 내부 이름, 폴더, 설명 등의 추가 옵션을 정의할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="콘텐츠 조각 유형"
>abstract="만들고자 하는 조각의 유형을 선택합니다. **시각적 조각**&#x200B;은 여러 이메일 게재 또는 콘텐츠 템플릿에서 재사용할 수 있는 사전 정의된 시각적 블록입니다. **표현식 조각**&#x200B;은 표현식 편집기의 전용 항목에서 사용할 수 있는 사전 정의된 표현식입니다."

콘텐츠 조각을 만드는 방법에는 두 가지가 있습니다.

* **[!UICONTROL 조각]** 전용 메뉴를 사용하여 처음부터 조각을 만드십시오. [방법 알아보기](#create-from-scratch)
* 콘텐츠를 디자인할 때 콘텐츠의 일부를 조각으로 저장합니다. [방법 알아보기](#save-as-fragment)

  >[!NOTE]
  >
  >이 기능은 시각적 조각에만 사용할 수 있습니다. 식 조각은 **조각** 메뉴에서만 만들어집니다.

저장되면 콘텐츠 조각을 모든 게재 또는 콘텐츠 템플릿에서 사용할 수 있습니다.

## 처음부터 콘텐츠 조각 만들기 {#create-from-scratch}

콘텐츠 조각을 처음부터 만들려면 아래 단계를 수행합니다.

1. [콘텐츠 관리](#access-manage-fragments) > **[!UICONTROL 조각]** 왼쪽 메뉴를 통해 조각 목록에 액세스&#x200B;**[!UICONTROL 하고]**&#x200B;조각 만들기&#x200B;**[!UICONTROL 를 선택합니다.]**

   ![조각 만들기 옵션을 표시하는 조각 목록 화면](assets/fragments-list.png)

1. 조각의 레이블을 입력합니다. 필요한 경우 조각 내부 이름, 해당 폴더 및 설명과 같은 추가 옵션을 정의합니다.

1. 만들 조각 유형을 선택하십시오. **시각적 조각** 또는 **표현식 조각**. [시각적 조각과 식 조각의 차이점 알아보기](fragments.md)

   ![유형 선택을 표시하는 조각 만들기 화면](assets/fragment-create.png)

   >[!AVAILABILITY]
   >
   >시각적 조각에는 Campaign v8.6.4에 대한 업데이트가 필요합니다. 자세한 내용은 [Campaign v8 클라이언트 콘솔 릴리스 정보](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/releases/release-notes)를 참조하세요.

1. **만들기** 단추를 클릭합니다.

   * **시각적 조각**&#x200B;의 경우 [이메일 Designer](../email/get-started-email-designer.md)이 표시됩니다. 필요에 따라 캠페인 내의 전자 메일에 대해 편집할 것과 같은 방식으로 콘텐츠를 편집한 다음 **저장 및 닫기** 단추를 클릭합니다. 이미지, 링크, 개인화 필드 및 다이내믹 콘텐츠를 추가합니다.

     ![시각적 조각에 대한 전자 메일 Designer 화면](assets/fragment-designer.png)

   * **식 조각**&#x200B;의 경우 식 편집기가 열립니다. 개인화 및 작성 기능을 사용하여 콘텐츠를 작성한 다음 **확인**&#x200B;을 클릭합니다. [식 편집기로 작업하는 방법을 알아봅니다](../personalization/personalize.md)

     ![식 조각에 대한 식 편집기 화면](assets/fragment-expression.png)

1. 콘텐츠가 준비되면 **저장**&#x200B;을 클릭합니다.

이제 Campaign 내에서 게재 또는 [콘텐츠 템플릿](../content/use-email-templates.md)을(를) 빌드할 때 콘텐츠 조각을 사용할 준비가 되었습니다. 다음 섹션에서 시각적 및 표현식 조각을 사용하는 방법을 알아봅니다.
* [이메일에 비주얼 조각 추가](use-visual-fragments.md)
* [표현식 편집기에 표현식 조각 추가](use-expression-fragments.md)

## 콘텐츠를 시각적 조각으로 저장 {#save-as-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="조각으로 저장"
>abstract="콘텐츠를 시각적 조각으로 저장하려면 개인화 필드와 동적 콘텐츠를 비롯하여 조각에 포함할 요소를 선택합니다. 인접한 섹션만 선택할 수 있습니다. 빈 구조 또는 다른 콘텐츠 조각은 선택할 수 없습니다. 선택이 완료된 콘텐츠는 독립된 조각이 되어 조각 목록에 추가되고 전용 메뉴에서 액세스할 수 있게 됩니다. Campaign 내에서 이메일이나 콘텐츠 템플릿을 작성할 때 이 조각을 사용할 수 있습니다."

<!--pas vu dans l'UI-->

모든 이메일 콘텐츠는 나중에 다시 사용할 수 있도록 시각적 조각으로 저장할 수 있습니다. [콘텐츠 템플릿](../content/use-email-templates.md) 또는 [이메일](../email/get-started-email-designer.md) 게재를 디자인할 때 콘텐츠의 일부를 시각적 조각으로 저장하십시오. 이렇게 하려면 아래 단계를 수행합니다.

1. [전자 메일 Designer](../email/get-started-email-designer.md)에서 화면 오른쪽 상단의 **자세히** 단추를 클릭합니다.

1. 드롭다운 메뉴에서 **[!UICONTROL 조각으로 저장]**&#x200B;을(를) 선택합니다.

   ![전자 메일 Designer에서 조각으로 저장 옵션](assets/fragment-save-as.png)

1. **[!UICONTROL 조각으로 저장]** 화면이 표시됩니다. 개인화 필드 및 다이내믹 콘텐츠를 포함하여 조각에 포함할 요소를 선택합니다.

   >[!CAUTION]
   >
   >인접한 섹션만 선택할 수 있습니다. 빈 구조나 다른 콘텐츠 조각을 선택할 수 없습니다.

   ![요소 선택을 표시하는 조각으로 저장](assets/fragment-save-as-screen.png)

1. Click **[!UICONTROL Create]**. 조각 이름을 입력하고 저장합니다.

   ![시각적 조각에 대한 확인 화면 저장](assets/fragment-save-confirm.png)

   이 콘텐츠는 이제 독립 실행형 조각으로, [조각 목록](#manage-fragments)에 추가되고 전용 메뉴에서 액세스할 수 있습니다. Campaign 내에서 [전자 메일](../email/get-started-email-designer.md) 또는 [콘텐츠 템플릿](../content/use-email-templates.md)을(를) 빌드할 때 이 조각을 사용하십시오. [방법 알아보기](../content/use-visual-fragments.md)

>[!NOTE]
>
>새 조각에 대한 변경 사항은 원래 이메일이나 템플릿에 전파되지 않습니다. 마찬가지로 원본 컨텐츠가 이메일 또는 템플릿 내에서 편집되는 경우 새 조각은 수정되지 않습니다.

## 콘텐츠 조각 관리 {#manage-fragments}

조각 목록에서 콘텐츠 조각을 편집, 업데이트, 복제 또는 삭제할 수 있습니다.

### 콘텐츠 조각 편집 및 업데이트 {#edit-fragments}

컨텐츠 조각을 편집하려면 아래 단계를 따르십시오.

1. **[!UICONTROL 조각]** 목록에서 편집할 조각의 이름을 클릭합니다.
1. 조각의 콘텐츠를 열려면 **콘텐츠 편집** 단추를 클릭하십시오.

   ![조각에 대한 콘텐츠 편집 단추](assets/fragment-edit-content.png)

1. 필요한 사항을 변경하고 수정 사항을 저장합니다.

>[!CAUTION]
>
>조각에 대한 변경 사항은 이를 사용하여 게재 또는 템플릿에 전파됩니다.

### 컨텐츠 조각 삭제 {#delete-fragments}

컨텐츠 조각을 삭제하려면 다음 단계를 수행합니다.

1. 조각 목록으로 이동한 후 삭제할 조각 옆에 있는 **[!UICONTROL 추가 작업]** 단추를 클릭합니다.
1. **삭제**&#x200B;를 클릭하고 확인하십시오.

   ![조각 목록의 삭제 옵션](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>조각을 삭제하면 게재 및 이를 사용하는 템플릿이 업데이트됩니다. 조각은 콘텐츠에서 제거되지만 계속 참조됩니다. 해당 게재 및 템플릿에 조각 콘텐츠를 유지하려면 조각을 삭제하기 전에 상속을 중단합니다. [이 섹션에 자세히 설명되어 있습니다](use-visual-fragments.md#break-inheritance).

### 컨텐츠 조각 보관 {#archive}

더 이상 브랜드와 관련이 없는 조각을 보관하여 조각 목록을 정리할 수 있습니다. 이렇게 하려면 원하는 조각 옆에 있는 **[!UICONTROL 추가 작업]** 단추를 클릭하고 **[!UICONTROL 보관]**&#x200B;을 선택합니다. 조각이 조각 목록에서 제거되어 사용자가 향후 이메일 또는 템플릿에서 사용할 수 없습니다.

보관된 조각에 액세스하려면 필터링 창을 사용하여 표시합니다. 조각을 보관 해제하려면 **[!UICONTROL 추가 작업]** 단추를 클릭하고 **[!UICONTROL 보관 해제]**&#x200B;를 선택합니다.

![조각에 대한 보관 해제 옵션](assets/fragment-unarchive.png)

>[!NOTE]
>
>콘텐츠에 사용된 조각을 보관하는 경우 해당 콘텐츠는 영향을 받지 않습니다.

### 콘텐츠 조각 복제 {#duplicate-fragments}

콘텐츠 조각을 쉽게 복제하여 새 조각을 만들 수 있습니다. 기존 조각을 복제하려면 다음 단계를 수행합니다.

1. 조각 목록으로 이동한 후 복제할 조각 옆에 있는 **[!UICONTROL 추가 작업]** 단추를 클릭합니다.
1. **복제**&#x200B;를 클릭하고 확인하십시오.
1. 새 조각의 레이블을 입력하고 변경 사항을 저장합니다.

   조각이 콘텐츠 조각 목록에 추가됩니다. 필요에 따라 편집하고 구성합니다.