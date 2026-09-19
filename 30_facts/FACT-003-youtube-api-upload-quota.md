# FACT-003 YouTube Data API 업로드 할당

| 항목 | 값 |
|---|---|
| 상태 | 검증됨. 계정 실측값 미확인 |
| 확인일 | 2026-09-19 |
| 제출 | LAB-D |
| 영향 채널 | econ, enka, trot, classic |

## 사실

- YouTube Data API v3의 할당은 Google Cloud 프로젝트 단위로 부여된다. 계정 단위가 아니다.
- 같은 프로젝트 안의 API 키가 여러 개여도 할당은 하나를 나눠 쓴다.
- 기본 할당은 세 갈래로 나뉜다.
  - search.list 하루 100회
  - videos.insert 하루 100회
  - 나머지 엔드포인트 전체 합산 하루 10,000 units
- 할당은 태평양 시간 자정에 초기화된다.
- 잘못된 요청도 최소 1 unit을 소모한다.
- 기본 할당을 넘기려면 감사 절차를 거쳐 증설을 신청해야 한다.

## 산술

패키지 1건은 롱폼 1편과 숏폼 2편으로 영상 3건이다.
채널 4개에 패키지 1건씩이면 하루 12건이다.

videos.insert 하루 100회 기준으로 여유는 88건이다. 현재 계획에서 업로드 할당은 병목이 아니다.

## 정정 이력

최초 제출본은 10,000 units를 1,600 units로 나눈 하루 6건을 상한으로 계산했다.
videos.insert가 units 풀에서 분리되어 별도 100회 할당을 받는 현행 구조를 반영하지 못한 계산이다.
채널별 GCP 프로젝트 분리는 현재 계획 규모에서 필요하지 않다.

## 확인이 필요한 부분

- 업로드를 API로 자동화하지 않고 YouTube Studio 화면에서 수동으로 하는 경우, 이 할당은 적용되지 않는다.
  Studio 수동 업로드에는 별도의 일일 개수 제한이 있으며 채널 인증 여부에 따라 달라진다. 실측 확인이 필요하다.
- 실제 자동 업로드를 도입할 때 GCP 프로젝트의 할당 화면에서 현재 값을 확인해야 한다.

## 출처

- YouTube Data API Overview, Google for Developers (developers.google.com/youtube/v3/getting-started)
- Quota and Compliance Audits, Google for Developers (developers.google.com/youtube/v3/guides/quota_and_compliance_audits)
