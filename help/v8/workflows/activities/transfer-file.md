---
audience: end-user
title: 파일 전송 활동 사용
description: 파일 전송 워크플로우 활동을 사용하는 방법 알아보기
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 15%

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
>abstract="파일 전송 원격 서버"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="파일 전송 소스"
>abstract="파일 전송 소스"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="전송 후 소스 파일 삭제"
>abstract="전송 후 소스 파일 삭제"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="세션 로그 표시"
>abstract="세션 로그 표시"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="모든 파일 나열"
>abstract="모든 파일 나열"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="파일 기록"
>abstract="파일 기록"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="누락된 파일 처리"
>abstract="누락된 파일 처리"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="오류 처리"
>abstract="오류 처리"

다음 **파일 전송** 활동은 입니다. **데이터 관리** 활동. 파일을 받거나 보내고, 파일의 존재를 테스트하거나, 서버에 있는 파일을 나열할 수 있습니다. 사용되는 프로토콜은 서버 간 프로토콜 또는 HTTP 프로토콜일 수 있습니다.

>[!NOTE]
>
>Campaign 웹 사용자 인터페이스를 사용하여 두 활동을 병합하여 하나로 통합했습니다 **파일 전송** 및 **웹 다운로드** 기능. 이 통합은 어떤 식으로든 활동의 기능에 영향을 주지 않습니다.

아래 설명된 단계에 따라 다음을 구성하십시오. **파일 전송** 활동.

## 전송 프로토콜 및 작업 선택 {#protocol}

1. 추가 **파일 전송** 활동을 워크플로우에 지정한 다음 사용할 프로토콜에 따라 수행할 전송 유형을 지정합니다.

   * HTTP 프로토콜의 경우 다음을 선택합니다 **[!UICONTROL 웹 다운로드]**. 이를 통해 명시적 URL, 외부 계정 또는 Adobe Campaign 인스턴스에 파일을 다운로드하거나 GETPOST 을 수행할 수 있습니다.
   * 다른 서버 간 프로토콜 및 관련 작업의 경우 **[!UICONTROL 파일 전송]**.

1. 활동으로 수행할 작업을 선택합니다. 사용 가능한 작업은 선택한 전송 유형에 따라 다릅니다. 자세한 내용을 보려면 아래 섹션을 확장하십시오.

   +++사용 가능한 작업 **파일 전송** 유형 활동

   * **[!UICONTROL 파일 다운로드]**: 서버에서 파일을 다운로드합니다.
   * **[!UICONTROL 파일 업로드]**: 서버에 파일을 업로드합니다.
   * **[!UICONTROL 파일이 있는지 테스트]**: 주어진 파일이 서버에 있는지 확인합니다. 활동 후 &quot;파일이 있음&quot; 및 &quot;파일이 없음&quot; 두 개의 아웃바운드 전환을 생성합니다.
   * **[!UICONTROL 파일 목록]**: 서버에서 사용할 수 있는 모든 파일을 나열합니다.

+++

   +++사용 가능한 작업 **웹 다운로드** 유형 활동

   * **[!UICONTROL 단순 전송(GET)]**: 파일을 검색합니다.
   * **[!UICONTROL 양식을 사용하여 전송(POST)]**: 파일 및 추가 매개 변수를 업로드합니다.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. 기본적으로 파일 업로드 작업의 경우 활동은 이전 활동에 지정된 파일을 사용합니다. 다른 파일을 사용하려면 **[!UICONTROL 이전 활동의 파일 사용]** 옵션을 끄고 **[!UICONTROL 파일 추가]** 단추를 클릭합니다.

   다음에서 **[!UICONTROL 소스]** 필드에 원하는 파일 이름을 입력하거나 표현식 편집기를 사용하여 이벤트 변수를 사용하여 파일 이름을 계산합니다. [이벤트 변수 및 표현식 편집기를 사용하여 작업하는 방법을 알아봅니다](../event-variables.md). 작업을 반복하여 파일을 필요한 만큼 추가합니다.

## 전송 대상 정의 {#destination}

1. 다음에서 **[!UICONTROL 원격 서버]** 섹션에서 다음 방법 중 하나를 사용하여 연결할 서버를 지정합니다.

   * **[!UICONTROL 외부 계정에 정의된 연결 매개 변수 사용]**: 외부 계정의 연결 매개 변수를 사용하여 서버에 연결합니다. 다음에서 **[!UICONTROL 서버 폴더]** 필드에 파일(또는 작업을 나열하는 파일의 폴더) 경로를 지정합니다.
   * **[!UICONTROL 빠른 구성]**: 파일(또는 작업을 나열하는 파일의 폴더)의 URL을 입력합니다.
   * **[!UICONTROL Adobe Campaign 인스턴스]** (웹 다운로드 유형 활동): Adobe Campaign 인스턴스 서버에서 파일을 다운로드합니다.

   ![](../assets/workflow-transfer-file-server.png)

1. 웹 다운로드 POST 작업의 경우 작업과 함께 추가 매개 변수를 전달할 수 있습니다. 이렇게 하려면 **[!UICONTROL 매개 변수 추가]** 그런 다음 매개 변수의 이름과 값을 지정합니다. 필요한 만큼 매개 변수를 추가할 수 있습니다.

1. 기본적으로 파일 업로드의 경우 서버에 업로드된 파일은 자동으로 저장됩니다. 이 기록을 유지하지 않으려면 **[!UICONTROL 보낸 파일 기록 보관]** 옵션 끄기.

## 내역 설정 {#historization}

매 시간 **[!UICONTROL 파일 전송]** 활동이 실행되면 업로드되거나 다운로드한 파일을 전용 폴더에 저장합니다. 워크플로우의 각 파일 전송 활동마다 폴더가 하나씩 생성됩니다. 기본적으로 파일은 Adobe Campaign 설치 폴더의 기본 스토리지 디렉터리(`/vars`)를 클릭하여 검색할 수 있습니다. 특정 폴더를 사용하려면 **[!UICONTROL 기본 저장소 디렉터리 사용]** 옵션을 끄고 디렉토리 경로를 입력합니다.

![](../assets/workflow-transfer-file-historization.png)

서버의 물리적 공간을 유지하려면 이 폴더의 크기를 제한할 수 있어야 합니다. 이를 위해 활동 폴더의 최대 파일 수나 총 크기를 정의할 수 있습니다. 기본적으로 파일 100개와 50MB가 승인됩니다.

활동이 실행될 때마다 폴더를 다음과 같이 확인합니다.

* 활동 실행 24시간 이전에 만든 파일만 고려합니다.
* 고려하는 파일 수가 의 값보다 큰 경우 **[!UICONTROL 파일 수]** 필드에서는 허용되는 최대 파일 수에 도달할 때까지 가장 오래된 파일부터 삭제합니다.
* 고려하는 파일의 총 크기가 의 값보다 큰 경우 **[!UICONTROL 최대 크기(MB)]** 매개 변수에서 허용되는 최대 크기(MB)에 도달할 때까지 가장 오래된 파일이 삭제됩니다.

>[!CAUTION]
>
>활동을 다시 실행하지 않는 경우 해당 폴더는 확인되거나 삭제되지 않습니다. 따라서 대용량 파일을 전송할 때는 주의하십시오.

## 고급 및 오류 관리 옵션 {#advanced}

1. 다음에서 **[!UICONTROL 고급 옵션]**&#x200B;를 통해 구성 중인 활동 유형에 따라 추가 옵션을 사용할 수 있습니다. 자세한 내용을 보려면 아래 섹션을 확장하십시오.

   +++추가 옵션 **[!UICONTROL 파일 전송]** 유형 활동

   * **[!UICONTROL 전송 후 소스 파일 삭제]**: 성공적으로 전송한 후 소스 파일을 지웁니다.
   * **[!UICONTROL 세션 로그 표시]**: 이 옵션이 활성화되면 워크플로우가 실행된 후 워크플로우 로그에 전송 작업과 관련된 정보가 표시됩니다.
   * **[!UICONTROL 모든 파일 나열]** (파일 목록 작업): 이 옵션은 서버에 있는 모든 파일을 `vars.filenames` 이벤트 변수. 여기서 파일 이름은 `n` 자. [이벤트 변수를 사용하여 작업하는 방법에 대해 알아봅니다](../event-variables.md)

+++

   +++추가 옵션 **[!UICONTROL 웹 다운로드]** 유형 활동

   * **[!UICONTROL 리디렉션 팔로우]**: 파일 리디렉션을 사용하면 재정의를 사용하여 데이터 입력 또는 출력을 다른 유형의 장치로 보낼 수 있습니다.
   * **[!UICONTROL 파일에 HTTP 헤더 추가]**: 경우에 따라 파일에 추가 HTTP 헤더를 추가할 수 있습니다. 가장 일반적으로 이러한 헤더는 문제 해결 목적으로 추가 정보를 제공하는 데 사용됩니다. [CORS(원본 간 리소스 공유)](https://developer.mozilla.org/docs/Web/HTTP/CORS)또는 특정 캐싱 지시문을 설정합니다.
   * **[!UICONTROL HTTP 반환 코드 무시]**: HTTP 상태 코드라고도 하는 HTTP 반환 코드는 HTTP 요청의 결과를 나타냅니다.

1. 다음 **[!UICONTROL 프로세스 오류]** 옵션을 사용하면 전송 중에 오류가 발생하는 경우 활동 후 &quot;오류&quot; 아웃바운드 전환을 활성화할 수 있습니다.

   또한 **파일 전송** 유형 활동, **[!UICONTROL 프로세스 누락 파일]** 옵션을 사용하면 지정된 경로에서 파일을 사용할 수 없는 경우 활동 후에 &quot;파일 없음&quot; 아웃바운드 전환을 활성화할 수 있습니다.
