---
title: 사용자 정의 필드
description: 사용자 정의 필드를 구성하는 방법 알아보기
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 19%

---

# 사용자 정의 필드 구성 {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="사용자 정의 필드"
>abstract="사용자 정의 필드는 Adobe Campaign 콘솔을 통해 기본 스키마에 추가되는 추가 속성입니다. 이제 웹 사용자 인터페이스에서 사용할 수 있습니다."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ko-KR" text="릴리스 정보 참조"



사용자 정의 필드는 Adobe Campaign 콘솔을 통해 기본 스키마에 추가되는 추가 속성입니다. 자세한 내용은 [Adobe Campaign v8 설명서](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}를 참조하세요.

이러한 사용자 정의 필드는 프로필 또는 테스트 프로필의 세부 사항 등 다양한 화면에 표시됩니다.

웹 사용자 인터페이스에서 사용자 정의 필드를 만들 수는 없지만 표시되는 방식을 수정할 수는 있습니다. 수정 사항은 모든 Campaign 사용자에게 적용됩니다.

>[!NOTE]
>
>사용자 정의 필드를 수정하려면 관리자 권한이 있어야 합니다.

사용자 정의 필드는 다음 스키마에서 사용할 수 있습니다.

* 수신자 (nms)
* 캠페인(nms)
* 게재(nms)
* 시드 주소(nms)

사용자 정의 필드를 구성하려면 다음 단계를 수행합니다.

1. **관리**&#x200B;에서 **스키마**&#x200B;를 클릭합니다.

   ![](assets/custom-fields.png){zoomable="yes"}

1. 원하는 스키마(예: **수신자(nms)** 스키마)를 찾습니다.

   ![](assets/custom-fields2.png){zoomable="yes"}

1. **추가 작업** 단추를 클릭하고 **사용자 지정 세부 정보 편집**&#x200B;을 선택합니다.

   ![](assets/custom-fields3.png){zoomable="yes"}

   **사용자 지정 세부 정보 편집** 화면에 모든 사용자 지정 필드와 해당 형식이 표시됩니다.

   ![](assets/custom-fields4.png){zoomable="yes"}

   이 화면에서는 다음 작업을 수행할 수 있습니다.

   * 위쪽 및 아래쪽 화살표를 사용하여 여러 필드의 순서를 변경합니다.
   * 필수 필드 만들기: **필수** 상자를 선택합니다.
   * 필드를 표시하거나 숨깁니다. **표시** 단추를 클릭하십시오.
   * 가시성 조건 추가: **다음의 경우 표시** 단추를 클릭하고 사용 가능한 xtk 함수를 사용하여 xtk 식을 작성합니다.

1. 사용자 정의 필드를 표시하는 화면으로 이동합니다. 이 예에서는 프로필 세부 사항 화면입니다.

   ![](assets/custom-fields5.png){zoomable="yes"}
