# 파일명과 ID 규칙

## 채널 코드

econ, enka, trot, classic

## 실험실 코드

LAB-A(Claude), LAB-B(ChatGPT), LAB-D(Genspark)
실험실 코드는 위 세 개로 고정한다. 다른 코드를 만들지 않는다.
LAB-C(Gemini)는 2026-09-21 퇴출되었다. ADR-0008 참조. LAB-C 코드는 다시 쓰지 않는다.
퇴출 전 기록의 LAB-C 표기와 파일명은 그대로 둔다.

## ID 형식

| 대상 | 형식 | 예 |
|---|---|---|
| 패키지 | `PKG-YYYY-MMDD-{channel}-{NN}` | PKG-2026-0919-econ-01 |
| 계획서 | `PLAN-YYYY-MMDD-{channel}-{NN}` | PLAN-2026-0919-enka-02 |
| 실패 기록 | `FAIL-YYYY-MMDD-{NNN}` | FAIL-2026-0919-001 |
| 사실 기록 | `FACT-{NNN}-{slug}` | FACT-001-suno-download-cap |

## 파일명

- 소문자와 하이픈만 쓴다. 공백과 한글은 파일명에 넣지 않는다.
- 실패 기록 파일명은 `FAIL-2026-0919-001__LAB-A__enka.md` 형태로 실험실과 채널을 붙인다.

## 번호

같은 날짜 안에서 001부터 순서대로. 번호를 재사용하지 않는다.

실험실은 FACT와 FAIL의 번호를 붙이지 않는다.
제출할 때는 주제만 적고, 번호는 커밋하면서 Philip이 부여한다.
커밋되지 않은 초안의 번호는 사용된 것으로 보지 않는다.
