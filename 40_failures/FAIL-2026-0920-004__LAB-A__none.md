# FAIL-2026-0920-004

```
id:        FAIL-2026-0920-004
lab:       LAB-A
channel:   none
stage:     other
symptom:   날짜가 2026-09-20으로 바뀐 뒤에도 LAB-A가 모든 신규 기록에 2026-09-19를 적었다. 실패 기록 파일명과 id, 사실 기록의 확인일이 전부 어제 날짜였다.
trigger:   전날 시작한 작업을 이어서 진행하는 과정에서 발생했다.
cause:     작업 시작 시 현재 날짜를 확인하지 않고 직전 작업의 날짜를 이어 썼다.
cost:      파일명과 id, 확인일 수정. Philip이 발견해 커밋 전에 바로잡았다.
note:      20_specs/naming.md는 같은 날짜 안에서 번호를 001부터 매기도록 규정한다. 날짜를 잘못 쓰면 번호 체계도 어긋난다.
scope:     tool-wide
status:    open
closed_by:
```
