# FACT-024 classic v1.6.1 숏폼 렌더 사양

| 항목 | 값 |
|---|---|
| 상태 | 원문 코드로 확인 |
| 확인일 | 2026-09-21 |
| 제출 | LAB-A |
| 영향 채널 | classic |

## 사실

render_shorts_v161.py 기준이다.

3시간 롱폼에서 구간을 잘라 중앙 크롭 후 확대한다. 별도 9:16 제작이 아니다.

| 항목 | short_A | short_B |
|---|---|---|
| 시작 | 120초 | 5,520초 |
| 길이 | 30초 | 32초 |

처리는 crop=608:1080 중앙 크롭 후 scale=1080:1920 이다. 가로로 약 1.78배 확대된다.

인코딩은 libx264, preset veryfast, CRF 20, 오디오 AAC 256kbps 다.

## 설정과 코드 불일치

config/episode.json 에는 short_B 시작이 2,700초로 되어 있다. 코드는 5,520초다.
코드가 설정 파일을 읽지 않고 값을 직접 들고 있다.

episode.json 에는 훅 문구도 들어 있다.

- short_A: Why does cello feel deeper after midnight?
- short_B: A quiet phrase for the page you cannot finish.

렌더 코드에 텍스트 레이어가 없어 화면에는 나오지 않는다.

## 확인이 필요한 부분

- 시작 지점 120초와 5,520초의 선정 근거. 장면 선별 기록이 없다.

## 출처

- scripts/render_shorts_v161.py 원문, 2026-09-21
- config/episode.json 원문, 2026-09-21
