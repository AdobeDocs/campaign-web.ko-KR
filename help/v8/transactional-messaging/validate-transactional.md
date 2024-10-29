---
audience: end-user
title: 트랜잭션 메시지 확인
description: Campaign 웹 사용자 인터페이스에서 트랜잭션 메시지의 유효성을 검사하는 방법 알아보기
source-git-commit: e0d87d22d9712837f085f94f9d9ba63e96f36b36
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# 트랜잭션 메시지 확인

트랜잭션 메시지를 만드는 동안 또는 만든 후에 데이터 샘플을 사용하여 콘텐츠의 유효성을 검사할 수 있습니다.

## 콘텐츠 시뮬레이션 {#simulate-content}

메시지 콘텐츠를 시뮬레이션하려면 다음 단계를 따르십시오.

* 메시지 콘텐츠의 개인화 경로가 컨텍스트 샘플과 일치하는지 확인합니다. 아래 예제에서는 테스트 프로필의 이름을 표시하기 위해 *rtEvent.ctx.basicDetails.firstName* 경로를 사용합니다.

  메시지 콘텐츠나 컨텍스트 샘플을 변경하여 정렬할 수 있습니다.

  ![](assets/validate-verification.png){zoomable="yes"}

* 컨텍스트 샘플에 입력한 데이터가 포함된 트랜잭션 메시지를 미리 보려면 **[!UICONTROL 콘텐츠 시뮬레이션]** 단추를 클릭하십시오.

  ![](assets/validate-simulate.png){zoomable="yes"}

  콘텐츠를 확인한 후 **[!UICONTROL 닫기]** 단추를 클릭합니다.

* 콘텐츠를 변경한 경우 **[!UICONTROL 다시 게시]** 단추를 클릭하는 것을 잊지 마십시오.

## 교정쇄 보내기

선택한 채널(예: 이메일, SMS 또는 푸시 알림)을 통해 게재되는 트랜잭션 메시지를 테스트하고 경험하려는 경우 증명 기능을 사용할 수 있습니다.

[시뮬레이션 콘텐츠 창](#simulate-content)에서 **[!UICONTROL 증명 보내기]** 단추를 클릭합니다.

![](assets/transactional-proof.png){zoomable="yes"}

표시되는 새 창에서 증명을 받을 이메일 주소(또는 채널에 따라 전화번호)를 입력합니다. 원하는 주소를 입력했으면 **[!UICONTROL 증명 보내기]** 및 **[!UICONTROL 확인]** 단추를 클릭합니다. 이 작업을 통해 트랜잭션 메시지 샘플을 보낼 수 있으므로 모든 개인화, 다이내믹 콘텐츠 및 서식이 최종 사용자의 경우와 마찬가지로 올바르게 표시되도록 할 수 있습니다.

![](assets/transactional-sendproof.png){zoomable="yes"}

이는 트랜잭션 메시지를 게시하기 전에 잠재적인 문제를 식별하는 필수 단계입니다.
