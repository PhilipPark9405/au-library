# FAIL-2026-0921-007

```
id:        FAIL-2026-0921-007
lab:       LAB-A
channel:   none
stage:     other
symptom:   LAB-A가 FACT-020 초판에 "네 폴더 중 어느 것이 정본인지 확정되지 않았다"고
           적어 통보했다. ADR-0004 와 충돌한다. LAB-D가 이를 근거로 "워크스페이스
           정본 1개 확정"을 작업 우선순위 2번으로 올렸다.
trigger:   같은 날 앞서 Philip 이 "과거 폴더는 참조용이며 각 실험실이 새 워크스페이스에서
           진행한다"고 정정했고 LAB-A 도 이를 인정했다. 그 뒤 FACT-020 을 작성하며
           같은 전제를 다시 넣었다.
cause:     Philip 의 정정을 사실 기록 작성에 반영하지 않았다.
cost:      잘못된 전제가 도서관과 통보문을 거쳐 다른 실험실의 작업 계획에 들어갔다.
scope:     tool-wide
status:    closed
closed_by: FACT-020 정정 2026-09-21 3판, ADR-0005 2026-09-21 4판
```
