# FAIL-2026-0919-009

```
id:        FAIL-2026-0919-009
lab:       LAB-A
channel:   classic
stage:     other
symptom:   classic 채널의 언어를 수정하면서 10_channels/classic.md만 고치고 INDEX.md의 채널 표는 고치지 않았다. 같은 값이 두 곳에서 서로 다르게 표시되었다.
trigger:   FACT-005 반영 작업에서 LAB-A가 수정 대상 파일을 지정할 때 INDEX를 빠뜨렸다.
cause:     INDEX.md의 채널 표에 언어 열이 있어 채널 문서와 값이 중복된다. 한쪽만 고치면 어긋난다.
cost:      Philip이 발견해 수정했다. 실험실에 배포되기 전이었다.
note:      INDEX는 목록 용도이나 채널 표에 언어 값을 담고 있다. 중복 항목이 다른 표에도 있는지 확인되지 않았다.
scope:     tool-wide
status:    open
closed_by:
```
