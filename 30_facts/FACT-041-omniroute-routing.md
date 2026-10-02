# FACT-041 OmniRoute 를 통한 실행 환경 라우팅

| 항목 | 값 |
|---|---|
| 상태 | 공식 문서와 화면 확인 |
| 확인일 | 2026-10-01 |
| 제출 | LAB-A |
| 영향 | 실행 담당을 쓰는 모든 작업 |

## 사실

- OmniRoute 는 로컬에서 도는 중계 서버다. 기본 포트는 20128 이다.
  실행 담당의 요청을 다른 모델 제공자로 넘긴다.
- 콤보는 먼저 쓸 모델과 실패했을 때 넘길 모델을 순서대로 묶은 설정이다.
- OmniRoute 쪽 문서는 Claude Code Desktop 과 launcher 를 별도 환경으로 설명한다.
- 시작 화면의 Combo 식별자는 Production 세션의 시작 경로만 알려준다. 실제 배차 결과는 별도로 확인해야 한다.
- MCP 로 OmniRoute 를 연결하는 것은 모델을 바꾸는 것이 아니다. 도구를 쓰게 하는 것이다.

## 세션 식별과 배차 판정은 다른 문제다

| 확인 대상 | 수단 | 알 수 있는 것 |
|---|---|---|
| 세션이 Production으로 시작됐는지 | 시작 화면의 Combo 식별자 | 시작 경로만 |
| 실제 요청을 누가 처리했는지 | OmniRoute Logs | Combo, Provider, Model, fallback 여부 |

- 시작 화면의 Combo 식별자는 1차 정보다. 실제 처리 Provider와 Model의 증거가 아니다.
- Claude Desktop의 일반 대화창과 Desktop Code 화면은 claude-production으로 시작했다는 근거가 없는 한 Production 세션으로 보지 않는다.
- `/model`은 Claude Code가 무엇을 요청할지 보여주거나 변경하는 설정이다. OmniRoute 배차 결과를 알려주지 않는다.
- Production 세션에서 사용자가 명시적으로 지시하지 않는 한 `/model`로 모델을 변경하지 않는다.
- 실제 Combo, Provider, Model, fallback은 OmniRoute Logs를 확인한 경우에만 사실로 기록한다.
- 로그를 확인하지 않았으면 "실제 Provider와 Model은 로그 미확인"이라고 적고 추측하지 않는다.

## 확인이 필요한 부분

- 콤보가 다른 모델로 넘어갔을 때 CLAUDE.md 의 금지 사항을 지키는지 확인하지 않았다.
- 긴 작업 도중 모델이 바뀌면 결과가 섞이는지 확인하지 않았다.

## 출처

- OmniRoute 문서와 Anthropic 문서, 2026-10-01
- Philip PC 실행 화면 표시, 2026-10-01
