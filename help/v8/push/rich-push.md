---
audience: end-user
title: 리치 푸시 알림 게재 디자인
description: Adobe Campaign 웹을 사용하여 풍부한 푸시 알림 게재를 디자인하는 방법을 알아봅니다
hide: true
hidefromtoc: true
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '1407'
ht-degree: 4%

---

# Android 리치 푸시 게재 디자인 {#content-push}

Firebase Cloud Messaging을 사용하면 두 가지 유형의 메시지 중에서 선택할 수 있습니다.

* 다음 **[!UICONTROL 데이터 메시지]** 는 클라이언트 앱에서 처리됩니다. 이러한 메시지는 모바일 애플리케이션으로 직접 전송되며, 모바일 애플리케이션은 디바이스에 Android 알림을 생성하고 표시합니다. 데이터 메시지에는 사용자 정의 애플리케이션 변수만 포함됩니다.

* 다음 **[!UICONTROL 알림 메시지]** FCM SDK에 의해 자동으로 처리됩니다. FCM은 클라이언트 앱을 대신하여 사용자의 장치에 메시지를 자동으로 표시합니다. 알림 메시지에는 사전 정의된 매개 변수 및 옵션 세트가 포함되어 있지만 사용자 지정 애플리케이션 변수를 사용하여 추가로 개인화할 수 있습니다.

![](assets/rich_push.png){zoomable=&quot;yes&quot;}

## 알림 콘텐츠 정의 {#push-message}

푸시 게재가 만들어지면 해당 콘텐츠를 정의할 수 있습니다. 아래 탭을 탐색하여 각 템플릿에 대한 메시지를 작성하는 방법을 알아보십시오.

세 가지 템플릿을 사용할 수 있습니다.

* **기본 템플릿** 간단한 아이콘과 함께 제공되는 이미지를 사용하여 알림을 보낼 수 있습니다.

* **기본 템플릿** 알림에 텍스트, 이미지 및 버튼을 포함할 수 있습니다.

* **회전 템플릿** 사용자가 스와이프할 수 있는 텍스트 및 여러 이미지로 알림을 보낼 수 있습니다.

이러한 템플릿을 개인화하는 방법에 대한 자세한 내용을 보려면 아래 탭으로 이동하십시오.

>[!BEGINTABS]

>[!TAB 기본 템플릿]

1. 다음에서 **[!UICONTROL 템플릿]** 드롭다운, 선택 **[!UICONTROL 기본값]**.

   ![](assets/rich_push_default.png)

1. 메시지를 작성하려면 **[!UICONTROL 제목]** 및 **[!UICONTROL 메시지]** 필드.

   ![](assets/rich_push_default_2.png)

1. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다. [자세히 알아보기](../personalization/personalize.md)

1. 다음을 정의합니다. **[!UICONTROL 클릭 동작]** 알림의 사용자 클릭에 연결됩니다. 이는 사용자가 특정 화면을 열거나 앱에서 특정 작업을 수행하는 것과 같이 알림과 상호 작용할 때의 동작을 결정합니다.

1. 푸시 알림을 추가로 개인화하려면 다음을 선택할 수 있습니다. **[!UICONTROL 이미지]** 푸시 알림 및 알림에 추가할 URL **[!UICONTROL 아이콘]** 을 입력하여 프로필 디바이스에 표시할 수 있습니다.

   ![](assets/rich_push_default_3.png)

1. 구성 **[!UICONTROL 고급 설정]** 푸시 알림. [자세히 알아보기](#push-advanced)

메시지 콘텐츠를 정의했으면 테스트 구독자를 사용하여 메시지를 미리 보고 테스트할 수 있습니다.

>[!TAB 기본 템플릿]

1. 다음에서 **[!UICONTROL 템플릿]** 드롭다운, 선택 **[!UICONTROL 기본]**.

   ![](assets/rich_push_basic.png)

1. 메시지를 작성하려면 **[!UICONTROL 제목]**, **[!UICONTROL 메시지]** 및 **[!UICONTROL 확장된 메시지]** 필드.

   다음 **[!UICONTROL 메시지]** 텍스트가 축소된 뷰에 나타나는 동안 **[!UICONTROL 확장된 메시지]** 알림이 확장되면 표시됩니다.

   ![](assets/rich_push_basic_2.png)

1. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다. [자세히 알아보기](../personalization/personalize.md)

1. 다음을 정의하는 URL 추가 **[!UICONTROL 클릭 동작]** 알림의 사용자 클릭에 연결됩니다. 이는 사용자가 특정 화면을 열거나 앱에서 특정 작업을 수행하는 것과 같이 알림과 상호 작용할 때의 동작을 결정합니다.

1. 다음 항목 선택 **[!UICONTROL 링크 유형]** 에 추가한 URL **[!UICONTROL 클릭 동작]** 필드:

   * **[!UICONTROL 웹 URL]**: 웹 URL은 사용자를 온라인 컨텐츠로 안내합니다. 클릭하면 디바이스의 기본 웹 브라우저에서 를 열고 지정된 URL로 이동하라는 메시지가 표시됩니다.

   * **[!UICONTROL Deeplink]**: 딥링크는 앱이 닫힌 경우에도 앱 내의 특정 섹션으로 사용자를 안내하는 URL입니다. 클릭하면 대화 상자가 표시되어 사용자가 링크를 처리할 수 있는 다양한 앱 중에서 선택할 수 있습니다.

   * **[!UICONTROL 앱 열기]**: 앱 URL 열기를 사용하면 애플리케이션 내의 콘텐츠에 직접 연결할 수 있습니다. 이를 통해 애플리케이션이 명확화 대화 상자를 거치지 않고 특정 유형의 링크에 대한 기본 핸들러로 자리매김할 수 있습니다.

   Android 앱 링크를 처리하는 방법에 대한 자세한 내용은 을 참조하십시오. [Android 개발자 설명서](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. 푸시 알림을 추가로 개인화하려면 다음을 선택할 수 있습니다. **[!UICONTROL 이미지]** 푸시 알림 및 알림에 추가할 URL **[!UICONTROL 아이콘]** 을 입력하여 프로필 디바이스에 표시할 수 있습니다.

1. 클릭 **[!UICONTROL 추가 단추]** 다음 필드를 채웁니다.

   * **[!UICONTROL 레이블]**: 버튼에 표시되는 텍스트
   * **[!UICONTROL 링크 URI]**: 버튼을 클릭할 때 실행할 URI를 지정합니다.
   * **[!UICONTROL 링크 유형]**: 링크의 유형 **[!UICONTROL 웹 URL]**, **[!UICONTROL Deeplink]**, 또는 **[!UICONTROL 앱 열기]**.

   푸시 알림에 최대 3개의 버튼을 포함할 수 있는 옵션이 있습니다. 을(를) 선택한 경우 **[!UICONTROL 나중에 알림 단추]**, 최대 2개의 버튼만 포함할 수 있습니다.

   ![](assets/rich_push_basic_4.png)

1. 클릭 **[!UICONTROL 나중에 알림 추가]** 푸시 알림에 [나중에 알림] 옵션을 추가하는 버튼. 입력 **[!UICONTROL 레이블]** 및 **[!UICONTROL 타임스탬프]**.

   타임스탬프 필드에는 에포크를 나타내는 값(초)이 필요합니다.

   ![](assets/rich_push_basic_5.png)

1. 구성 **[!UICONTROL 고급 설정]** 푸시 알림. [자세히 알아보기](#push-advanced)

메시지 콘텐츠를 정의했으면 테스트 구독자를 사용하여 메시지를 미리 보고 테스트할 수 있습니다.

>[!TAB 회전 템플릿]

1. 다음에서 **[!UICONTROL 템플릿]** 드롭다운, 선택 **[!UICONTROL 회전판]**.

   ![](assets/rich_push_carousel.png)

1. 메시지를 작성하려면 **[!UICONTROL 제목]**, **[!UICONTROL 메시지]** 및 **[!UICONTROL 확장된 메시지]** 필드.

   다음 **[!UICONTROL 메시지]** 텍스트가 축소된 뷰에 나타나는 동안 **[!UICONTROL 확장된 메시지]** 알림이 확장되면 표시됩니다.

   ![](assets/rich_push_carousel_1.png)

1. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다. [자세히 알아보기](../personalization/personalize.md)

1. 다음을 정의하는 URL 추가 **[!UICONTROL 클릭 동작]** 알림의 사용자 클릭에 연결됩니다. 이는 사용자가 특정 화면을 열거나 앱에서 특정 작업을 수행하는 것과 같이 알림과 상호 작용할 때의 동작을 결정합니다.

1. 다음 항목 선택 **[!UICONTROL 링크 유형]** 에 추가한 URL **[!UICONTROL 클릭 동작]** 필드:

   * **[!UICONTROL 웹 사용자]**L: 웹 URL은 사용자를 온라인 컨텐츠로 안내합니다. 클릭하면 디바이스의 기본 웹 브라우저에서 를 열고 지정된 URL로 이동하라는 메시지가 표시됩니다.

   * **[!UICONTROL Deeplink]**: 딥링크는 앱이 닫힌 경우에도 앱 내의 특정 섹션으로 사용자를 안내하는 URL입니다. 클릭하면 대화 상자가 표시되어 사용자가 링크를 처리할 수 있는 다양한 앱 중에서 선택할 수 있습니다.

   * **[!UICONTROL 앱 열기]**: 앱 URL 열기를 사용하면 애플리케이션 내의 콘텐츠에 직접 연결할 수 있습니다. 이를 통해 애플리케이션이 명확화 대화 상자를 거치지 않고 특정 유형의 링크에 대한 기본 핸들러로 자리매김할 수 있습니다.

   Android 앱 링크를 처리하는 방법에 대한 자세한 내용은 을 참조하십시오. [Android 개발자 설명서](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. 푸시 알림을 추가로 개인화하려면 다음 알림을 선택할 수 있습니다. **[!UICONTROL 아이콘]** 을 입력하여 프로필 디바이스에 표시할 수 있습니다.

1. 방법 선택 **[!UICONTROL 회전판]** 운영됨:

   * **[!UICONTROL 자동]**: 이미지를 슬라이드로 자동 순환하여 사전 정의된 간격으로 전환합니다.
   * **[!UICONTROL 수동]**: 사용자가 슬라이드 사이를 수동으로 밀어 이미지를 탐색할 수 있습니다.

     활성화 **[!UICONTROL 필름 스트립]** 기본 슬라이드와 함께 이전 및 다음 이미지의 미리 보기를 포함하는 옵션.

1. 클릭 **[!UICONTROL 이미지 추가]** 이미지 URL과 텍스트를 입력합니다.

   최소 3개의 이미지와 최대 5개의 이미지를 포함해야 합니다.

   ![](assets/rich_push_carousel_3.png)

1. 아래쪽 및 위쪽 화살표를 사용하여 이미지 순서를 처리합니다.

1. 구성 **[!UICONTROL 고급 설정]** 푸시 알림. [자세히 알아보기](#push-advanced)

메시지 콘텐츠를 정의했으면 테스트 구독자를 사용하여 메시지를 미리 보고 테스트할 수 있습니다.

>[!ENDTABS]

## 푸시 알림 고급 설정 {#push-advanced}

![](assets/push_content_5.png){zoomable=&quot;yes&quot;}

| 매개변수 | 설명 |
|---------|---------|
| **[!UICONTROL 아이콘 색상]** | 16진수 색상 코드로 아이콘 색상을 설정합니다. |
| **[!UICONTROL 제목 색상]** | 16진수 색상 코드로 제목의 색상을 설정합니다. |
| **[!UICONTROL 메시지 텍스트 색상]** | 16진수 색상 코드를 사용하여 메시지 텍스트 색상을 설정합니다. |
| **[!UICONTROL 알림 배경색]** | 16진수 색상 코드로 알림 배경의 색상을 설정합니다. |
| **[!UICONTROL 사운드]** | 장치에서 알림을 받을 때 소리가 재생되도록 설정합니다. |
| **[!UICONTROL 알림 수]** | 애플리케이션 아이콘에 직접 표시할 읽지 않은 새 정보의 수를 설정합니다. 사용자는 이를 통해 보류 중인 알림 수를 빠르게 확인할 수 있습니다. |
| **[!UICONTROL 채널 ID]** | 알림의 채널 ID를 설정합니다. 이 채널 ID의 알림을 수신하려면 먼저 앱에서 이 채널 ID로 채널을 만들어야 합니다. |
| **[!UICONTROL 태그]** | 알림 대화 상자에서 기존 알림을 바꾸는 데 사용되는 식별자를 설정합니다. 이렇게 하면 여러 알림이 누적되는 것을 방지하고 최신 관련 알림만 표시됩니다. |
| **[!UICONTROL 우선 순위]** | 알림의 우선 순위 수준을 기본, 최소, 낮음 또는 높음으로 설정합니다. 우선 순위 수준은 알림이 표시되는 방식과 특정 시스템 설정을 우회할 수 있는지 여부에 영향을 주며 알림의 중요도와 긴급도를 결정합니다. 자세한 내용은 다음을 참조하십시오. [FCM 설명서](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL 가시성]** | 공개, 비공개 또는 비밀일 수 있는 알림의 가시성 수준을 설정합니다. 표시 수준은 잠금 화면 및 기타 중요 영역에 표시되는 알림 콘텐츠의 양을 결정합니다. 자세한 내용은 [FCM 설명서](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL 고정 알림]** | 활성화되면 사용자가 알림을 클릭한 후에도 알림이 계속 표시됩니다. <br>비활성화되면 사용자가 알림과 상호 작용할 때 알림이 자동으로 해제됩니다. 고정 동작을 사용하면 중요한 알림을 더 오랜 시간 동안 화면에 유지할 수 있습니다. |
| **[!UICONTROL 애플리케이션 변수]** | 알림 동작을 정의할 수 있습니다. 이러한 변수는 완전히 사용자 정의할 수 있으며 모바일 디바이스로 전송되는 메시지 페이로드의 일부로 포함됩니다. |