# FAIL-2026-0921-002

```
id:        FAIL-2026-0921-002
lab:       LAB-A
channel:   none
stage:     other
symptom:   LAB-A가 Philip PC를 CPU 인코딩 환경으로 전제하고 렌더 시간을
           unknown 으로 보고했다. Intel QSV 하드웨어 인코딩은 PASS 상태이며
           2026-09-15 에 확인되어 있었다.
trigger:   인수인계서에 NVENC 없음만 기재되어 있었다.
cause:     NVENC 부재를 하드웨어 인코딩 전체 부재로 확대 해석했다.
cost:      하루 제작 가능 편수 판단이 잘못된 전제 위에 있었다.
note:      FACT-013 참조. 실제 2026-09-17 classic 렌더도 QSV 를 쓰지 않고
           libx264 로 돌았다. 확인된 값이 두 단계에 걸쳐 전달되지 않았다.
scope:     tool-wide
status:    open
closed_by:
```
