---
audience: end-user
product: campaign
title: 콘텐츠 템플릿 작업
description: 템플릿을 만들어 Adobe Campaign 이메일의 콘텐츠를 재사용하는 방법 알아보기
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 19%

---

# 콘텐츠 템플릿 작업 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="콘텐츠 템플릿"
>abstract="디자인 프로세스를 가속화하고 개선하기 위해 독립 실행형 이메일 템플릿을 만들어 Adobe Campaign에서 사용자 정의 콘텐츠를 쉽게 재사용할 수 있습니다. 이러한 콘텐츠 템플릿은 기본 제공 또는 사용자 정의 템플릿을 기반으로 처음부터 디자인하거나, 기존 콘텐츠에서 생성하거나, 콘텐츠 템플릿 편집기에서 가져올 수 있습니다."

디자인 프로세스를 가속화하고 개선하기 위해 독립 실행형 템플릿을 만들어 사용자 지정 콘텐츠를 여러 곳에서 쉽게 재사용할 수 있습니다 [!DNL Adobe Campaign]. 이러한 콘텐츠 템플릿은 기본 제공 또는 사용자 정의 템플릿을 기반으로 처음부터 디자인하거나, 기존 콘텐츠에서 생성하거나, 콘텐츠 템플릿 편집기에서 가져올 수 있습니다.

이 기능을 통해 콘텐츠 중심 사용자는 독립 실행형 템플릿에서 작업할 수 있으므로 마케팅 사용자는 이메일 캠페인 내에서 이를 재사용하고 조정할 수 있습니다.

>[!NOTE]
>
>현재는 **이메일** 콘텐츠 템플릿이 지원됩니다.

## 콘텐츠 템플릿 액세스 {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="템플릿 콘텐츠 편집"
>abstract="이메일 디자이너로 콘텐츠를 업데이트하려면 **콘텐츠 편집** 버튼을 클릭합니다."

콘텐츠 템플릿 목록에 액세스하려면 **[!UICONTROL 콘텐츠 관리]** > **[!UICONTROL 콘텐츠 템플릿]** 왼쪽 레일의 메뉴

![](assets/content-template-list.png){zoomable=&quot;yes&quot;}

이 대시보드는 사용 가능한 모든 콘텐츠 템플릿을 목록으로 표시합니다. 특정 항목을 필터링할 수 있습니다 [폴더](../get-started/permissions.md#folders) 드롭다운 목록 사용 또는 다음을 사용하여 규칙 추가 [쿼리 모델러](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png){zoomable=&quot;yes&quot;}

목록에서 기존 콘텐츠 템플릿을 편집, 복제 또는 삭제할 수 있습니다. 상위 섹션의 버튼을 사용하여 콘텐츠 템플릿을 만듭니다.


## 콘텐츠 템플릿 만들기 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="콘텐츠 템플릿 디자인"
>abstract="이메일 콘텐츠 템플릿을 디자인합니다."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="콘텐츠 템플릿 선택"
>abstract="이메일 콘텐츠 템플릿을 선택합니다."

콘텐츠 템플릿은 다음 방법으로 만들 수 있습니다. [기존 이메일을 템플릿으로 저장](#save-as-template)또는 이메일 템플릿 목록에서 **콘텐츠 템플릿 만들기** 단추, [아래에 자세히 설명됨](#create-template-from-scratch).

저장하면 이제 템플릿을 작성할 때 이 템플릿을 사용할 수 있습니다. [이메일](../email/create-email.md) 다음 범위 내 [!DNL Adobe Campaign]. [방법 알아보기](use-email-templates.md)

>[!NOTE]
>
>* 콘텐츠 템플릿에 대한 변경 사항은 이메일에 전파되지 않습니다.
>
>* 마찬가지로 전자 메일에서 템플릿을 사용하는 경우 전자 메일 콘텐츠를 편집해도 이전에 사용한 콘텐츠 템플릿에는 영향을 주지 않습니다.

### 새 콘텐츠 템플릿 만들기 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="템플릿 속성 정의"
>abstract="필요할 때 쉽게 검색할 이메일 콘텐츠 템플릿 속성을 정의합니다."

콘텐츠 템플릿 대시보드에서 새 콘텐츠 템플릿을 만들려면 다음 단계를 수행하십시오.

1. 에서 콘텐츠 템플릿 목록으로 이동합니다. **[!UICONTROL 콘텐츠 관리]** > **[!UICONTROL 콘텐츠 템플릿]** 왼쪽 레일.

1. 선택 **[!UICONTROL 템플릿 만들기]**.

   ![](assets/content-template-create.png){zoomable=&quot;yes&quot;}

1. 템플릿 레이블 및 속성을 입력합니다. 템플릿을 저장할 폴더를 선택할 수 있습니다. 기본적으로 콘텐츠 템플릿은 Adobe Campaign 계층의 전용 폴더에 저장됩니다. **[!UICONTROL 탐색기]** > **[!UICONTROL 리소스]** > **[!UICONTROL 템플릿]** > **[!UICONTROL 콘텐츠 템플릿]**. 의 폴더에 대해 자세히 알아보기 [이 페이지](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png){zoomable=&quot;yes&quot;}

1. 클릭 **[!UICONTROL 만들기]** 다양한 옵션에서 템플릿 디자인 방법을 선택합니다.

   * [처음부터 콘텐츠 디자인](create-email-content.md) 이메일 디자이너의 인터페이스를 통해

   * [코드 또는 복사하여 붙여넣기 원시 HTML](code-content.md) 이메일 디자이너에 바로 로그인합니다.

   * [기존 HTML 콘텐츠 가져오기](existing-content.md) .zip 폴더 또는 파일로 내보낼 때 시간별 세부기간이 작동하지 않는 문제를 해결했습니다.

   * 기본 제공 또는 사용자 지정 템플릿 목록의 기존 콘텐츠를 사용합니다. 이메일에서 콘텐츠 템플릿을 사용하는 단계는에 설명되어 있습니다 [이 섹션](use-email-templates.md).

   ![](assets/email_designer-templates.png){zoomable=&quot;yes&quot;}

1. 이메일 디자이너가 표시됩니다. 선택한 옵션에 따라 이메일에 대해 수행하는 것과 동일한 방식으로 콘텐츠를 필요에 따라 편집합니다. 에서 이메일 디자이너를 사용하는 방법을 알아봅니다. [이 섹션](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. 템플릿이 준비되면 **[!UICONTROL 저장]**.

   필요한 경우 템플릿 이름 옆에 있는 화살표를 클릭하여 로 돌아갑니다. **[!UICONTROL 세부 사항]** 템플릿을 스크린하고 편집합니다.

   ![](assets/content-template-save-back.png){zoomable=&quot;yes&quot;}

템플릿은에서 사용할 수 있습니다 **[!UICONTROL 콘텐츠 템플릿]** 목록을 표시합니다. [자세히 알아보기](#access-templates)

이제 이 템플릿을 사용하여 새 콘텐츠를 작성할 수 있습니다. 템플릿은에서 사용할 수 있습니다. **[!UICONTROL 저장된 템플릿]** 이메일 디자이너의 탭. [방법 알아보기](use-email-templates.md)

### 이메일 콘텐츠를 템플릿으로 저장 {#save-as-template}

한 번 [이메일 디자인](create-email-content.md), 나중에 다시 사용할 수 있도록 이 콘텐츠를 템플릿으로 저장할 수 있습니다. Adobe Campaign 환경의 모든 사용자는 저장된 템플릿을 사용할 수 있습니다.

이메일 내용을 템플릿으로 저장하려면 다음 단계를 따르십시오.

1. 이메일 디자이너에서 **[!UICONTROL 자세히]** 화면 오른쪽 상단의 단추.

1. 선택 **[!UICONTROL 콘텐츠 템플릿으로 저장]** 드롭다운 메뉴에서 을(를) 선택합니다.

   ![](assets/email_designer-save-template.png){zoomable=&quot;yes&quot;}

1. 이 템플릿의 이름을 입력하고 저장합니다.

   ![](assets/email_designer-template-name.png){zoomable=&quot;yes&quot;}

템플릿이에 저장되고 표시됩니다. **[!UICONTROL 콘텐츠 템플릿]** 목록을 표시합니다. 이 템플릿은 목록에 있는 다른 항목으로 액세스, 편집 및 삭제할 수 있는 독립 실행형 콘텐츠 템플릿이 됩니다. [자세히 알아보기](#access-manage-templates)

이제 이 템플릿을 사용하여 새 콘텐츠를 작성할 수 있습니다. 템플릿은에서 사용할 수 있습니다. **[!UICONTROL 저장된 템플릿]** 이메일 디자이너의 탭. [방법 알아보기](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable=&quot;yes&quot;}


>[!NOTE]
>
>새 템플릿에 대한 변경 사항은 원래 이메일에 전파되지 않습니다. 마찬가지로 원본 콘텐츠가 해당 이메일 내에서 편집되는 경우 새 템플릿은 수정되지 않습니다.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## 콘텐츠 템플릿 수정 {#modify-delete}

기존 콘텐츠 템플릿을 업데이트하려면 다음 단계를 따르십시오.

1. 콘텐츠 템플릿 목록에서 수정하려는 템플릿의 레이블을 클릭하여 편집합니다.

1. 다음을 클릭합니다. **[!UICONTROL 콘텐츠 편집]** 단추를 클릭하여 콘텐츠를 [이메일 디자이너](get-started-email-designer.md).

![](assets/content-template-edition.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>콘텐츠 템플릿에 대한 변경 사항은 이 콘텐츠 템플릿을 사용하는 이메일에 전파되지 않습니다.

## 콘텐츠 템플릿 삭제 {#content-delete}

다음 두 가지 방법으로 콘텐츠 템플릿을 삭제할 수 있습니다.

* 콘텐츠 템플릿 목록에서 줄임표 버튼을 클릭한 다음 을 선택합니다 **삭제**

  ![대시보드에서 콘텐츠 템플릿 삭제](assets/content-template-list-delete.png)

* 콘텐츠 템플릿 자체에서 **자세히** 버튼을 누른 다음 선택 **삭제**


>[!NOTE]
>
>콘텐츠 템플릿을 삭제해도 이 템플릿을 사용하여 만든 게재에는 영향을 주지 않습니다.


## 콘텐츠 템플릿 복제 {#content-duplicate}

다음 두 가지 방법으로 콘텐츠 템플릿을 복제할 수 있습니다.

* 콘텐츠 템플릿 목록에서 줄임표 버튼을 클릭한 다음 을 선택합니다 **복제**

* 콘텐츠 템플릿 자체에서 **자세히** 버튼을 누른 다음 선택 **복제**

두 경우 모두 복제를 확인하여 새 콘텐츠 템플릿을 만듭니다. 새 콘텐츠 템플릿의 레이블은 입니다. **다음의 사본`<label of the initial campaign`**. 템플릿 설정으로 이동하여 이 레이블을 업데이트합니다.

