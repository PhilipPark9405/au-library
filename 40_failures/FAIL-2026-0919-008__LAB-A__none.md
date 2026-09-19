# FAIL-2026-0919-008

```
id:        FAIL-2026-0919-008
lab:       LAB-A
channel:   none
stage:     other
symptom:   LAB-A가 사실 기록을 FACT-005로 제출했다. 도서관의 마지막 번호는 FACT-003이었다. 004를 건너뛴 상태로 제출했다.
trigger:   LAB-A가 당일 오전 작성했다가 취소한 FACT-004 초안의 번호를 소진된 것으로 간주했다.
cause:     커밋되지 않은 초안의 번호를 사용된 번호로 취급했다. 개정 전 20_specs/naming.md는 번호 재사용을 금지했으나 미사용 번호 건너뛰기를 규정하지 않았다.
cost:      제출물 파일명 수정. 커밋 전에 발견되어 도서관에는 반영되지 않았다.
note:      같은 시각 LAB-D도 FACT-004를 제출했다. 실험실이 각자 번호를 부여하는 구조에서 충돌이 발생한다. naming.md를 개정해 번호 부여 주체를 Philip으로 정했다.
scope:     tool-wide
status:    closed
closed_by: 20_specs/naming.md 개정, 2026-09-19
```
