---
audience: end-user
title: 푸시 알림 게재 디자인
description: Adobe Campaign 웹을 사용하여 푸시 알림 게재를 디자인하는 방법을 알아봅니다
badge: 레이블=“Alpha” 유형=“Positive”
source-git-commit: fbedfc5d1886b86932c156574037549270480f44
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 13%

---

# 푸시 게재 디자인 {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Android 콘텐츠 푸시"
>abstract="Android 콘텐츠 푸시를 정의합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="iOS 콘텐츠 푸시"
>abstract="iOS 콘텐츠 푸시를 정의합니다."

## 메시지 {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Firebase Cloud Messaging을 사용하면 두 가지 유형의 메시지 중에서 선택할 수 있습니다.

* 다음 **데이터 메시지**&#x200B;클라이언트 앱에서 처리됩니다. 메시지는 android 알림을 생성하고 장치에 표시하는 모바일 애플리케이션으로 직접 전송됩니다. 데이터 메시지에는 사용자 정의 애플리케이션 변수만 포함됩니다.

   다음을 클릭합니다. **[!UICONTROL 메시지]** 필드를 작성하고 표현식 편집기를 사용하여 콘텐츠를 정의하고 데이터를 개인화하며 다이내믹 콘텐츠를 추가합니다.

* FCM SDK에 의해 자동으로 처리되는 알림 메시지. FCM은 클라이언트 앱을 대신하여 사용자의 장치에 메시지를 자동으로 표시합니다. 알림 메시지에는 사전 정의된 매개 변수 및 옵션 세트가 포함되어 있지만 사용자 지정 애플리케이션 변수를 사용하여 추가로 개인화할 수 있습니다.

   메시지를 작성하려면 **[!UICONTROL 제목]** 및 **[!UICONTROL 본문]** 필드. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다.

   푸시 알림을 추가로 개인화하기 위해 푸시 알림에 추가할 이미지를 선택하고, 알림의 아이콘을 선택하여 프로필의 디바이스 및 색상을 표시할 수 있습니다.

>[!TAB iOS]

![](assets/push_content_1.png)

메시지를 작성하려면 **[!UICONTROL 제목]** 및 **[!UICONTROL 본문]** 필드. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다.

다음을 추가할 수 있습니다. **[!UICONTROL 부제]**: iOS 알림 페이로드의 자막 매개 변수 값입니다. 이 섹션을 참조하십시오.

자동 푸시 모드에서는 &quot;자동&quot; 알림을 모바일 애플리케이션으로 전송할 수 있습니다. 사용자는 알림이 도착한 것을 알지 못합니다. 애플리케이션에 바로 전송됩니다.

>[!ENDTABS]

## 고급 설정 {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

| 매개변수 | 설명 |
|---------|---------|
| **[!UICONTROL 사운드]** | 장치에서 알림을 받을 때 소리가 재생되도록 설정합니다. |
| **[!UICONTROL 알림 횟수]** | 애플리케이션 아이콘에 직접 표시할 읽지 않은 새 정보의 수를 설정합니다. |
| **[!UICONTROL 채널 ID]** | 알림의 채널 ID를 설정합니다. 이 채널 ID의 알림을 수신하려면 먼저 앱에서 이 채널 ID로 채널을 만들어야 합니다. |
| **[!UICONTROL 클릭 동작]** | 사용자 알림의 사용자 클릭과 관련된 작업을 설정합니다. |
| **[!UICONTROL 태그]** | 알림 대화 상자에서 기존 알림을 바꾸는 데 사용되는 식별자를 설정합니다. |
| **[!UICONTROL 우선 순위]** | 알림의 우선 순위 수준을 기본값, 최소, 낮음 또는 높음으로 설정합니다. 자세한 내용은 FCM 설명서를 참조하십시오. |
| **[!UICONTROL 가시성]** | 알림의 가시성 수준을 공개, 비공개 또는 비밀로 설정합니다. 자세한 내용은 FCM 설명서를 참조하십시오. |
| **[!UICONTROL 고정]** | 비활성화되면 사용자가 알림을 클릭할 때 자동으로 알림이 해제됩니다. 활성화되면 사용자가 클릭해도 알림이 계속 표시됩니다. |

>[!TAB iOS]

![](assets/push_content_2.png)

| 매개변수 | 설명 |
|---------|---------|
| **[!UICONTROL 중요 경고 모드]** | 사용자의 전화기가 포커스 모드로 설정되어 있거나 iPhone이 음소거된 경우에도 알림에 사운드를 추가하려면 이 옵션을 활성화합니다. |
| **[!UICONTROL 정리 배지]** | 배지 값을 새로 고치려면 이 옵션을 활성화합니다. |
| **[!UICONTROL 알림 횟수]** | 애플리케이션 아이콘에 읽지 않은 새 정보의 수를 직접 표시하는 데 사용할 숫자를 설정하십시오. |
| **[!UICONTROL 수량]** | 0~100의 사운드 볼륨입니다. |
| **[!UICONTROL 변경 가능한 콘텐츠]** | 모바일 애플리케이션에서 미디어 콘텐츠를 다운로드하도록 하려면 이 옵션을 활성화합니다. 자세한 내용은 [Apple 개발자 설명서](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)를 참조하십시오. |
| **[!UICONTROL 관련성 점수]** | 관련성 점수를 0에서 100으로 설정합니다. 시스템은 이 옵션을 사용하여 알림 요약의 알림을 정렬합니다. |
| **[!UICONTROL 중단 수준]** | <ul> <li>**[!UICONTROL 활성]**: 기본적으로 설정되어 있으므로 시스템에서 알림을 즉시 표시하고 화면을 켜며 사운드를 재생할 수 있습니다. 알림은 포커스 모드를 통과하지 않습니다.</li><li>**[!UICONTROL 수동]**: 화면에 불이 들어오거나 소리가 재생되지 않고 알림 목록에 알림이 추가됩니다. 알림은 포커스 모드를 통과하지 않습니다.</li><li>**[!UICONTROL 시간에 민감함]**: 시스템에서 알림을 즉시 표시하고 화면을 켜며 사운드를 재생하고 포커스 모드를 중단할 수 있습니다. 이 수준에서는 Apple의 특별한 권한이 필요하지 않습니다.</li> <li>**[!UICONTROL 중요]**: 시스템에서 알림을 즉시 표시하고 화면을 켜며 음소거 스위치 또는 포커스 모드를 건너뜁니다. 이 수준에는 Apple의 특별한 권한이 필요합니다.</ul> |
| **[!UICONTROL Thread-id]** | 관련 알림을 함께 그룹화하는 데 사용되는 식별자. |
| **[!UICONTROL 범주]** | 작업 단추를 표시할 범주 ID의 이름입니다. 이러한 알림은 사용자가 애플리케이션을 열거나 탐색하지 않고도 알림에 응답하여 다른 작업을 보다 빠르게 수행할 수 있도록 합니다. |
| **[!UICONTROL 대상 콘텐츠 ID]** | 알림이 열릴 때 앞으로 가져올 애플리케이션 창을 대상으로 지정하는 데 사용되는 식별자입니다. |
| **[!UICONTROL 이미지 실행]** | 표시할 론치 이미지 파일의 이름입니다. 사용자가 애플리케이션을 시작하도록 선택하면 애플리케이션의 시작 화면 대신 선택한 이미지가 표시됩니다. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



