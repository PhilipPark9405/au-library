# INDEX

이 파일 하나만 읽으면 도서관에 무엇이 있는지 전부 알 수 있습니다.
파일이 추가되거나 삭제되면 여기도 같이 고칩니다.

최종 갱신: 2026-09-24 (2판)

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
| `10_channels/_banned.md` | 전 채널 공통 금지어와 금지 표현 | |

## 20 규격

| 파일 | 내용 |
|---|---|
| `20_specs/package-contract.md` | 영상 패키지 1건의 완료 조건 |
| `20_specs/upload-plan.md` | 업로드 계획서 스키마 |
| `20_specs/naming.md` | 파일명과 ID 규칙 |
| `20_specs/response-rules.md` | 답변 15원칙. 06 범위와 09 적용, 충돌 시 순서 |

## 30 검증된 사실

| 파일 | 내용 | 상태 |
|---|---|---|
| `30_facts/FACT-001-suno-download-cap.md` | Suno 다운로드 한도 | 검증됨. 계정 실측값 미확인 |
| `30_facts/FACT-002-youtube-skills-scope.md` | youtube-skills의 기능 범위와 크레딧 | 검증됨 |
| `30_facts/FACT-003-youtube-api-upload-quota.md` | YouTube API 업로드 할당 | 검증됨. 계정 실측값 미확인 |
| `30_facts/FACT-004-classic-audio-volume.md` | Moonlight Classic 롱폼의 음원 소요량 | 09-21 재정정. 세트 14곡, 실제 다운로드 18곡 |
| `30_facts/FACT-005-classic-multilingual.md` | Moonlight Classic의 언어 구성 | 검증됨 |
| `30_facts/FACT-006-song-selection-time.md` | 곡 선별에 드는 사람 시간 | 확인됨. 실측 미완료 |
| `30_facts/FACT-007-econ-longform-length.md` | 경제의 촉 롱폼 길이 기준 | 2026-09-21 정정. 근거 미보강 |
| `30_facts/FACT-008-competitor-apps.md` | 경쟁 앱 두 종의 제품 구조 | 화면과 판매사 답변 기준. 실사용 미검증 |
| `30_facts/FACT-009-channel-personas.md` | enka와 trot 채널의 가수 설정 | Philip 확정 |
| `30_facts/FACT-010-library-url-form.md` | 도서관 조회 주소의 형태별 차이 | 09-21 정정. 주소로 정본 지정 안 함 |
| `30_facts/FACT-011-lab-c-url-access.md` | LAB-C의 URL 조회 불가 | 4회 시도로 확인 |
| `30_facts/FACT-012-lab-c-notebook-source.md` | LAB-C의 노트북 소스 경로 | 확인됨 |
| `30_facts/FACT-013-hardware-encoding.md` | Philip PC의 하드웨어 인코딩 지원 범위 | 명령 출력으로 확인 |
| `30_facts/FACT-014-toolchain-versions.md` | 제작 환경 도구 버전 | 명령 출력으로 확인. 09-15 시점 |
| `30_facts/FACT-015-classic-render-time.md` | classic 3시간 롱폼 렌더 실측 소요 시간 | 파일 타임스탬프로 산출 |
| `30_facts/FACT-016-remotion-license.md` | Remotion 라이선스 조건 | 당시 확인 기록. 재확인 미실시 |
| `30_facts/FACT-017-quality-baseline.md` | 제작 품질 기준선 | ffprobe 실측 |
| `30_facts/FACT-018-shorts-bitrate-gap.md` | 숏폼 비트레이트 격차 | 실측과 검수 기록 대조 |
| `30_facts/FACT-019-output-assets.md` | 산출물 폴더의 보유 자산 | 파일 목록으로 확인. 일부 미확인 |
| `30_facts/FACT-020-workspace-inventory.md` | C:\Dev 의 과거 유튜브 제작 폴더. 참고 자료 | 파일 목록으로 확인. 09-21 정정 |
| `30_facts/FACT-021-local-library-copy.md` | 로컬 도서관 사본 | 확인됨. 09-21 처리 완료 |
| `30_facts/FACT-022-repo-push-condition.md` | 도서관 저장소 푸시 조건 | 푸시 실패와 성공으로 확인 |
| `30_facts/FACT-023-classic-longform-render-spec.md` | classic v1.6.1 롱폼 렌더 사양 | 원문 코드로 확인 |
| `30_facts/FACT-024-classic-shorts-render-spec.md` | classic v1.6.1 숏폼 렌더 사양 | 원문 코드로 확인 |
| `30_facts/FACT-025-classic-master-composition.md` | classic 오디오 마스터 구성 방식 | 원문 코드와 설정으로 확인 |
| `30_facts/FACT-026-review-implementation-gap.md` | 09-16 classic 검수 지적의 반영 현황 | 검수 기록과 코드 대조 |
| `30_facts/FACT-027-econ-voice-config.md` | econ 채널 음성 설정 | 생성 기록으로 확인. 실물 미확인 |
| `30_facts/FACT-028-ypp-status.md` | 채널별 파트너 프로그램 가입 상태와 기준 변경 | 스튜디오 화면과 공식 안내로 확인 |
| `30_facts/FACT-029-powershell-relative-path.md` | PowerShell 5.1의 상대 경로 해석 | 명령 출력으로 확인 |
| `30_facts/FACT-030-shared-assets-and-uploads.md` | 공유 산출물 폴더와 업로드 완료 건 | Philip 확인. 파일 목록 미확인 |
| `30_facts/FACT-031-classic-download-inventory.md` | classic 보유 음원 18개의 길이와 비트레이트 | ffprobe 실측 |
| `30_facts/FACT-032-render-time-by-source.md` | 소스 이미지 해상도에 따른 렌더 시간 | 실측 |

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
| `40_failures/FAIL-2026-0919-010__LAB-C__econ.md` | 브라우징 불가로 sources를 채우지 못함 |
| `40_failures/FAIL-2026-0920-001__LAB-A__enka.md` | 채널 문서의 인물 설정이 실제와 달랐음 |
| `40_failures/FAIL-2026-0920-002__LAB-A__none.md` | 조회 문제 원인을 주소 형태로 단정함 |
| `40_failures/FAIL-2026-0920-003__LAB-C__none.md` | 상위 모델에서도 조회 실패, 원인 단정 |
| `40_failures/FAIL-2026-0920-004__LAB-A__none.md` | 날짜가 바뀐 것을 확인하지 않고 전날 날짜를 사용함 |
| `40_failures/FAIL-2026-0921-001__LAB-A__none.md` | 정본과 교차 확인 주소가 함께 낡은 값을 반환함 |
| `40_failures/FAIL-2026-0921-002__LAB-A__none.md` | NVENC 부재를 하드웨어 인코딩 전체 부재로 오인함 |
| `40_failures/FAIL-2026-0921-003__LAB-A__classic.md` | 콜라주 산술 건에서 판정을 세 차례 바꿈 |
| `40_failures/FAIL-2026-0921-004__LAB-A__classic.md` | 음원 소요량을 실제의 약 4배로 산정함 |
| `40_failures/FAIL-2026-0921-005__LAB-A__none.md` | 프로젝트 첨부 파일을 확인하지 않고 회수를 권고함 |
| `40_failures/FAIL-2026-0921-006__LAB-A__none.md` | 산출물 전달 시 배치 위치를 명시하지 않음 |
| `40_failures/FAIL-2026-0921-007__LAB-A__none.md` | 과거 폴더에 정본 지정 전제를 사실 기록에 넣음 |
| `40_failures/FAIL-2026-0921-008__LAB-A__none.md` | 텔레그램 봇 간 통신 규칙을 확인 없이 단정함 |
| `40_failures/FAIL-2026-0922-001__LAB-D__none.md` | .env 읽기 실패. PowerShell 위치와 프로세스 작업 디렉터리가 달라 발생 |
| `40_failures/FAIL-2026-0922-002__LAB-D__none.md` | 파일 읽기 실패의 원인을 인코딩으로 단정함 |
| `40_failures/FAIL-2026-0922-003__LAB-D__none.md` | 파일명 규칙을 위반한 이름을 생성하고 안내함 |
| `40_failures/FAIL-2026-0922-004__LAB-D__none.md` | 승인 항목에 선택지와 기본값이 없어 결정할 수 없는 형태로 송신함 |
| `40_failures/FAIL-2026-0922-005__LAB-A__enka.md` | 사실 기록에 우리 채널 원본 수치를 적음 |
| `40_failures/FAIL-2026-0923-001__LAB-D__classic.md` | 소재를 도구로 만들다 실패. 게이트 오판, 소스 과해상도, 주소 미검증 |
| `40_failures/FAIL-2026-0923-002__LAB-A__classic.md` | 수치 게이트를 다 통과한 패키지가 육안 검수에서 폐기됨 |

## 50 성과

| 파일 | 내용 |
|---|---|
| `50_metrics/_TEMPLATE.md` | 주간 제출 양식. 실제 수치는 금고에 제출 |

실제 주간 수치는 도서관에 두지 않는다. 헌장 4절.

## 60 결정

| 파일 | 내용 |
|---|---|
| `60_decisions/ADR-0001-builder-and-repo.md` | 구축 담당과 저장소 형태 |
| `60_decisions/ADR-0002-music-source-policy.md` | 음원 조달 정책, 채널별 배분 |
| `60_decisions/ADR-0003-change-detection.md` | 도서관 변경 감지 방식. 최신 커밋 기준 |
| `60_decisions/ADR-0004-lab-autonomy.md` | 실험실의 자율 범위 |
| `60_decisions/ADR-0005-lab-workspaces.md` | 실험실별 워크스페이스 지정과 상호 접근 금지 |
| `60_decisions/ADR-0006-operating-rules.md` | 운영 규칙. 호칭, 표시명, 승인, 소통, 설계서, 공유 자원, 토큰, 선행 검토, 곡 제목과 공유, 앱 병행 |
| `60_decisions/ADR-0007-neutral-control-plane.md` | 중립 Control Plane. Railway, 1단계 기능, 텔레그램 구성 |
| `60_decisions/ADR-0008-lab-c-exit.md` | LAB-C 퇴출 |
| `60_decisions/ADR-0009-lab-d-stop.md` | LAB-D 중단. 실험실 2개. 소재와 검수 규칙 |
| `60_decisions/ADR-0010-product-goal.md` | 제품 목표. 요구 한두 줄로 조사, 프롬프트, 생성, 패키지까지 자동 |
