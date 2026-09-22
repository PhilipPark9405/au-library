# FAIL-2026-0919-005

```
id:        FAIL-2026-0919-005
lab:       LAB-A
channel:   none
stage:     other
symptom:   LAB-A가 raw 주소를 반복 조회했으나 계속 초판 내용만 반환되었다. 2판부터 5판까지 모든 갱신을 확인하지 못했다. 같은 시각 Philip 브라우저에서는 최신 내용이 정상 표시되었다.
trigger:   도서관 갱신 후 LAB-A가 자체 조회 도구로 검증을 시도할 때마다 발생했다. 하루 동안 다섯 차례 반복되었다.
cause:     unknown. LAB-A 조회 도구의 캐시로 추정되나 확인되지 않았다.
cost:      LAB-A가 커밋 결과를 검증하지 못한다. 검증은 Philip이 직접 화면으로 수행하고 있다.
scope:     tool-wide
status:    open
closed_by:
```
