---
audience: end-user
title: Campaign Web 사용자 인터페이스의 권한 관리
description: Campaign Web 사용자 인터페이스의 권한에 대해 자세히 알아보기
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 20%

---


# 사용 권한 {#permissions}

Adobe Campaign의 각 사용자는 애플리케이션에서 고유한 권한과 제한 사항이 있습니다.

사용자는 연산자 그룹의 일부일 수 있으며, 그룹의 권한을 상속합니다.

연산자는 사용 권한에 따라 다음을 수행할 수 있습니다.

* 특정 기능에 액세스
* 특정 데이터 액세스
* 특정 작업(만들기, 수정, 삭제)에 대한 액세스

## 폴더에 대한 권한 {#folder-permissions}

권한에 따라 **[!UICONTROL 폴더 설정]**의 폴더에 대한 권한을 보고 관리할 수 있습니다.
게재 폴더의 예제 아래에서 다음을 수행합니다.

![](assets/folder_settings.png){zoomable="yes"}

**[!UICONTROL 폴더 설정]**&#x200B;의 **[!UICONTROL 보안]** 섹션에서 폴더에 액세스할 수 있는 운영자 또는 그룹을 보고 관리(추가 또는 삭제)할 수 있습니다.

![](assets/folder_security.png){zoomable="yes"}

권한을 직접 클릭하여 **[!UICONTROL 허용됨]** 또는 **[!UICONTROL 거부됨]**&#x200B;으로 변경할 수 있습니다.

![](assets/folder_security_denied.png){zoomable="yes"}

**[!UICONTROL 전파]** 옵션이 활성화되면 폴더에 정의된 모든 권한이 모든 하위 폴더에 적용됩니다. 이러한 권한은 각 하위 폴더에 대해 오버로드될 수 있습니다.

**[!UICONTROL 시스템 폴더]** 옵션을 선택하면 해당 사용 권한에 관계없이 모든 연산자에 액세스할 수 있습니다.

[Adobe Campaign 콘솔의 폴더에 대한 권한을 관리](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions)할 수도 있습니다.
Campaign 웹 UI의 모든 권한은 Campaign 클라이언트 콘솔 권한과 동기화됩니다.
