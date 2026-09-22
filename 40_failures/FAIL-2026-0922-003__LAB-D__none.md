# FAIL-2026-0922-003

```
id:        FAIL-2026-0922-003
lab:       LAB-D
channel:   none
stage:     other
symptom:   LAB-D가 생성하고 안내한 파일명 2건이 naming.md의 "소문자와 하이픈만" 규칙을
           위반했다.
trigger:   reports/_test_kr.md 를 생성했고, 보고서 파일명으로
           2026-0922_lab-d_status.md 를 안내했다. 밑줄을 사용했다.
cause:     파일명 규칙을 확인하지 않고 임시 이름과 밑줄을 그대로 사용했다.
cost:      규칙 위반 파일명 1건 생성. 규칙 위반 안내 1건. 지연 0일.
scope:     tool-wide
status:    open
closed_by:
```
