---
title: Campaign 콘텐츠 개인화
description: Adobe Campaign Web UI에서 콘텐츠를 개인화하는 방법 알아보기
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: ht
source-wordcount: '277'
ht-degree: 100%

---


# 내장된 콘텐츠 블록 {#ootb-content-blocks}

내장된 콘텐츠 블록은 다음과 같습니다.

* **[!UICONTROL Adobe Campaign에 의해 활성화됨]**: “Adobe Campaign에서 활성화됨” 로고를 삽입합니다.
* **[!UICONTROL 고유 명사 서식 지정 기능]**: **[!UICONTROL toSmartCase]** 자바스크립트 기능을 생성합니다. 이 기능은 각 단어의 첫 글자를 대문자로 바꿉니다.
* **[!UICONTROL 인사말]**: 수신자의 전체 이름과 함께 쉼표가 뒤따르는 인사말을 삽입합니다. 예: “안녕하세요 John Doe 님,”
* **[!UICONTROL 로고 삽입]**: 인스턴스 설정에서 정의한 로고를 삽입합니다.
* **[!UICONTROL 미러 페이지 링크]**: [미러 페이지](../content/mirror-page.md)에 대한 링크를 삽입합니다. 기본 형식은 “이 메시지가 제대로 표시되지 않는 경우 여기를 클릭하십시오.”입니다.
* **[!UICONTROL 미러 페이지 URL]**: 미러 페이지 URL을 삽입하여 게재 디자이너가 링크를 확인할 수 있도록 합니다.
* **[!UICONTROL 단일 모드의 오퍼 수락 URL]**: 오퍼를 **[!UICONTROL 수락됨]**&#x200B;으로 설정할 수 있는 URL을 삽입합니다. 상호 작용 모듈이 활성화된 경우 이 블록을 사용할 수 있습니다.
* **[!UICONTROL 등록 확인]**: 구독을 확인할 수 있는 링크를 삽입합니다.
* **[!UICONTROL 등록 링크]**: 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다. 기본 콘텐츠는 “등록하려면 여기를 클릭하십시오.”입니다.
* **[!UICONTROL 등록 링크(레퍼러 포함)]**: 방문자 및 게재를 식별할 수 있는 구독 링크를 삽입합니다. 이 링크는 인스턴스 설정에서 정의됩니다.
* **[!UICONTROL 등록 페이지 URL]**: 구독 URL을 삽입합니다.
* **[!UICONTROL 콘텐츠 이메일 스타일]** 및 **[!UICONTROL 알림 스타일]**: 미리 정의된 HTML 스타일로 이메일 형식을 지정하는 코드를 생성합니다.
* **[!UICONTROL 구독 취소 링크]**: 모든 게재에서 구독을 취소(차단 목록에 추가)할 수 있는 링크를 삽입합니다. 기본 관련 콘텐츠는 다음과 같습니다. “귀하가 ***조직 이름***&#x200B;의 소식을 받고 있거나 제휴를 맺고 있기 때문에 이 메시지가 전송되었습니다. 더 이상 ***조직 이름***&#x200B;에서 메시지를 받지 않으려면 여기를 클릭하십시오.”
