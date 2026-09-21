# FACT-027 econ 채널 음성 설정

| 항목 | 값 |
|---|---|
| 상태 | 설정 파일 생성 기록으로 확인. 실물 미확인 |
| 확인일 | 2026-09-21 |
| 제출 | LAB-A |
| 영향 채널 | econ |

## 사실

| 항목 | 값 |
|---|---|
| 엔진 | Supertonic TTS |
| 음색 | M1 |
| 속도 | 1.02 |
| total_steps | 12 |
| sample_rate | 44,100 |
| 언어 | ko |
| 상태 | LOCKED |

M1 부터 M5 까지 청취 비교에서 M1이 1위, M2가 2위였다. 속도는 B안이 채택되었다.

설정 파일 경로다.

```
config/voices/economyuichok.json
config/pronunciation/economyuichok.json
```

발음 사전에 등재된 항목이다.

10년물, 5%, FOMC, KOSPI, NASDAQ, S&P500, SK하이닉스, AI, HBM, PER

## 렌더

econ 은 Remotion 으로 렌더한다. 확인된 명령은 다음과 같다.

```
remotion render src\index.ts EconomyUichok <출력경로> --codec=h264 --crf=16
```

classic 은 CRF 21, econ 은 CRF 16 이다. 채널별로 다르며 기준이 문서화되어 있지 않다.

## 확인이 필요한 부분

- 설정 파일 실물. 생성 명령만 확인했다.
- 대본 글자 수 대비 음성 길이 환산값. 이 값이 있어야 롱폼 길이를 대본 단계에서 예측할 수 있다. FACT-007 참조.

## 출처

- 경제의촉-1.docx 4497~4760행, 5720행
