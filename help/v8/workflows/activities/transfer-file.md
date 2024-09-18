---
audience: end-user
title: 파일 전송 활동 사용
description: 파일 전송 워크플로우 활동을 사용하는 방법 알아보기
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 29%

---

# 파일 전송 {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="파일 전송"
>abstract="**파일 전송** 활동을 통해 파일을 수신 또는 전송하거나, 파일 존재 여부를 테스트하거나, 서버에서 파일을 나열할 수 있습니다. 사용되는 프로토콜은 서버 간 프로토콜 또는 HTTP 프로토콜일 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="파일 전송 옵션"
>abstract="파일 전송 옵션"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="파일 전송 활동"
>abstract="파일 전송 활동"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="파일 전송 원격 서버"
>abstract="연결할 서버를 지정합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="파일 전송 소스"
>abstract="원하는 파일 이름을 입력하십시오."

**파일 전송** 활동은 **데이터 관리** 활동입니다. 파일을 받거나 보내고, 파일의 존재를 테스트하거나, 서버에 있는 파일을 나열할 수 있습니다. 사용되는 프로토콜은 서버 간 프로토콜 또는 HTTP 프로토콜일 수 있습니다.

>[!NOTE]
>
>Campaign 웹 사용자 인터페이스를 사용하여 **파일 전송** 및 **웹 다운로드** 기능을 모두 병합하여 두 활동을 하나로 통합했습니다. 이 통합은 어떤 식으로든 활동의 기능에 영향을 주지 않습니다.

**파일 전송** 활동을 구성하려면 아래 설명된 단계를 따르십시오.

## 전송 프로토콜 및 작업 선택 {#protocol}

1. 워크플로우에 **파일 전송** 활동을 추가한 다음 사용할 프로토콜에 따라 수행할 전송 유형을 지정합니다.

   * HTTP 프로토콜의 경우 **[!UICONTROL 웹 다운로드]**&#x200B;를 선택하십시오. 이를 통해 명시적 URL, 외부 계정 또는 Adobe Campaign 인스턴스에 파일을 다운로드하거나 GETPOST 을 수행할 수 있습니다.
   * 다른 서버 간 프로토콜 및 관련 작업을 보려면 **[!UICONTROL 파일 전송]**&#x200B;을 선택하십시오.

1. 활동으로 수행할 작업을 선택합니다. 사용 가능한 작업은 선택한 전송 유형에 따라 다릅니다. 자세한 내용을 보려면 아래 섹션을 확장하십시오.

   +++**파일 전송** 형식 활동에서 사용할 수 있는 액션

   * **[!UICONTROL 파일 다운로드]**: 서버에서 파일을 다운로드합니다.
   * **[!UICONTROL 파일 업로드]**: 서버에 파일을 업로드합니다.
   * **[!UICONTROL 파일이 있는지 테스트합니다]**: 지정된 파일이 서버에 있는지 확인합니다. 활동 후 &quot;파일이 있음&quot; 및 &quot;파일이 없음&quot; 두 개의 아웃바운드 전환을 생성합니다.
   * **[!UICONTROL 파일 목록]**: 서버에서 사용할 수 있는 모든 파일을 나열합니다.

+++

   +++**웹 다운로드** 유형 활동에서 사용할 수 있는 액션

   * **[!UICONTROL 단순 전송(GET)]**: 파일을 검색합니다.
   * **[!UICONTROL 양식을 사용하여 전송(POST)]**: 파일 및 추가 매개 변수를 업로드합니다.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. 기본적으로 파일 업로드 작업의 경우 활동은 이전 활동에 지정된 파일을 사용합니다. 다른 파일을 사용하려면 **[!UICONTROL 이전 활동에서 파일 사용]** 옵션을 끄고 **[!UICONTROL 파일 추가]** 단추를 클릭하십시오.

   **[!UICONTROL Source]** 필드에 원하는 파일 이름을 입력하거나 표현식 편집기를 사용하여 이벤트 변수를 사용하여 파일 이름을 계산합니다. [이벤트 변수 및 식 편집기로 작업하는 방법을 알아봅니다](../event-variables.md). 작업을 반복하여 파일을 필요한 만큼 추가합니다.

## 전송 대상 정의 {#destination}

1. **[!UICONTROL 원격 서버]** 섹션에서 다음 방법 중 하나를 사용하여 연결할 서버를 지정합니다.

   * **[!UICONTROL 외부 계정에 정의된 연결 매개 변수를 사용합니다]**: 외부 계정의 연결 매개 변수를 사용하여 서버에 연결합니다. **[!UICONTROL 서버 폴더]** 필드에 파일(또는 파일 목록 작업을 위한 폴더)의 경로를 지정합니다.
   * **[!UICONTROL 빠른 구성]**: 파일(또는 파일 목록 작업의 폴더)의 URL을 입력합니다.
   * **[!UICONTROL Adobe Campaign 인스턴스]**(웹 다운로드 유형 활동): Adobe Campaign 인스턴스 서버에서 파일을 다운로드합니다.

   ![](../assets/workflow-transfer-file-server.png)

1. 웹 다운로드 POST 작업의 경우 작업과 함께 추가 매개 변수를 전달할 수 있습니다. 이렇게 하려면 **[!UICONTROL 매개 변수 추가]** 단추를 클릭한 다음 매개 변수의 이름과 값을 지정하십시오. 필요한 만큼 매개 변수를 추가할 수 있습니다.

1. 기본적으로 파일 업로드의 경우 서버에 업로드된 파일은 자동으로 저장됩니다. 이 기록을 보관하지 않으려면 **[!UICONTROL 보낸 파일 기록 보관]** 옵션을 끄십시오.

## 내역 설정 {#historization}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="파일 기록"
>abstract="**[!UICONTROL 파일 전송]** 활동이 실행될 때마다 업로드 또는 다운로드한 파일이 전용 폴더에 저장됩니다. 워크플로의 각 파일 전송 활동마다 폴더가 하나씩 생성됩니다. 기본적으로 파일은 처리되기 전에 Adobe Campaign 설치 폴더의 기본 저장 디렉터리(`/vars`)에 저장됩니다. 특정 폴더를 사용하려면 **[!UICONTROL 기본 스토리지 디렉터리 사용]** 옵션을 끄고 디렉터리 경로를 입력하십시오."

**[!UICONTROL 파일 전송]** 활동이 실행될 때마다 업로드 또는 다운로드한 파일이 전용 폴더에 저장됩니다. 워크플로의 각 파일 전송 활동마다 폴더가 하나씩 생성됩니다. 기본적으로 파일은 처리되기 전에 Adobe Campaign 설치 폴더의 기본 저장 디렉터리(`/vars`)에 저장됩니다. 특정 폴더를 사용하려면 **[!UICONTROL 기본 스토리지 디렉터리 사용]** 옵션을 끄고 디렉터리 경로를 입력하십시오.

![](../assets/workflow-transfer-file-historization.png)

서버의 물리적 공간을 유지하려면 이 폴더의 크기를 제한할 수 있어야 합니다. 이를 위해 활동 폴더의 최대 파일 수나 총 크기를 정의할 수 있습니다. 기본적으로 파일 100개와 50MB가 승인됩니다.

활동이 실행될 때마다 폴더를 다음과 같이 확인합니다.

* 활동 실행 24시간 이전에 만든 파일만 고려합니다.
* 고려하는 파일 수가 **[!UICONTROL 파일 수]** 필드의 값보다 큰 경우 허용되는 최대 파일 수에 도달할 때까지 가장 오래된 파일부터 삭제합니다.
* 고려하는 파일의 총 크기가 **[!UICONTROL 최대 크기(MB)]** 매개 변수의 값보다 큰 경우, 허용되는 최대 크기(MB)에 도달할 때까지 가장 오래된 파일부터 삭제합니다.

>[!CAUTION]
>
>활동을 다시 실행하지 않는 경우 해당 폴더는 확인되거나 삭제되지 않습니다. 따라서 대용량 파일을 전송할 때는 주의하십시오.

## 고급 및 오류 관리 옵션 {#advanced}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="전송 후 소스 파일 삭제"
>abstract="전송이 성공적으로 완료되면 소스 파일을 삭제합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="세션 로그 표시"
>abstract="전송 작업과 관련된 정보가 워크플로 로그에 표시됩니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="모든 파일 나열"
>abstract="이 옵션은 **vars.filenames** 이벤트 변수에서 서버에 있는 모든 파일의 색인을 생성합니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="누락된 파일 처리"
>abstract="이 옵션을 사용하면 활동 후 **파일 없음** 아웃바운드 전환을 활성화할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="오류 처리"
>abstract="이 옵션을 사용하면 활동 후 **오류** 아웃바운드 전환을 활성화할 수 있습니다."

1. **[!UICONTROL 고급 옵션]**&#x200B;에서는 구성 중인 활동 유형에 따라 추가 옵션을 사용할 수 있습니다. 자세한 내용을 보려면 아래 섹션을 확장하십시오.

   +++**[!UICONTROL 파일 전송]** 유형 활동에 대한 추가 옵션

   * **[!UICONTROL 전송 후 원본 파일을 삭제합니다]**: 전송 후 원본 파일을 지웁니다.
   * **[!UICONTROL 세션 로그를 표시합니다]**: 이 옵션을 활성화하면 워크플로우가 실행되면 전송 작업과 관련된 정보가 워크플로우 로그에 표시됩니다.
   * **[!UICONTROL 모든 파일 나열]**(파일 나열 작업): 이 옵션은 서버에 있는 모든 파일을 `vars.filenames` 이벤트 변수로 색인화합니다. 이때 파일 이름은 `n`자로 구분됩니다. [이벤트 변수를 사용하여 작업하는 방법을 알아봅니다](../event-variables.md)

+++

   +++**[!UICONTROL 웹 다운로드]** 유형 활동에 대한 추가 옵션

   * **[!UICONTROL 리디렉션 따르기]**: 파일 리디렉션을 사용하면 재정의를 사용하여 데이터 입력 또는 출력을 다른 형식의 장치로 보낼 수 있습니다.
   * **[!UICONTROL 파일에 HTTP 헤더를 추가]**: 경우에 따라 파일에 추가 HTTP 헤더를 추가할 수 있습니다. 가장 일반적으로 이러한 헤더는 문제 해결 목적으로 [CORS(원본 간 리소스 공유)](https://developer.mozilla.org/docs/Web/HTTP/CORS)에 대한 추가 정보를 제공하거나 특정 캐싱 지침을 설정하는 데 사용됩니다.
   * **[!UICONTROL HTTP 반환 코드 무시]**: HTTP 상태 코드라고도 하는 HTTP 반환 코드는 HTTP 요청의 결과를 나타냅니다.

1. **[!UICONTROL 오류 처리]** 옵션을 사용하면 전송 중에 오류가 발생하는 경우 활동 후 &quot;오류&quot; 아웃바운드 전환을 활성화할 수 있습니다.

   또한 **파일 전송** 유형 활동의 경우 **[!UICONTROL 누락된 파일 처리]** 옵션을 사용하면 지정된 경로에서 파일을 사용할 수 없는 경우 활동 후에 &quot;파일 없음&quot; 아웃바운드 전환을 활성화할 수 있습니다.
