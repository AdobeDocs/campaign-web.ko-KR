---
audience: end-user
title: 파일 추출 워크플로우 활동 사용
description: 파일 추출 워크플로우 활동을 사용하는 방법 알아보기
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 7%

---

# 파일 추출 {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="파일 추출"
>abstract="다음 **파일 추출** 활동을 사용하면 Adobe Campaign의 데이터를 외부 파일 형태로 내보낼 수 있습니다. 그런 다음 파일 전송 활동을 사용하여 데이터를 SFTP, 클라우드 스토리지 또는 캠페인 서버와 같은 서버 위치로 내보낼 수 있습니다."

다음 **파일 추출** 활동은 입니다. **데이터 관리** 활동. 이 활동을 사용하여 Adobe Campaign의 데이터를 외부 파일 형태로 내보냅니다. 그런 다음 파일 전송 활동을 사용하여 데이터를 SFTP, 클라우드 스토리지 또는 캠페인 서버와 같은 서버 위치로 내보낼 수 있습니다.

을(를) 구성하려면 다음을 수행하십시오. **파일 추출** 활동, 추가 **파일 추출** 활동을 워크플로우에 포함시킨 다음 아래 단계를 수행합니다.

## 추출할 파일 구성 {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="추출할 파일"
>abstract="추출할 파일을 선택합니다."

다음 **[!UICONTROL 추출할 파일]** 섹션에서 포함할 파일 속성 및 데이터를 구성할 수 있습니다.

![](../assets/extract-file-file.png)

1. 다음에서 **[!UICONTROL 파일 이름]** 필드에 추출할 파일의 이름을 입력합니다.

   이벤트 변수, 조건 및 날짜/시간 함수를 사용하여 파일 이름을 개인화할 수 있습니다. 이렇게 하려면 **[!UICONTROL 개인화 대화 상자 열기]** 아이콘을 클릭하여 표현식 편집기를 엽니다. [이벤트 변수 및 표현식 편집기를 사용하여 작업하는 방법을 알아봅니다](../event-variables.md)

1. 추출된 파일에 표시할 열을 지정합니다. 이렇게 하려면 다음 단계를 수행합니다.

   1. 다음을 클릭합니다. **[!UICONTROL 출력 열 추가]**.
   1. 열에 표시할 속성을 선택한 다음 확인합니다. 사용 가능한 속성은 워크플로우의 타겟팅 차원에 따라 다릅니다.
   1. 열이 추가되면 열을 변경할 수 있습니다 **[!UICONTROL 레이블]** 및 관련 항목 수정 **[!UICONTROL 속성]**.
   1. 열의 값에 변형을 적용하려면 드롭다운 목록에서 변형을 선택합니다. 예를 들어 선택한 열의 모든 값을 대문자로 전환할 수 있습니다.

1. 추출 파일에 필요한 수만큼 열을 추가하려면 이 단계를 반복합니다. 열의 위치를 변경하려면 위쪽 및 아래쪽 화살표를 사용합니다.

1. 추출된 파일에서 모든 중복 행을 제거하려면 **[!UICONTROL 중복 행 제거(나열)]** 옵션을 선택합니다.

1. 속성을 기준으로 추출된 파일을 정렬하려면 **[!UICONTROL 정렬 활성화]** 옵션을 선택한 다음 원하는 정렬 방법(오름차순 또는 내림차순)과 함께 파일을 정렬할 속성을 선택합니다. 파일의 열에 추가되었는지 여부에 관계없이 현재 타겟팅 차원의 모든 속성을 정렬할 수 있습니다.

## 추출된 파일 형식 구성 {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="대상 형식"
>abstract="형식을 선택합니다."

다음 **[!UICONTROL 대상]** 형식 섹션에서 추출된 파일의 형식을 지정할 수 있습니다.

1. 다음을 선택합니다. **[!UICONTROL 출력 형식]** 추출된 파일의 경우: **텍스트**, **열과 함께 고정을 사용하는 텍스트**, **CSV (Excel)** 또는 **XML**.

1. 다음을 클릭합니다. **[!UICONTROL 추출 형식]** 선택한 형식과 관련된 특정 옵션에 액세스하기 위한 단추입니다. 섹션을 아래쪽으로 확장하여 자세한 내용을 봅니다.

+++ 사용 가능한 추출 형식 옵션

   * **[!UICONTROL 첫 번째 줄을 열 머리글로 사용]** (텍스트/CSV(Excel) 형식): 첫 번째 열을 헤더로 사용하려면 이 옵션을 켜거나 끕니다.
   * **[!UICONTROL 열 구분자]** (텍스트 형식): 출력 파일에서 열 구분 기호로 사용할 문자를 지정합니다.
   * **[!UICONTROL 문자열 구분 기호]** (텍스트 형식): 출력 파일에서 문자열을 구분하는 방법을 지정합니다.
   * **[!UICONTROL 라인 끝]** (텍스트 형식): 출력 파일에서 줄 끝을 구분하는 방법을 지정합니다.
   * **[!UICONTROL 인코딩]**: 출력 파일의 인코딩을 선택합니다.
   * **[!UICONTROL 날짜 형식 및 구분 기호]**: 출력 파일에서 날짜 형식을 지정하는 방법을 지정합니다.
   * **[!UICONTROL 숫자 형식]**: 출력 파일에서 숫자의 형식을 지정하는 방법을 지정합니다.
   * **[!UICONTROL 열거형의 내부 값 대신 레이블 내보내기]**: 열거형 값을 내보내고 내부 ID가 아닌 이해하기 쉬운 열 레이블을 검색하려는 경우 이 옵션을 켜거나 끕니다.

+++

   ![](../assets/extract-file-format.png)

## 후 처리 단계 추가 {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="사후 처리"
>abstract="사후 처리 단계 정의"

다음 **[!UICONTROL 수정 스크립트 내보내기]** 를 사용하면 압축 또는 암호화와 같은 데이터 추출 중에 실행할 처리 단계를 적용할 수 있습니다. 이렇게 하려면 **[!UICONTROL 스크립트 편집]** 단추를 클릭합니다.

표현식 편집기가 열리고 파일에 적용할 명령을 입력할 수 있습니다. 왼쪽 창에는 스크립트를 작성하는 데 활용할 수 있는 사전 정의된 구문이 제공됩니다. [이벤트 변수 및 표현식 편집기를 사용하여 작업하는 방법을 알아봅니다](../event-variables.md)

![](../assets/extract-file-script.png)

## 추가 옵션 {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="아웃바운드 전환"
>abstract="**아웃바운드 전환 생성** 옵션을 토글하여 현재 활동 뒤에 아웃바운드 전환을 추가할 수 있습니다."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="오류 처리"
>abstract="**오류 처리** 옵션을 토글하여 오류가 포함된 아웃바운드 전환을 추가할 수 있습니다."

출력 파일 추출이 구성되면 전환 및 오류 관리와 관련된 추가 옵션을 사용할 수 있습니다.

* **[!UICONTROL 아웃바운드 전환 생성]**: 아웃바운드 전환을 추가하고 해당 레이블을 구성하려면 이 옵션을 토글합니다.
* **[!UICONTROL 인바운드 전환이 비어 있는 경우 파일을 생성하지 않음]**: 인바운드 전환에 데이터가 없는 경우 파일 추출을 건너뛰려면 이 옵션을 켜거나 끕니다.
* **[!UICONTROL 프로세스 오류]**: 파일 추출 중에 오류가 발생하는 경우 아웃바운드 전환을 추가하려면 이 옵션을 토글합니다.

## 예제 {#example}

다음 예제에서는 **대상자 작성** 활동 뒤에 다음 **파일 추출** 활동: 모든 타겟팅된 프로필을 CSV 파일로 추출

![](../assets/extract-file-example.png)

* 다음 **[!UICONTROL 파일 이름]** 필드는 추출 날짜를 포함하도록 구성됩니다.

  ![](../assets/extract-file-example-name.png)

* 프로필의 이름과 성, 고객 ID 및 데이터베이스의 작성 날짜를 표시하는 열이 추가됩니다.

  ![](../assets/extract-file-example-columns.png)