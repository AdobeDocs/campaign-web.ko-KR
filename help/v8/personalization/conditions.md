---
title: 조건부 콘텐츠 만들기
description: Adobe Campaign 웹에서 콘텐츠를 개인화할 조건을 정의하는 방법을 알아봅니다
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: f6e3fc0da05ecc2fda158c970458cc702b27079c
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 8%

---

# 조건부 콘텐츠 작성{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="조건부 콘텐츠 추가"
>abstract="조건부 콘텐츠 필드를 구성하여 수신자 프로필 데이터를 기반으로 고급 동적 개인화를 만듭니다. 텍스트 블록, 링크, 제목 줄 및/또는 이미지는 특정 조건이 충족되면 메시지 콘텐츠에서 교체됩니다."

## 조건부 콘텐츠 시작 {#gs}

조건부 콘텐츠는 수신자의 프로필 데이터를 기반으로 동적 개인화를 만들 수 있는 강력한 기능으로, 특정 조건이 충족되면 자동으로 텍스트 블록 및 이미지를 대체합니다. 이 기능은 캠페인을 새로운 차원으로 끌어올리고 대상자에게 고도로 타겟팅되고 개인 맞춤화된 경험을 제공할 수 있습니다.

조건부 콘텐츠 필드를 구성하여 예를 들어 수신자의 프로필을 기반으로 고급 동적 개인화를 만들 수 있습니다. 특정 조건이 충족되면 메시지 콘텐츠에서 텍스트 블록, 링크, 제목란 및/또는 이미지가 교체됩니다. 예를 들어 Adobe Campaign 데이터베이스의 Gender 필드 값에 따라 &#39;Mr&#39; 또는 &#39;Mrs&#39;를 표시하거나 수신자 기본 언어를 기반으로 다른 링크를 포함할 수 있습니다.

조건부 콘텐츠를 만들려면 **표현식 편집기** 특정 도우미 함수를 사용합니다. 이 방법은 제목란 또는 이메일 링크 및 텍스트/버튼 콘텐츠 구성 요소와 같이 표현식 편집기에 액세스할 수 있는 모든 필드의 모든 게재 채널에 사용할 수 있습니다. [표현식 편집기에 액세스하는 방법 알아보기](gs-personalization.md#access)

표현식 편집기 외에도 전용 을 활용할 수 있습니다 **조건부 콘텐츠 빌더** 이메일 본문의 요소에 대해 여러 변형을 만들 수 있는 이메일을 디자인할 때. [이메일에서 조건부 콘텐츠를 만드는 방법을 알아봅니다](#condition-condition-builder)

## 표현식 편집기에서 조건 만들기 {#condition-perso-editor}

표현식 편집기를 사용하여 게재에 대한 조건부 콘텐츠를 정의하려면 아래 단계를 수행합니다. 이 예제에서는 수신자의 언어(프랑스어 또는 영어)를 기반으로 조건부 콘텐츠를 만들려고 합니다.

1. 게재를 열고 콘텐츠 편집 섹션으로 이동합니다.

1. 조건부 콘텐츠를 추가할 필드를 찾습니다. 예를 들어 SMS 메시지에 조건부 콘텐츠를 추가할 수 있습니다.

1. 다음을 클릭합니다. **[!UICONTROL 개인화 대화 상자 열기]** 필드 옆에 있는 아이콘을 클릭하여 표현식 편집기를 엽니다.

   ![](assets/open-perso-editor-sms.png){zoomable=&quot;yes&quot;}

1. 개인화 편집기에서 **[!UICONTROL 조건]** 왼쪽에 있는 메뉴입니다.

1. 조건 작성을 시작하려면 옆에 있는 &#39;+&#39; 아이콘을 클릭합니다. **If** 함수. 다음 줄이 중앙 화면에 추가됩니다.`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * 바꾸기 `<FIELD>` 수신자의 언어와 같은 개인화 필드 사용: `recipient.language`.
   * 바꾸기 `<VALUE>` 를 만족시킬 값으로 채우십시오. 예를 들어, `'French'`.
   * 바꾸기 `Ìnsert content here` 지정된 조건을 충족하는 프로필에 표시할 콘텐츠로 대체합니다.

     ![](assets/condition-sample1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 수신자가 조건을 충족하지 않을 경우 표시되어야 하는 콘텐츠를 지정합니다. 이렇게 하려면 다음을 사용하십시오. **else** 도우미 함수:

   1. 표현식 닫기 태그 앞에 커서를 놓습니다. `%>` 을(를) 클릭하고 `+` 다음 옆에 **Else** 함수.

   1. 바꾸기 `Ìnsert content here` if 함수의 조건을 충족하지 않는 프로필에 표시할 콘텐츠로 식별됩니다.

   ![](assets/condition-sample2.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   다음을 사용할 수도 있습니다 **else if** 여러 콘텐츠 변형을 사용하여 조건을 빌드하는 도우미 함수입니다. 예를 들어 아래 표현식은 수신자의 언어에 따라 메시지의 세 가지 변형을 표시합니다.

   ![](assets/condition-sample3.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   >[!NOTE]
   >
   >도우미 함수가 추가될 때마다 (`<%`) 및 닫기(`%>`) 태그는 함수 앞뒤에 자동으로 추가됩니다.
   >
   >표현식 내에 &quot;Else&quot; 도우미 함수를 추가한 후의 예: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >구문 오류를 방지하려면 이러한 태그를 제거해야 합니다. 이 예에서 를 제거한 후 수정된 표현식은 **else** 함수 태그:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. 상태가 준비되면 콘텐츠를 저장하고 콘텐츠를 시뮬레이션하여 렌더링을 확인할 수 있습니다.

## 이메일에 조건부 콘텐츠 만들기 {#condition-condition-builder}

이메일의 조건부 콘텐츠는 다음 두 가지 방법으로 만들 수 있습니다.
* 도우미 함수를 사용하여 조건을 빌드하여 표현식 편집기에서
* 이메일을 디자인할 때 액세스할 수 있는 전용 조건부 콘텐츠 빌더에서.

다음 섹션에서는 이메일 디자이너의 조건부 콘텐츠 기능을 사용하여 조건을 만드는 방법에 대한 단계별 지침을 제공합니다. 표현식 편집기를 사용하여 조건을 만드는 방법에 대한 자세한 정보를 사용할 수 있습니다 [여기](#condition-perso-editor).

이 예제에서는 수신자의 언어를 기반으로 여러 변형이 있는 이메일 메시지를 만들려고 합니다. 다음 단계를 수행하십시오.

1. 이메일 게재를 만들거나 열고 콘텐츠를 편집한 다음 **[!UICONTROL 이메일 본문 편집]** 단추를 클릭하여 전자 메일 디자인 작업 영역을 엽니다.

1. 콘텐츠 구성 요소를 선택하고 **[!UICONTROL 조건부 콘텐츠 활성화]** 아이콘.

   ![](assets/condition-email-enable.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 다음 **[!UICONTROL 조건부 콘텐츠]** 창이 화면 왼쪽에서 열립니다. 이 창에서는 조건을 사용하여 선택한 콘텐츠 구성 요소의 변형을 여러 개 만들 수 있습니다.

1. 첫 번째 변형을 구성합니다. 마우스로 가리키기 **[!UICONTROL 변형 - 1]** 다음에서 **[!UICONTROL 조건부 콘텐츠]** 창을 클릭하고 **[!UICONTROL 조건 추가]** 단추를 클릭합니다.

   ![](assets/condition-add-condition.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 쿼리 모델러가 열립니다. 수신자의 프로필 데이터를 필터링하여 조건을 만들 수 있습니다. [쿼리 모델러를 사용하여 작업하는 방법을 알아봅니다](../query/query-modeler-overview.md).

   메시지의 첫 번째 변형에 대한 조건이 준비되면 **[!UICONTROL 확인]**. 이 예제에서는 언어가 &#39;프랑스어&#39;인 수신자를 타겟팅하는 규칙을 만들고 있습니다.

   ![](assets/condition-example.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 이제 규칙이 변형과 연결됩니다. 가독성을 높이기 위해 줄임표 메뉴를 클릭하여 변형 이름을 바꾸는 것이 좋습니다.

1. 메시지를 보낼 때 규칙이 충족되는 경우 구성 요소가 표시되는 방식을 구성합니다. 이 예제에서는 수신자의 선호 언어인 경우 프랑스어로 텍스트를 표시하려고 합니다.

   ![](assets/condition-email-variant1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. 콘텐츠 구성 요소에 필요한 만큼 변형을 추가합니다. 언제든지 변형 간을 전환하여 조건부 규칙에 따라 콘텐츠 구성 요소가 표시되는 방식을 확인할 수 있습니다.

   >[!NOTE]
   >메시지를 보낼 때 변형에 정의된 규칙을 충족하지 않는 경우 콘텐츠 구성 요소는에 정의된 콘텐츠를 표시합니다. **[!UICONTROL 기본 변형]** 다음에서 **[!UICONTROL 조건부 콘텐츠]** 창.
