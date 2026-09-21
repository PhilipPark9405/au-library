# FAIL-2026-0921-004

```
id:        FAIL-2026-0921-004
lab:       LAB-A
channel:   classic
stage:     other
symptom:   FACT-004 초판이 3시간 롱폼에 곡 54개, 다운로드 54회, 생성 27회가
           필요하다고 산정했다. 실제 제작 방식은 14곡 한 세트를 3패스로
           반복하는 것이며 다운로드는 14회다. 소요량이 실제의 약 4배로 기록되었다.
trigger:   2026-09-19 FACT-004 작성 시 실제 제작 코드를 확인하지 않았다.
cause:     롱폼 길이를 곡당 평균 길이로 나누는 방식으로 산정했다.
           반복 구성 가능성을 고려하지 않았다.
cost:      ADR-0002 의 Suno 배분과 Premier 전환 검토가 부풀려진 수치 위에서
           이루어졌다.
note:      build_audio.py 는 2026-09-16 이전부터 존재했다.
           FACT-004 작성 시점에 확인 가능한 자료였다. FACT-025 참조.
scope:     lab-only
status:    closed
closed_by: FACT-025
```
