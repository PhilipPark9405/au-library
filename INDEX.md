# INDEX

이 파일 하나만 읽으면 도서관에 무엇이 있는지 전부 알 수 있습니다.
파일이 추가되거나 삭제되면 여기도 같이 고칩니다.

최종 갱신: 2026-09-19 (9판)

## 00 헌장

| 파일 | 내용 |
|---|---|
| `00_CHARTER.md` | 목적, 절대 규칙, 실험실 목록, 개정 절차 |

## 10 채널

| 파일 | 채널 | 언어 |
|---|---|---|
| `10_channels/econ.md` | 경제의 촉 | 한국어 |
| `10_channels/enka.md` | 演歌魂 EnkaKing | 일본어 |
| `10_channels/trot.md` | 트로트 인생 멜로디 | 한국어 |
| `10_channels/classic.md` | Moonlight Classic | 영어, 한국어, 일본어 |
| `10_channels/_banned.md` | 전 채널 공통 금지어와 금지 표현 |

## 20 규격

| 파일 | 내용 |
|---|---|
| `20_specs/package-contract.md` | 영상 패키지 1건의 완료 조건 |
| `20_specs/upload-plan.md` | 업로드 계획서 스키마 |
| `20_specs/naming.md` | 파일명과 ID 규칙 |

## 30 검증된 사실

| 파일 | 내용 | 상태 |
|---|---|---|
| `30_facts/FACT-001-suno-download-cap.md` | Suno 다운로드 한도 | 검증됨 |
| `30_facts/FACT-002-youtube-skills-scope.md` | youtube-skills의 기능 범위와 크레딧 | 검증됨 |
| `30_facts/FACT-003-youtube-api-upload-quota.md` | YouTube API 업로드 할당 | 검증됨 |
| `30_facts/FACT-004-classic-audio-volume.md` | Moonlight Classic 롱폼의 음원 소요량 | 검증됨 |
| `30_facts/FACT-005-classic-multilingual.md` | Moonlight Classic의 언어 구성 | 검증됨 |
| `30_facts/FACT-006-song-selection-time.md` | 곡 선별에 드는 사람 시간 | 검증됨 |

## 40 실패 기록

| 파일 | 내용 |
|---|---|
| `40_failures/_TEMPLATE.md` | 제출 양식 |
| `40_failures/FAIL-2026-0919-001__LAB-A__none.md` | raw 주소 조회 시 이전 내용 반환 |
| `40_failures/FAIL-2026-0919-002__LAB-C__none.md` | LAB-C가 커밋 API를 열지 못함 |
| `40_failures/FAIL-2026-0919-003__LAB-C__none.md` | LAB-C가 읽지 못한 값과 원인을 단정함 |
| `40_failures/FAIL-2026-0919-004__LAB-C__none.md` | 드라이브 사본을 최신으로 오인함 |
| `40_failures/FAIL-2026-0919-005__LAB-A__none.md` | LAB-A가 저장소 갱신을 조회하지 못함 |
| `40_failures/FAIL-2026-0919-006__LAB-C__none.md` | LAB-C가 새 세션에서도 raw 주소를 열지 못함 |
| `40_failures/FAIL-2026-0919-007__LAB-A__classic.md` | classic 채널 난이도를 잘못 산정함 |
| `40_failures/FAIL-2026-0919-008__LAB-A__none.md` | 사실 기록 번호를 건너뛰어 제출함 |
| `40_failures/FAIL-2026-0919-009__LAB-A__classic.md` | INDEX와 채널 문서의 값이 어긋남 |

## 50 성과

| 파일 | 내용 |
|---|---|
| `50_metrics/_TEMPLATE.md` | 주간 제출 양식 |

기록 없음.

## 60 결정

| 파일 | 내용 |
|---|---|
| `60_decisions/ADR-0001-builder-and-repo.md` | 구축 담당과 저장소 형태 |
| `60_decisions/ADR-0002-music-source-policy.md` | 음원 조달 정책, 채널별 배분 |
| `60_decisions/ADR-0003-change-detection.md` | 도서관 변경 감지 방식 |
| `60_decisions/ADR-0004-lab-autonomy.md` | 실험실의 자율 범위 |
