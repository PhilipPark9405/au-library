# FAIL-2026-0919-001

```
id:        FAIL-2026-0919-001
lab:       LAB-A
channel:   none
stage:     other
symptom:   커밋 직후 LAB-A가 raw 주소를 조회했을 때 이전 내용이 반환되었다. 같은 시각 GitHub 웹 화면과 Philip의 브라우저에서는 최신 내용이 보였다.
trigger:   INDEX.md와 FACT-003 커밋 직후 LAB-A가 자체 조회 도구로 raw 주소를 열었다.
cause:     unknown. LAB-A 조회 도구의 캐시로 추정되나 확인되지 않았다.
cost:      FACT-004 초안 작성 시간. 도서관에는 반영되지 않았다.
scope:     tool-wide
status:    open
closed_by:
```
