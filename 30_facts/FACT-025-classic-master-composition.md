# FACT-025 classic 오디오 마스터 구성 방식

| 항목 | 값 |
|---|---|
| 상태 | 원문 코드와 설정 파일로 확인 |
| 확인일 | 2026-09-21 |
| 제출 | LAB-A |
| 영향 채널 | classic |

## 사실

build_audio.py 는 목표 길이에 닿을 때까지 같은 곡 묶음을 반복한다.

반복 순서는 3패스 고정이다.

| 패스 | 순서 |
|---|---|
| 1 | 원래 순서 |
| 2 | 홀수 번째, 그다음 짝수 번째 |
| 3 | 짝수 역순, 그다음 홀수 역순 |

곡 사이는 크로스페이드로 잇는다. 전체에 페이드인 2.5초, 페이드아웃 7초를 적용한다.
random 을 import 하지만 사용하지 않는다. 같은 입력이면 항상 같은 결과가 나온다.

마스터가 하나라도 없으면 FileNotFoundError 로 중단한다.

## MC-UL-001 설정값

| 항목 | 값 |
|---|---|
| project_id | MC-UL-001 |
| working_title | Rainy Library After Midnight |
| target_runtime_seconds | 10,800 |
| track_count | 14 |
| download_format | wav |
| crossfade_ms | 2,500 |
| privacy_status | private |
| contains_synthetic_media | true |

곡 세트는 MC001-T01 부터 MC001-T14 까지 14곡이다. 전부 instrumental 이며
첼로와 피아노 중심, 54~64 BPM 구간이다. 프롬프트에 fully original 표기가 들어 있다.

## 확인이 필요한 부분

- 곡당 평균 길이 실측값.
- 에피소드마다 곡 세트를 새로 만드는지, 기존 세트를 재사용하는지.
- 같은 곡을 3회 반복한 롱폼이 유튜브 반복 콘텐츠 정책에 저촉되는지.

## 출처

- scripts/build_audio.py 원문, 2026-09-21
- config/episode.json, config/tracks.json 원문, 2026-09-21
