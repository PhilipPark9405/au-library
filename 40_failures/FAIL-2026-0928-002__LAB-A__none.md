# FAIL-2026-0928-002

```
id:        FAIL-2026-0928-002
lab:       LAB-A
channel:   none
stage:     other
symptom:   LAB-A 실행 담당이 작업 폴더를 찾으려고 C:\Dev\유튜브 제작 전체를 검색했고,
           그 결과에 다른 실험실 워크스페이스의 파일 경로가 나왔다. CLAUDE.md 금지 사항이다.
trigger:   앱에서 Claude Code 를 처음 켠 세션에서 PM 이 경로를 지시문에 넣지 않았다.
cause:     PM 지시에 작업 경로가 없었다. 실행 담당은 찾기 위해 상위 폴더를 훑었다.
cost:      경로 이름만 노출. 파일 내용은 열지 않았다.
scope:     tool-wide
status:    closed
closed_by: 2026-09-28 지시문에 경로 네 개를 고정으로 적고 CLAUDE.md 4장에 상위 폴더 검색 금지를 추가
note:      실행 담당이 스스로 위반 사실을 보고했다
```
