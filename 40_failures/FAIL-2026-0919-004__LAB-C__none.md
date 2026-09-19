# FAIL-2026-0919-004

```
id:        FAIL-2026-0919-004
lab:       LAB-C
channel:   none
stage:     기타
symptom:   LAB-C가 구글 드라이브에서 도서관 사본을 찾아 읽고, 이를 도서관의 최신 상태로 보고했다. 읽은 내용은 초판이었고 당시 정본은 4판이었다.
trigger:   Philip이 도서관 초기 파일 묶음을 내려받는 과정에서 드라이브 동기화 폴더에 저장되었다. LAB-C가 GitHub URL을 읽지 못하는 상태에서 드라이브를 대체 경로로 사용했다.
cause:     드라이브 사본은 한 시점의 스냅샷이며 정본과 연결되어 있지 않다. 읽기가 성공하므로 오래된 내용이 최신으로 보고되었다.
cost:      LAB-C가 두 시간 전 도서관 상태를 기준으로 판단하고 있었다. 실제 작업에는 반영되기 전이었다.
scope:     tool-wide
status:    open
closed_by:
```
