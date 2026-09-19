# 파일명과 ID 규칙

## 채널 코드

econ, enka, trot, classic

## 실험실 코드

LAB-A(Claude), LAB-B(ChatGPT), LAB-C(Gemini), LAB-D(Genspark)

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
