---
audience: end-user
title: 파일 로드 워크플로우 활동 사용
description: 파일 로드 워크플로우 활동을 사용하는 방법 알아보기
badge: label="제한 공개"
source-git-commit: 88daf84e617595a80c5cd3fd536969618f0fdcf5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 33%

---

# 파일 로드 {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="파일 활동 로드"
>abstract="다음 **파일 로드** 활동은 입니다. **데이터 관리** 활동. 이 활동을 사용하여 외부 파일에 저장된 데이터로 작업합니다."

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
>title="파일 활동 로드에 대한 관리 거부"
>abstract="파일 활동 로드에 대한 관리 거부"

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
>title="파일 활동 로드에 대한 서식 지정"
>abstract="파일 활동 로드에 대한 서식 지정"


다음 **파일 로드** 활동은 입니다. **데이터 관리** 활동. 이 활동을 사용하여 외부 파일에 저장된 프로필 및 데이터를 사용합니다. 프로필 및 데이터는 데이터베이스에 추가되지 않지만 입력 파일의 모든 필드는 다음에 사용할 수 있습니다. [개인화](../../personalization/gs-personalization.md)또는 를 사용하여 프로필 또는 기타 테이블을 업데이트할 수 있습니다.


>[!NOTE]
>지원되는 파일 형식은 텍스트(TXT)와 쉼표로 구분된 값(CSV)입니다.


이 활동은 다음에서 사용할 수 있습니다. [조정](reconciliation.md) 활동을 통해 미식별 데이터를 기존 리소스에 연결할 수 있습니다. 예를 들어 **파일 로드** 활동은 다음에 배치할 수 있습니다. **조정** 활동(비표준 데이터를 데이터베이스로 가져오는 경우)


## 파일 로드 활동 구성 {#load-configuration}

다음 단계에 따라 **파일 로드** 활동:


1. 드래그 앤 드롭 **파일 로드** 활동을 워크플로우에 추가합니다. 다음을 클릭합니다. **파일에서 선택** 단추를 클릭합니다.
1. 사용할 로컬 파일을 선택합니다. 형식은 다음과 일치해야 합니다. [샘플 파일](../../audience/file-audience.md#sample-file).
1. 화면 중앙 섹션에서 데이터가 매핑되는 방식을 미리 보고 확인합니다.
1. 열 설정과 사용 가능한 옵션에서 데이터 서식을 지정하는 방법을 조정합니다.
1. 설정이 적절하면 **확인**&#x200B;을 클릭합니다.

## 예제{#load-example}

외부 파일 로드 샘플은 **조정** 의 활동 [이 섹션](reconciliation.md#example).