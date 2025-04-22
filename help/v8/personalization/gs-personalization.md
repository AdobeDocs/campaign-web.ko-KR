---
title: 다이내믹 콘텐츠를 만드는 방법
description: 개인화 및 조건부 콘텐츠를 사용하여 다이내믹 콘텐츠를 만드는 방법에 대해 알아봅니다.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 100%

---

# 다이내믹 콘텐츠를 만드는 방법 {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="개인화"
>abstract="개인화 편집기를 통해 모든 데이터를 선택하고, 배열하고, 사용자 정의하고 검증하여 콘텐츠에 대해 맞춤화된 경험을 만들 수 있습니다. 프로필 데이터를 활용하여 각 수신자에 맞게 메시지를 개인화하고, 조건부 콘텐츠를 생성하여 각 수신자에 맞게 메시지를 적응하고 관련 콘텐츠만 표시할 수 있습니다."

마케팅 담당자는 당사의 서비스에 관심이 있는 고객을 대상으로 효과적인 관련 콘텐츠를 제공하여 고객 참여를 유도하는 것이 중요합니다. 수신자의 범위가 다양하므로 여러 사용자에게 흥미를 일으키는 다양한 마케팅 콘텐츠를 만드는 데 오랜 시간이 걸릴 수 있습니다. 여기서 동적 콘텐츠가 필수입니다.

Adobe Campaign Web 동적 콘텐츠 기능을 사용하여 수신자에 대해 수집한 정보를 기반으로 콘텐츠를 사용자 정의할 수 있습니다. 동적 콘텐츠를 활용하여 원치 않거나 불필요한 제품 또는 서비스 마케팅을 방지하면서 마케팅 활동의 관련성을 높일 수 있습니다. 이 접근 방식을 사용하면 콘텐츠를 더 매력적으로 만들 수 있고 콘텐츠를 읽을 가능성이 높아집니다. 또한 콘텐츠를 개인화할 수 있어 수신자는 기계가 아닌 개인으로부터 정보를 수신하는 것처럼 느낍니다.

## 동적 콘텐츠를 만드는 방법 {#make-content-dyn}

Campaign Web 표현식 편집기에 JavaScript 구성을 삽입하여 메시지 콘텐츠를 동적으로 만들 수 있습니다. 메시지 전송 시 올바른 콘텐츠를 각 수신자에게 게재하기 위해 Adobe Campaign에서 해당 표현식을 해석합니다.

* **메시지 개인화** 이름, 관심 분야, 거주지, 구매 제품 등의 프로필 데이터를 활용하여 각 특정 수신자에게 게재합니다. 수신자, 메시지 또는 게재와 관련하여 개인화 편집기의 데이터베이스에서 사용 가능한 모든 필드를 선택할 수 있습니다. 이러한 개인화 속성은 메시지의 제목 줄이나 본문에 삽입할 수 있습니다. 다음 구문은 콘텐츠에 수신자의 도시를 삽입합니다. `<%= recipient.location.city %>`

  [설명: 개인화 속성을 사용하여 수신자의 도시를 제목 줄에 삽입하는 예.](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **조건부 콘텐츠 만들기** 각 수신자에 맞게 게재를 조정하고 고객에 대한 정보를 기반으로 특정 고객과 관련된 콘텐츠만 표시합니다. 이를 통해 조건에 &#x200B;&#x200B;따라 특정 텍스트 블록 및/또는 이미지를 표시할 수 있습니다. 예를 들어 특정 서비스에 대한 수신자 구독을 기반으로 이메일 배너를 조정합니다.

  [설명: 수신자의 구독에 따라 달라지는 이메일 배너의 조건부 콘텐츠 예.](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [비디오에서 이 기능 살펴보기](#video)

## 표현식 편집기에 액세스 {#access}

Adobe Campaign Web에서 제공하는 표현식 편집기를 통해 모든 데이터를 선택하고, 배열하고, 사용자 정의하고 검증하여 개인 맞춤화 콘텐츠를 경험할 수 있습니다. 표현식 편집기는 제목 줄 필드나 이메일 링크 및 텍스트/버튼 콘텐츠 구성 요소 등 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘과 함께 모든 필드의 모든 채널에서 사용할 수 있습니다.

다음은 동적 콘텐츠에 따라 표현식 편집기에 액세스하는 방법에 대한 몇 가지 예입니다.

* *발신자 이름 필드에서 표현식 편집기에 액세스*

  [설명: 발신자 이름 필드에서 표현식 편집기에 액세스의 예.](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *이메일 텍스트 구성 요소에서 표현식 편집기에 액세스*

  [설명: 이메일 텍스트 구성 요소에서 표현식 편집기에 액세스의 예.](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *이메일의 링크에서 표현식 편집기에 액세스*

  [설명: 이메일의 링크에서 표현식 편집기에 액세스의 예.](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>이메일을 디자인할 때는 표현식 편집기 외에 전용 조건부 콘텐츠 빌더를 사용할 수도 있습니다. [이메일의 조건부 콘텐츠를 빌드하는 방법 알아보기](conditions.md)

## 사용 방법 비디오 {#video}

표현식 편집기를 사용하여 메시지를 개인화하거나 조건부 콘텐츠를 추가하여 메시지 내용을 다이내믹하게 만드는 방법에 대해 알아봅니다.

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)