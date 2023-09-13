---
audience: end-user
title: 중복 제거 워크플로우 활동 사용
description: 중복 제거 워크플로우 활동을 사용하는 방법 알아보기
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 13%

---


# 중복 제거 {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="포크 활동"
>abstract="중복 제거 활동을 통해 다음을 수행할 수 있습니다."

중복 제거 활동을 통해 인바운드 활동의 결과에서 중복을 삭제할 수 있습니다.

중복 제거 활동은 일반적으로 타겟팅 활동 후 타겟팅된 데이터를 사용할 수 있는 활동 전에 사용됩니다.

## 구성

다음 단계에 따라 **스케줄러** 활동:

1. 추가 **중복 제거** 활동을 워크플로우에 추가합니다.

1. 다음에서 **중복을 식별하는 필드** 섹션에서 **속성 추가** 이메일 주소, 이름, 성 등 동일한 값에서 중복을 식별할 수 있는 필드를 지정하는 버튼입니다. 필드의 순서를 사용하면 먼저 처리할 필드를 지정할 수 있습니다.

1. 고유한 숫자 선택 **유지할 중복 항목**. 이 필드의 기본값은 1입니다. 값 0을 사용하면 모든 중복을 유지할 수 있습니다.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. 다음 항목 선택 **중복 제거 방법** 사용 방법:

   * **무작위 선택**: 중복 중에서 유지할 레코드를 임의로 선택합니다.
   * **표현식 사용**: 입력한 표현식의 값이 가장 작거나 가장 큰 레코드를 유지할 수 있습니다. ++ 표현식 ++ 정렬
   * **값 목록 팔로우**: 하나 이상의 필드에 대한 값 우선 순위를 정의할 수 있습니다. 값을 정의하려면 **속성** 필드를 선택하거나 표현식을 만든 다음 해당 테이블에 값을 추가합니다. 새 필드를 정의하려면 값 목록 위에 있는 추가 버튼을 클릭합니다. ++ 정렬

1. 다음 확인: **보조 항목 생성** 나머지 모집단을 활용하려면 옵션을 선택합니다. 보완은 모든 중복으로 구성됩니다. 그런 다음 추가 전환이 활동에 추가됩니다.
