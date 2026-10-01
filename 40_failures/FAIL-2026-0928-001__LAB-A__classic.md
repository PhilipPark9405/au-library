# FAIL-2026-0928-001

```
id:        FAIL-2026-0928-001
lab:       LAB-A
channel:   classic
stage:     video
symptom:   롱폼 35분 3초 이후 약 30분 동안 곡 제목과 문구 자막이 나오지 않았다.
trigger:   반복 트랙 네 개에 새 제목을 붙인 뒤 렌더했다.
cause:     새 제목에 해당하는 문구가 설정 파일에 없었다. 조회가 실패했는데 오류를 내지 않고
           조용히 건너뛰었다.
cost:      Philip 검수에서 발견. 재렌더 1회.
scope:     tool-wide
status:    closed
closed_by: 2026-09-28 문구 13개 추가
note:      값이 없을 때 조용히 넘어가는 코드는 화면에서만 드러난다. 설정 조회는 실패 시 중단하게 둔다
```
