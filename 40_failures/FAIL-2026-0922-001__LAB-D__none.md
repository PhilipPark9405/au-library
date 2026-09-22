# FAIL-2026-0922-001

```
id:        FAIL-2026-0922-001
lab:       LAB-D
channel:   none
stage:     other
symptom:   스크립트가 .env를 읽지 못하고 "token missing"을 출력했다. .env와 토큰은 정상이었다.
trigger:   C:\Dev\유튜브 제작\LAB-D-Youtube-DeepSeek-Workspace 에서 cd 한 뒤
           .\scripts\send_lab_d_report.ps1 를 실행했다. 스크립트는
           [System.IO.File]::ReadAllLines(".\.env", [System.Text.Encoding]::UTF8) 로
           상대 경로를 읽었다.
cause:     PowerShell 위치와 프로세스 작업 디렉터리가 달랐다. 위치는
           C:\Dev\유튜브 제작\LAB-D-Youtube-DeepSeek-Workspace 였고, 프로세스 작업
           디렉터리는 C:\Users\jihwa 였다. .NET 정적 메서드는 상대 경로를 프로세스
           작업 디렉터리 기준으로 해석했다.
cost:      송신 실패 1회. 진단 왕복 2회. 지연 0일.
scope:     tool-wide
status:    closed
closed_by: 2026-09-22. 스크립트 진입에서 [Environment]::CurrentDirectory 를 워크스페이스로
           고정한 뒤 송신에 성공했다. reports/send_log.jsonl 에 ok=true 2건이 기록되었다.
```
