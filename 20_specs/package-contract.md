# 영상 패키지 완료 조건

패키지 1건은 아래 5개가 전부 있을 때만 완료로 본다.
"작성했습니다"라는 문장은 완료 근거가 아니다. 파일 경로가 근거다.

| 항목 | 수량 | 형식 |
|---|---|---|
| 롱폼 | 1 | mp4 |
| 숏폼 | 2 | mp4, 세로 9:16 |
| 썸네일 | 1 | png 또는 jpg, 1280x720 |
| 업로드 계획서 | 1 | json, upload-plan 스키마 준수 |

## 완료 판정 필드

```json
{
  "package_id": "PKG-2026-0919-econ-01",
  "channel": "econ",
  "lab": "LAB-A",
  "files": {
    "longform": "경로",
    "short_1": "경로",
    "short_2": "경로",
    "thumbnail": "경로",
    "upload_plan": "경로"
  },
  "sources": {
    "music_origin": "suno | public_domain | licensed | none",
    "footage_origin": "generated | licensed | own",
    "download_consumed": 0
  },
  "checks": {
    "banned_words": "pass | fail | unknown",
    "synthetic_disclosure": "set | not_required | unknown",
    "human_approved": false
  },
  "status": "draft | ready | approved | uploaded"
}
```

## 필드 설명

- `download_consumed`: 이 패키지가 소비한 Suno 다운로드 횟수. FACT-001 때문에 반드시 센다.
- `human_approved`: 사람이 승인하기 전에는 false. 이 값이 false면 업로드하지 않는다.
- `synthetic_disclosure`: AI 생성 음성이나 인물이 들어간 경우 업로드 설정에서 표기했는지.
- 검사 대상이 아직 존재하지 않으면 `unknown`을 쓴다. 검사하지 않은 것을 `pass`로 적지 않는다.
- `synthetic_disclosure`는 유튜브 업로드 설정에서 표기를 켰는지를 뜻한다. 설명문에 문구를 넣은 것과는 다른 항목이다.

## 육안 검수

수치 검사만으로 완료로 보지 않는다. 해상도와 비트레이트는 통과 조건의 일부일 뿐이다.

- 롱폼은 30초 간격 컨택트시트 1장, 숏폼은 3초 간격 1장을 만든다.
- 기준선 패키지(FACT-017)의 같은 종류 캡처와 나란히 놓고 비교한 결과를 적는다.
- 만든 쪽이 먼저 보고, 기준선에 못 미치면 사람에게 올리지 않는다.
- 사람이 보고 승인하기 전에는 status 를 approved 로 올리지 않는다.
- FAIL-2026-0923-002 참조.

## 영상 소재

소재를 사람이 넣든 도구가 만들든 아래 관문을 통과해야 쓴다.

- 소재마다 출처와 라이선스를 기록한다. 모르면 unknown 으로 적고 업로드 승인 때 판단한다.
- 소스 이미지는 렌더에 넣기 전에 2200x1238 로 줄인다. FACT-032 참조.
- 소재 품질을 파일 크기나 해상도로만 판정하지 않는다. 압축이 잘 되는 사진이 크기 미달로 걸러질 수 있고,
  해상도만 높은 잡음 이미지가 통과할 수 있다. FAIL-2026-0923-001 참조.
- 도구가 만든 소재는 쓰기 전에 사람이나 그림을 볼 수 있는 검사기가 실제로 보고 판정한다.
  판정 없이 렌더에 넣지 않는다.
- 같은 소재를 한 편에서 세 번 넘게 쓰지 않는다.

### 적용 범위

이 절은 우리 채널 패키지에 적용한다.
2026-09-24 현재 우리 채널 패키지의 소재는 사람이 넣는다. 도구가 만든 소재가 육안 기준을 넘지 못했기 때문이다.
이것은 현재 품질 수준에서 나온 임시 방식이며, 앱의 소재 자동 생성을 막는 규칙이 아니다.
앱의 목표는 ADR-0010 이 정한다.
