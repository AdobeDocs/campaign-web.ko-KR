---
audience: end-user
title: 게재 로그 모니터링
description: 게재 로그 모니터링 방법 알아보기
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 55%

---

# 게재 로그 모니터링 {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="게재 로그"
>abstract="게재 로그에는 전송 세부 정보가 표시됩니다. 여기에는 전송 세부 정보와 제외된 대상 및 그 이유와 함께 열람 및 클릭 등의 추적 정보가 표시됩니다."

게재가 준비되고 **보내기** 단추를 클릭하면 게재 로그를 찾아 경고, 오류, 상태, 제외 및 추적 데이터를 확인합니다. 메시지 대시보드에서 로그에 직접 액세스할 수 있습니다. 여기에는 전송 세부 정보와 제외된 대상 및 그 이유와 함께 열람 및 클릭 등의 추적 정보가 표시됩니다.

로그를 보려면 게재 대시보드에 액세스하고 **로그** 버튼을 클릭합니다.

다음 탭을 사용할 수 있습니다.

* [로그](#logs-tab)
* [게재](#deliveries-tab)
* [제외](#exclusion-tab)
* [제외 원인](#exclusion-causes)
* [추적된 URL](#tracked-urls)
* [추적](#tracking)

## 로그 {#logs-tab}

**로그** 탭에는 게재 및 교정쇄와 관련된 모든 메시지가 포함되어 있습니다. 특정 아이콘을 통해 오류나 경고를 확인할 수 있습니다.

모든 유효성 검사 단계, 경고 및 오류가 나열됩니다. 색상이 지정된 아이콘은 메시지 유형을 나타냅니다.

* 회색 아이콘은 유익한 메시지를 나타냅니다.
* 노란색 아이콘은 중요하지 않은 처리 오류를 나타냅니다.
* 빨간색 아이콘은 게재를 보낼 수 없는 심각한 오류를 나타냅니다. 게재를 보내려면 중대 오류를 수정해야 합니다.

![&#x200B; 유효성 검사 단계, 경고 및 오류를 표시하는 로그 탭과 메시지 유형을 나타내는 컬러 아이콘](assets/logs.png){zoomable="yes"}

## 게재 {#deliveries-tab}

**전송 로그** 탭에는 이 게재의 모든 발생 내역이 표시됩니다. 보낸 메시지 및 상태 목록이 여기에 저장됩니다. 여기에서 각 수신자에 대한 게재 상태를 볼 수 있습니다.

보낸 메시지의 기록 및 상태를 표시하는 ![&#x200B; 게재 탭.](assets/logs2.png){zoomable="yes"}

## 제외 {#exclusion-tab}

**제외 로그** 탭에는 대상에서 제외된 모든 메시지가 나열되며, 전송 실패 이유가 함께 제공됩니다.

![제외된 메시지 및 전송 실패 이유를 나열하는 제외 탭](assets/logs3.png){zoomable="yes"}

## 제외 원인 {#exclusion-causes-tab}

**제외 원인** 탭에는 가능한 각 원인에 대해 대상에서 제외된 메시지 수가 표시됩니다.

![제외 원인 탭에서 각 원인에 대해 제외된 메시지 수를 표시합니다.](assets/logs4.png){zoomable="yes"}

## 추적된 URL {#tracked-urls-tab}

**추적된 URL** 탭은 보낸 메시지의 URL 유형 및 소스 URL을 포함하여 보낸 메시지에 포함된 URL을 다시 그룹화합니다.

![보낸 메시지에 포함된 URL, 해당 형식 및 원본 URL을 표시하는 추적된 URL 탭입니다.](assets/logs5.png){zoomable="yes"}

## 추적 {#tracking-tab}

**추적** 탭에는 이 게재에 대한 추적 기록이 나열됩니다. 이 탭에는 Adobe Campaign의 추적 대상이 되는 모든 URL을 포함하여 전송된 메시지에 대한 추적 데이터가 표시됩니다.

![보낸 메시지의 추적 기록 및 데이터를 표시하는 추적 탭입니다.](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>게재에 대해 추적이 활성화되어 있지 않은 경우 이 탭이 표시되지 않습니다.