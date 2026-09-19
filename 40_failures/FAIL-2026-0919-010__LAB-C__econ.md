# FAIL-2026-0919-010

```
id:        FAIL-2026-0919-010
lab:       LAB-C
channel:   econ
stage:     script
symptom:   econ 채널 패키지 제작 중 upload-plan.json의 sources 필드를 채우지 못해 내부 검수를 통과하지 못했다.
trigger:   LAB-C의 검수 에이전트가 20_specs/upload-plan.md의 경제 채널 sources 필수 규칙을 적용해 검사하던 중 확인되었다.
cause:     LAB-C 런타임에서 외부 웹 브라우징이 되지 않아 한국은행과 연준 등의 공식 수치와 출처 URL을 확보하지 못했다. 모르는 값을 unknown으로 둔 원칙은 지켰으나 스키마 필수 조건과 충돌한다.
cost:      출처 데이터가 외부에서 주어지지 않는 한 LAB-C는 econ 채널 패키지를 완성할 수 없다.
note:      브라우징 제약은 econ 채널에 한정된 문제가 아니다. 출처가 필요한 모든 작업에 해당한다. FAIL-002, 006 참조.
scope:     tool-wide
status:    open
closed_by:
```
