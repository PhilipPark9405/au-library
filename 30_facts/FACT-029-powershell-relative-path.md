# FACT-029 PowerShell 5.1의 상대 경로 해석

| 항목 | 값 |
|---|---|
| 상태 | 명령 출력으로 확인 |
| 확인일 | 2026-09-22 |
| 제출 | LAB-D |
| 영향 | Windows PowerShell 5.1 환경 |

## 사실

- cd 로 PowerShell 공급자 위치를 바꾸어도 프로세스 작업 디렉터리는 바뀌지 않는다.
- 같은 시점 실측값. $PWD.ProviderPath 는
  C:\Dev\유튜브 제작\LAB-D-Youtube-DeepSeek-Workspace 였고,
  [Environment]::CurrentDirectory 는 C:\Users\jihwa 였다.
- .NET 정적 메서드는 상대 경로를 프로세스 작업 디렉터리 기준으로 해석한다.
  [System.IO.File], [System.IO.Directory] 가 해당한다.
- PowerShell cmdlet 은 PowerShell 위치 기준으로 해석한다.
  Test-Path, Get-Content 가 해당한다.
- 같은 시점에 [System.IO.File]::Exists("C:\Users\jihwa\scripts\send_lab_d_report.ps1") 는
  False 였다.
- 실행 환경은 Windows PowerShell 5.1.26100.9444 였다.

## 확인이 필요한 부분

- PowerShell 7 이상에서 같은지 확인하지 않았다.
- 같은 조건에서 다른 .NET API 가 쓰는 기준 디렉터리는 확인하지 않았다.

## 출처

- Philip PC 명령 출력, 2026-09-22
