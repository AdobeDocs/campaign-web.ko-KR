---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign Web UI에서 콘텐츠를 개인화하는 방법 알아보기
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 7a58b8323dbecc7cca0ba513d98a5afb213d3bc2
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 59%

---


# 내장된 콘텐츠 블록 {#ootb-content-blocks}

Adobe Campaign은 사전 구성된 콘텐츠 블록 목록을 제공합니다. 이러한 콘텐츠 블록은 동적이고 개인화된 블록이며 게재에 삽입할 수 있는 특정 렌더링을 포함합니다. 예를 들어 미러 페이지에 로고, 인사말 메시지 또는 링크를 추가할 수 있습니다.

게재에 콘텐츠 블록을 추가하려면 다음 단계를 수행합니다.

1. 게재를 열고 콘텐츠를 편집합니다.

1. 콘텐츠 블록을 추가할 필드를 찾은 다음 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘을 클릭하여 표현식 편집기를 엽니다.

   ![](assets/content-block-access.png){width="800" align="center"}

1. 표현식 편집기에서 **[!UICONTROL 콘텐츠 블록]** 왼쪽 메뉴.

1. 콘텐츠 블록을 추가하려면 콘텐츠 내에서 원하는 위치에 커서를 놓고 &#39;+&#39; 단추를 클릭하여 삽입합니다.

   ![](assets/content-blocks.png){width="800" align="center"}

내장된 콘텐츠 블록은 다음과 같습니다.

* **[!UICONTROL Purl 개인화 승인]**
* **[!UICONTROL 기본 옵트아웃 배너]**
* **[!UICONTROL Adobe Campaign에 의해 활성화됨]**: “Adobe Campaign에서 활성화됨” 로고를 삽입합니다.
* **[!UICONTROL Facebook 사전 입력]**
* **[!UICONTROL 고유 명사 서식 지정 기능]**: **[!UICONTROL toSmartCase]** 자바스크립트 기능을 생성합니다. 이 기능은 각 단어의 첫 글자를 대문자로 바꿉니다.
* **[!UICONTROL 인사말]**: 수신자의 전체 이름과 함께 쉼표가 뒤따르는 인사말을 삽입합니다. 예: “안녕하세요 John Doe 님,”
* **[!UICONTROL 로고 삽입]**: 인스턴스 설정에 정의된 로고를 삽입합니다.
* **[!UICONTROL 미러 페이지 링크]**: [미러 페이지](../content/mirror-page.md)에 대한 링크를 삽입합니다. 기본 형식은 “이 메시지가 제대로 표시되지 않는 경우 여기를 클릭하십시오.”입니다.
* **[!UICONTROL 미러 페이지 URL]**: 미러 페이지 URL을 삽입하여 게재 디자이너가 링크를 확인할 수 있도록 합니다.
* **[!UICONTROL 알림 스타일]**
* **[!UICONTROL 단일 모드의 오퍼 수락 URL]**: 오퍼를 **[!UICONTROL 수락됨]**&#x200B;으로 설정할 수 있는 URL을 삽입합니다. 상호 작용 모듈이 활성화된 경우 이 블록을 사용할 수 있습니다.
* **[!UICONTROL 등록 확인]**: 구독을 확인할 수 있는 링크를 삽입합니다.
* **[!UICONTROL 등록 링크]**: 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다. 기본 콘텐츠는 “등록하려면 여기를 클릭하십시오.”입니다.
* **[!UICONTROL 등록 링크(레퍼러 포함)]**: 방문자 및 게재를 식별할 수 있는 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다.
* **[!UICONTROL 등록 페이지 URL]**: 구독 URL을 삽입합니다.
* 소셜 네트워크 공유 링크
* **[!UICONTROL 콘텐츠 이메일 스타일]** 및 **[!UICONTROL 알림 스타일]**: 미리 정의된 HTML 스타일로 이메일 형식을 지정하는 코드를 생성합니다.
* **[!UICONTROL 구독 취소 링크]**: 모든 게재에서 구독을 취소(차단 목록에 추가)할 수 있는 링크를 삽입합니다. 기본 관련 콘텐츠는 다음과 같습니다. “귀하가 ***조직 이름***&#x200B;의 소식을 받고 있거나 제휴를 맺고 있기 때문에 이 메시지가 전송되었습니다. 더 이상 ***조직 이름***&#x200B;에서 메시지를 받지 않으려면 여기를 클릭하십시오.”

>[!NOTE]
>
>게재 개인화를 최적화할 수 있도록 Adobe Campaign v8 콘솔에서 새 블록을 정의할 수 있습니다. 다음에서 자세히 알아보기 [Campaign v8(콘솔) 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}.

