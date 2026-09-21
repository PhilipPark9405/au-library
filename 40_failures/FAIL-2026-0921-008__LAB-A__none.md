# FAIL-2026-0921-008

```
id:        FAIL-2026-0921-008
lab:       LAB-A
channel:   none
stage:     other
symptom:   LAB-A 가 "텔레그램 봇은 다른 봇의 메시지를 받지 못한다"고 보고하고, 이를
           랩 간 격리의 근거로 제시했다. 텔레그램은 2026-05-07 Bot-to-Bot
           Communication Mode 를 도입했으며 조건에 따라 봇 간 메시지 수신이 가능하다.
trigger:   자동화 구조 제안 중. 한 차례는 "재확인하겠다"고 적었으나 다음 답변에서
           확정 사실처럼 썼다.
cause:     공식 문서를 확인하지 않고 이전에 알던 규칙을 사용했다.
cost:      격리 근거가 잘못된 상태로 제안되었다. LAB-B 가 지적해 바로잡혔다.
           도서관에는 반영되지 않았다.
scope:     tool-wide
status:    closed
closed_by: ADR-0007 2026-09-21. 실험실 봇을 같은 방에 넣지 않고 Bot-to-Bot 모드를 켜지 않도록 구성으로 격리
```
