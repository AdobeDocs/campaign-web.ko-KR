---
audience: end-user
title: 푸시 알림 게재 디자인
description: Adobe Campaign 웹을 사용하여 푸시 알림 게재를 디자인하는 방법을 알아봅니다
badge: label="제한 공개"
exl-id: 031bc38a-2435-4468-8ee6-3bcf1132da55
source-git-commit: ff8a8388cfe4124ccddeb789460be7845da41089
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 38%

---

# 푸시 메시지 게재 디자인 {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Android 콘텐츠 푸시"
>abstract="Android 디바이스에 대한 푸시 알림 내용을 정의합니다. 메시지 작성을 시작하려면 **콘텐츠 편집** 버튼을 클릭합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="iOS 콘텐츠 푸시"
>abstract="iOS 디바이스에 대한 푸시 알림 내용을 정의합니다. 메시지 작성을 시작하려면 **콘텐츠 편집** 버튼을 클릭합니다."

## 알림 콘텐츠 정의 {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="iOS 메시지 푸시"
>abstract="iOS 디바이스에 대한 푸시 알림 내용을 정의합니다. 메시지를 작성하려면 **제목** 및 **메시지** 필드를 클릭합니다. 표현식 편집기를 사용하여 데이터를 개인화하고 동적 콘텐츠를 추가합니다. 더 많은 사용자 정의 구성을 보려면 **고급 설정** 섹션으로 이동합니다."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_msg"
>title="iOS 메시지 푸시"
>abstract="Android 디바이스에 대한 푸시 알림 내용을 정의합니다. 메시지를 작성하려면 **제목** 및 **메시지** 필드를 클릭합니다. 표현식 편집기를 사용하여 데이터를 개인화하고 동적 콘텐츠를 추가합니다. 푸시 알림을 추가로 개인화하려면 푸시 알림에 추가할 이미지, 프로필 디바이스에 표시할 알림 아이콘 및 색상을 선택할 수 있습니다. 더 많은 사용자 정의 구성을 보려면 **고급 설정** 섹션으로 이동합니다."



>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="iOS에 대한 자동 알림"
>abstract="사일런트 푸시 모드를 사용하면 “자동” 알림을 모바일 애플리케이션으로 전송할 수 있습니다. 사용자는 알림이 도착했음을 알지 못합니다. 애플리케이션으로 직접 전송됩니다."

푸시 게재가 만들어지면 해당 콘텐츠를 정의할 수 있습니다. 매개 변수 및 설정은 모바일 운영 체제(Android 또는 iOS)에 따라 다릅니다. 아래 탭을 탐색하여 각 운영 체제에 대한 메시지를 작성하는 방법을 알아보십시오.

>[!BEGINTABS]

>[!TAB Android]

Firebase Cloud Messaging을 사용하면 두 가지 유형의 메시지 중에서 선택할 수 있습니다.

* 다음 **[!UICONTROL 데이터 메시지]** 는 클라이언트 앱에서 처리됩니다. 이러한 메시지는 모바일 애플리케이션으로 직접 전송되며, 모바일 애플리케이션은 디바이스에 Android 알림을 생성하고 표시합니다. 데이터 메시지에는 사용자 정의 애플리케이션 변수만 포함됩니다.

  콘텐츠를 정의하고, 데이터를 개인화하고, 동적 콘텐츠를 추가하려면 **[!UICONTROL 메시지]** 필드를 작성하고 표현식 편집기를 사용합니다. 이 편집기에 액세스하여 메시지를 사용자 정의할 수 있습니다.
다음에서 **[!UICONTROL 애플리케이션 변수]** 메뉴에서 애플리케이션 변수가 자동으로 추가됩니다. 이러한 변수를 사용하여 알림 동작을 정의할 수 있습니다. 예를 들어, 사용자가 알림을 활성화할 때 특정 애플리케이션 화면이 표시되도록 구성할 수 있습니다.

  ![](assets/push_content_4.png)

* 다음 **[!UICONTROL 알림 메시지]** FCM SDK에 의해 자동으로 처리됩니다. FCM은 클라이언트 앱을 대신하여 사용자의 장치에 메시지를 자동으로 표시합니다. 알림 메시지에는 사전 정의된 매개 변수 및 옵션 세트가 포함되어 있지만 사용자 지정 애플리케이션 변수를 사용하여 추가로 개인화할 수 있습니다.

  메시지를 작성하려면 **[!UICONTROL 제목]** 및 **[!UICONTROL 메시지]** 필드를 클릭합니다. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다.

  푸시 알림을 추가로 개인화하려면 푸시 알림에 추가할 이미지, 프로필의 디바이스에 표시할 알림의 아이콘 및 색상을 선택할 수 있습니다.

  ![](assets/push_content_3.png)

>[!TAB iOS]

메시지를 작성하려면 **[!UICONTROL 제목]** 및 **[!UICONTROL 메시지]** 필드를 클릭합니다. 표현식 편집기를 사용하여 콘텐츠를 정의하고, 데이터를 개인화하고, 다이내믹 콘텐츠를 추가합니다.

다음을 추가할 수 있습니다. **[!UICONTROL 부제]**: iOS 알림 페이로드의 자막 매개 변수 값입니다. 이 섹션을 참조하십시오.

사일런트 푸시 모드를 사용하면 “자동” 알림을 모바일 애플리케이션으로 전송할 수 있습니다. 사용자는 알림이 도착했음을 알지 못합니다. 애플리케이션으로 직접 전송됩니다.

![](assets/push_content_1.png)

>[!ENDTABS]

## 푸시 알림 고급 설정 {#push-advanced}


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings"
>title="푸시 알림에 대한 고급 설정"
>abstract="우선 순위, 관련 알림 수, 애플리케이션 변수 등과 같은 푸시 알림에 대한 고급 설정을 정의합니다."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_critical"
>title="중요 경고 모드"
>abstract="사용자의 휴대폰이 포커스 모드로 설정되어 있거나 디바이스가 음소거된 경우에도 알림에 소리를 추가하려면 이 옵션을 활성화합니다. 이렇게 하면 어떠한 경우에도 사용자가 중요한 알림을 수신할 수 있습니다."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_count"
>title="알림 횟수"
>abstract="이 옵션을 사용하여 읽지 않은 알림 수를 앱 아이콘에 바로 표시하도록 설정합니다. 사용자는 이를 통해 보류 중인 알림 수를 빠르게 확인할 수 있습니다."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="변경 가능한 콘텐츠"
>abstract="이 옵션을 사용하여 모바일 애플리케이션이 알림과 관련된 미디어 콘텐츠를 다운로드하도록 허용합니다."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_score"
>title="관련성 점수"
>abstract="알림 요약에서 알림 순서의 우선 순위를 지정하려면 관련성 점수를 0에서 100 사이로 설정하십시오. 점수가 높을수록 더 중요한 알림입니다."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_app_variables"
>title="애플리케이션 변수"
>abstract="애플리케이션 변수를 사용하여 알림 비헤이비어를 정의합니다. 이러한 변수는 완전히 사용자 정의할 수 있으며 모바일 디바이스로 전송되는 메시지 페이로드의 일부로 포함됩니다."


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_category"
>title="범주 ID"
>abstract="알림과 연결된 범주 ID의 이름을 지정합니다. 이렇게 하면 작업 버튼이 표시되어 사용자가 애플리케이션을 열지 않고도 알림에서 직접 다양한 작업을 수행할 수 있습니다."

고급 옵션은 모바일 운영 체제(Android 또는 iOS)에 따라 다릅니다. 아래 탭을 탐색하여 각 운영 체제에 대한 메시지 옵션을 정의하는 방법을 알아보십시오.

>[!BEGINTABS]

>[!TAB Android]

![](assets/push_content_5.png)

| 매개변수 | 설명 |
|---------|---------|
| **[!UICONTROL 사운드]** | 장치에서 알림을 받을 때 소리가 재생되도록 설정합니다. |
| **[!UICONTROL 알림 수]** | 애플리케이션 아이콘에 직접 표시할 읽지 않은 새 정보의 수를 설정합니다. 사용자는 이를 통해 보류 중인 알림 수를 빠르게 확인할 수 있습니다. |
| **[!UICONTROL 채널 ID]** | 알림의 채널 ID를 설정합니다. 이 채널 ID의 알림을 수신하려면 먼저 앱에서 이 채널 ID로 채널을 만들어야 합니다. |
| **[!UICONTROL 클릭 동작]** | 알림에 대한 사용자 클릭과 관련된 작업을 정의합니다. 이는 사용자가 특정 화면을 열거나 앱에서 특정 작업을 수행하는 것과 같이 알림과 상호 작용할 때의 동작을 결정합니다. |
| **[!UICONTROL 태그]** | 알림 대화 상자에서 기존 알림을 바꾸는 데 사용되는 식별자를 설정합니다. 이렇게 하면 여러 알림이 누적되는 것을 방지하고 최신 관련 알림만 표시됩니다. |
| **[!UICONTROL 우선 순위]** | 알림의 우선 순위 수준을 기본, 최소, 낮음 또는 높음으로 설정합니다. 우선 순위 수준은 알림이 표시되는 방식과 특정 시스템 설정을 우회할 수 있는지 여부에 영향을 주며 알림의 중요도와 긴급도를 결정합니다. 자세한 내용은 다음을 참조하십시오. [FCM 설명서](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL 가시성]** | 공개, 비공개 또는 비밀일 수 있는 알림의 가시성 수준을 설정합니다. 표시 수준은 잠금 화면 및 기타 중요 영역에 표시되는 알림 콘텐츠의 양을 결정합니다. 자세한 내용은 [FCM 설명서](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL 고정]** | 활성화되면 사용자가 알림을 클릭한 후에도 알림이 계속 표시됩니다. <br>비활성화되면 사용자가 알림과 상호 작용할 때 알림이 자동으로 해제됩니다. 고정 동작을 사용하면 중요한 알림을 더 오랜 시간 동안 화면에 유지할 수 있습니다. |
| **[!UICONTROL 애플리케이션 변수]** | 알림 동작을 정의할 수 있습니다. 이러한 변수는 완전히 사용자 정의할 수 있으며 모바일 디바이스로 전송되는 메시지 페이로드의 일부로 포함됩니다. |

>[!TAB iOS]

![](assets/push_content_2.png)

| 매개변수 | 설명 |
|---------|---------|
| **[!UICONTROL 중요 경고 모드]** | 사용자의 휴대폰이 포커스 모드로 설정되어 있거나 디바이스가 음소거된 경우에도 알림에 소리를 추가하려면 이 옵션을 활성화합니다. 이렇게 하면 중요한 알림을 사용자가 인지할 수 있습니다. 선택한 경우 볼륨 레벨 바를 사용하여 알림의 볼륨을 조정할 수 있습니다. 막대 위에 0에서 100 사이의 숫자가 있으면 설정이 반영됩니다. |
| **[!UICONTROL 정리 배지]** | 애플리케이션 아이콘에 표시된 배지 값을 새로 고치려면 이 옵션을 활성화합니다. 이는 배지가 읽지 않은 새로운 정보의 수를 정확하게 반영하도록 한다. |
| **[!UICONTROL 알림 수]** | 읽지 않은 새 정보의 수를 나타내는 애플리케이션 아이콘에 직접 표시되는 숫자를 설정하십시오. 이를 통해 사용자에게 빠른 시각적 참조를 제공합니다. |
| **[!UICONTROL 볼륨]** | 0~100의 사운드 볼륨입니다. |
| **[!UICONTROL 변경 가능한 콘텐츠]** | 모바일 애플리케이션이 알림과 연관된 미디어 콘텐츠를 다운로드하도록 하려면 이 옵션을 활성화합니다. 자세한 내용은 [Apple 개발자 설명서](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html)를 참조하십시오. |
| **[!UICONTROL 관련성 점수]** | 알림 요약에서 알림 순서의 우선 순위를 지정하려면 관련성 점수를 0에서 100 사이로 설정하십시오. 점수가 높을수록 더 중요한 알림입니다. |
| **[!UICONTROL 중단 수준]** | <ul> <li>**[!UICONTROL 활성]**: 기본적으로 설정되어 있으므로 시스템에서 알림을 즉시 표시하고 화면을 켜며 사운드를 재생할 수 있습니다. 알림은 포커스 모드를 통과하지 않습니다.</li><li>**[!UICONTROL 수동]**: 화면에 불이 들어오거나 소리가 재생되지 않고 알림 목록에 알림이 추가됩니다. 알림은 포커스 모드를 통과하지 않습니다.</li><li>**[!UICONTROL 시간에 민감함]**: 시스템에서 알림을 즉시 표시하고 화면을 켜며 사운드를 재생하고 포커스 모드를 중단할 수 있습니다. 이 수준에서는 Apple의 특별한 권한이 필요하지 않습니다.</li> <li>**[!UICONTROL 중요]**: 시스템에서 알림을 즉시 표시하고 화면을 켜며 음소거 스위치 또는 포커스 모드를 건너뜁니다. 이 수준에는 Apple의 특별한 권한이 필요합니다.</ul> |
| **[!UICONTROL Thread-id]** | 관련 알림을 함께 그룹화하는 데 사용되는 식별자. 스레드 ID가 동일한 알림은 알림 목록에서 단일 대화 또는 스레드로 구성됩니다. |
| **[!UICONTROL 범주]** | 알림과 연결된 범주 ID의 이름을 지정합니다. 이렇게 하면 작업 버튼이 표시되어 사용자가 애플리케이션을 열지 않고도 알림에서 직접 다양한 작업을 수행할 수 있습니다. |
| **[!UICONTROL 대상 콘텐츠 ID]** | 알림이 열릴 때 앞으로 가져올 애플리케이션 창을 대상으로 지정하는 데 사용되는 식별자입니다. |
| **[!UICONTROL 이미지 실행]** | 사용자가 알림에서 애플리케이션을 시작하도록 선택할 때 표시할 시작 이미지 파일의 이름을 지정합니다. 애플리케이션의 일반 시작 화면 대신 선택한 이미지가 표시됩니다. |
| **[!UICONTROL 애플리케이션 변수]** | 알림 동작을 정의할 수 있습니다. 이러한 변수는 완전히 사용자 정의할 수 있으며 모바일 디바이스로 전송되는 메시지 페이로드의 일부로 포함됩니다. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->
