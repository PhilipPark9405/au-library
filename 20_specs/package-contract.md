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
    "banned_words": "pass | fail",
    "synthetic_disclosure": "set | not_required",
    "human_approved": false
  },
  "status": "draft | ready | approved | uploaded"
}
```

## 필드 설명

- `download_consumed` — 이 패키지가 소비한 Suno 다운로드 횟수. FACT-001 때문에 반드시 센다.
- `human_approved` — 사람이 승인하기 전에는 false. 이 값이 false면 업로드하지 않는다.
- `synthetic_disclosure` — AI 생성 음성이나 인물이 들어간 경우 업로드 설정에서 표기했는지.
