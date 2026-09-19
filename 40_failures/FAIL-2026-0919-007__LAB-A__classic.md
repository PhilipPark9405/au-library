# FAIL-2026-0919-007

```
id:        FAIL-2026-0919-007
lab:       LAB-A
channel:   classic
stage:     other
symptom:   LAB-A가 classic 채널을 단일 언어 채널이자 난이도가 가장 낮은 채널로 판단하고 착수 1순위로 정했다. 실제로는 3개국어 채널이며 롱폼 1편에 곡 18개에서 54개가 들어가는 채널이었다.
trigger:   실험실 설계 단계에서 10_channels/classic.md의 언어 항목과 ADR-0002의 배분표를 근거로 채널 난이도를 산정했다.
cause:     10_channels/classic.md의 언어 항목이 영어로만 기재되어 있었다. ADR-0002는 classic 패키지 1건에 다운로드 1회가 든다고 계산했다. 두 값 모두 실제와 달랐다.
cost:      착수 순서를 재산정했다. 실제 제작에는 반영되기 전이었다.
note:      채널 문서와 결정 문서의 값이 실제와 다를 수 있다는 것이 확인되었다. 다른 채널 문서도 검증되지 않았다.
scope:     all-channels
status:    open
closed_by:
```
