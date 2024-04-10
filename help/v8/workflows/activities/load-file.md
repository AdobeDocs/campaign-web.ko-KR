---
audience: end-user
title: 파일 로드 워크플로우 활동 사용
description: 파일 로드 워크플로우 활동을 사용하는 방법 알아보기
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 1eaa2710e682e9038befc5d0752c064e2bb48521
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 47%

---

# 파일 로드 {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="파일 로드 활동"
>abstract="**파일 로드** 활동은 **데이터 관리** 활동입니다. 이 활동을 사용하여 외부 파일에 저장된 데이터로 작업할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="샘플 파일"
>abstract="샘플 파일"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="파일 이름"
>abstract="파일 이름"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Target 데이터베이스"
>abstract="Target 데이터베이스"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="파일 로드 활동에 대한 관리 거부"
>abstract="파일 로드 활동에 대한 관리 거부"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="관리 아웃바운드 전환 거부"
>abstract="관리 아웃바운드 전환 거부"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="거부에 대한 관리 아웃바운드 전환 거부"
>abstract="거부에 대한 관리 아웃바운드 전환 거부"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="파일 로드 활동에 대한 서식 지정"
>abstract="파일 로드 활동에 대한 서식 지정"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="파일 로드 활동에 대한 대상 파일"
>abstract="파일 로드 활동에 대한 대상 파일"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="파일 로드 활동에 대한 값 재매핑"
>abstract="파일 로드 활동에 대한 값 재매핑"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="파일 로드 명령"
>abstract="사전 처리를 위해 임의 명령을 허용하는 것은 보안과 관련된 문제이므로 보안 옵션인 XtkSecurity_Disable_Preproc을 비활성화하여 사전 정의된 명령 목록을 강제로 사용하도록 하십시오."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="가져오기 후 파일 삭제"
>abstract="파일을 가져온 후 서버에서 원본 파일을 삭제하려면 **가져오기 후 파일 삭제**&#x200B;를 토글하십시오."

**파일 로드** 활동은 **데이터 관리** 활동입니다. 이 활동을 사용하여 외부 파일에 저장된 프로필 및 데이터를 사용합니다. 프로필 및 데이터는 데이터베이스에 추가되지 않지만 입력 파일의 모든 필드는 다음에 사용할 수 있습니다. [개인화](../../personalization/gs-personalization.md)또는 를 사용하여 프로필 또는 기타 테이블을 업데이트할 수 있습니다.

>[!NOTE]
>지원되는 파일 형식은 텍스트(TXT)와 쉼표로 구분된 값(CSV)입니다.

이 활동은 다음에서 사용할 수 있습니다. [조정](reconciliation.md) 활동을 통해 미식별 데이터를 기존 리소스에 연결할 수 있습니다. 예를 들어 **파일 로드** 활동은 다음에 배치할 수 있습니다. **조정** 활동(비표준 데이터를 데이터베이스로 가져오는 경우)

## 파일 로드 활동 구성 {#load-configuration}

다음 단계에 따라 **파일 로드** 활동:

1. 드래그 앤 드롭 **파일 로드** 활동을 워크플로우에 추가합니다. 다음을 클릭합니다. **파일에서 선택** 단추를 클릭합니다.

1. 사용할 로컬 파일을 선택합니다. 형식은 다음과 일치해야 합니다. [샘플 파일](../../audience/file-audience.md#sample-file).

1. 화면 중앙 섹션에서 데이터가 매핑되는 방식을 미리 보고 확인합니다.

   ![](../assets/load-file.png)

1. 사용 **열** 왼쪽 창의 섹션에서 각 열의 데이터 유형과 너비를 조정할 수 있습니다.

1. 다음에서 **서식** 열 구성 아래에 있는 섹션에서 데이터를 올바르게 가져오도록 외부 파일의 형식을 지정하는 방법을 지정합니다.

1. 설정이 적절하면 **확인**&#x200B;을 클릭합니다.

## 예제{#load-example}

와 함께 사용되는 외부 파일 로드 샘플 **조정** 활동은에서 사용할 수 있습니다. [이 섹션](reconciliation.md#reconciliation-example).
