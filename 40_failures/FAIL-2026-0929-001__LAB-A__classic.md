# FAIL-2026-0929-001

```
id:        FAIL-2026-0929-001
lab:       LAB-A
channel:   classic
stage:     upload
symptom:   업로드 계획서를 마크다운 파일로 만들어 곡 목록의 순번이 복사되지 않았다.
           뷰어가 1. 을 자동 번호 목록으로 바꿔 보여주기 때문이다. 구역 구분도 눈에 들어오지 않았다.
trigger:   2026-09-29 계획서를 00_upload_plan.md 로 작성했다.
cause:     복사해 붙여넣는 용도의 문서를 마크다운으로 만들었다. 보이는 것과 복사되는 것이 달라진다.
cost:      Philip 검수에서 발견. 재작성 1회.
scope:     tool-wide
status:    closed
closed_by: 2026-09-29 순수 텍스트 파일로 재작성. 줄바꿈은 CRLF
```
