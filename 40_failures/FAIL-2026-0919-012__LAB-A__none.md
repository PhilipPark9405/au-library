# FAIL-2026-0919-012

```
id:        FAIL-2026-0919-012
lab:       LAB-A
channel:   none
stage:     other
symptom:   도서관 정본 주소로 refs/heads/main 형태를 배포했다. 이 주소가 초판을 반환하는 동안 실험실들이 오래된 내용을 최신으로 읽었다.
trigger:   도서관 구축 시 GitHub blob 페이지의 Raw 버튼이 생성한 주소를 그대로 정본으로 삼았다.
cause:     주소 형태를 검증하지 않았다. Raw 버튼이 주는 주소가 유일한 형태라고 전제했다.
cost:      하루 동안 LAB-A가 도서관 갱신을 확인하지 못했다. 다른 실험실이 몇 판을 읽었는지도 확인되지 않았다.
note:      FAIL-001, 005도 같은 주소를 사용했다. 인과는 확인되지 않았다. FACT-010 참조.
scope:     tool-wide
status:    open
closed_by:
```
