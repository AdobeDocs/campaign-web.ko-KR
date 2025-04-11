---
audience: end-user
title: 트랜잭션 메시지
description: Adobe Campaign 웹을 사용한 트랜잭션 메시지 기본 정보
exl-id: 90830dca-acff-4aa3-a88b-1005e349cf52
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 13%

---

# 트랜잭션 메시지 정보 {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="트랜잭션 메시지"
>abstract="트랜잭션 메시지는 트리거 메시지 처리를 위해 설계된 Adobe Campaign의 특수 모듈입니다."

<!-- >>[!CONTEXTUALHELP]
>id="acw_transacmessages_exclusionlogs"
>title="Transactional messaging exclusion logs"
>abstract="Transactional messaging exclusion logs" -->

트랜잭션 메시지는 트리거 메시지 처리를 위해 설계된 Adobe Campaign의 특수 모듈입니다. 이러한 메시지는 정보 시스템에서 발생하는 이벤트에 대한 응답으로 자동으로 생성됩니다. 이러한 이벤트의 일반적인 예로는 버튼 또는 링크 클릭, 장바구니 포기, 제품 가용성 경고 요청, 계정 생성 또는 수정이 있습니다.

트랜잭션 메시지는 다음을 전송하는 데 사용됩니다.

* 주문 확인 또는 암호 재설정 등 중요한 알림
* 계정 생성 또는 구매 완료와 같은 고객 작업에 대한 실시간 응답
* 고객 상호 작용에 중요한 홍보용 콘텐츠가 아닌 콘텐츠.

트랜잭션 메시지 모듈은 정보 시스템과 완벽하게 통합됩니다. 고객 작업과 같은 이벤트는 Adobe Campaign에 푸시되어 해당 개인화된 메시지를 전송합니다. 이러한 메시지는 이메일, SMS 또는 푸시 알림과 같은 다양한 채널을 통해 개별적으로 또는 일괄적으로 전송할 수 있습니다.

**[!UICONTROL 트리거된 메시지]** 섹션에서 **[!UICONTROL 트랜잭션 메시지]** 모듈을 찾을 수 있습니다.

![트리거된 메시지와 해당 상태를 표시하는 트랜잭션 메시지 인터페이스](assets/transactional.png){zoomable="yes"}

**[!UICONTROL 트랜잭션 메시지]** 페이지에 세 개의 탭이 있습니다.

* **[!UICONTROL 찾아보기]**, 상태의 트랜잭션 메시지 목록이 있는 경우,
* 트랜잭션 메시지 템플릿을 찾아 만드는 **[!UICONTROL 템플릿]**,
* **[!UICONTROL 내역]**. 여기서 실행된 모든 트랜잭션 메시지에 대한 세부 정보가 있습니다.

다음 방법을 알아보려면 이 설명서를 참조하십시오.

* 템플릿을 사용하여 [트랜잭션 메시지를 만들고](create-transactional.md) 필요한 설정을 알아봅니다.
* [트랜잭션 메시지의 내용을 확인하고](validate-transactional.md) 개인화를 시뮬레이션하고,
* [트랜잭션 메시지 모니터링](monitor-transactional.md).