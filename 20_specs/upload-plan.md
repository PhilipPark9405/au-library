# 업로드 계획서 스키마

채널과 무관하게 동일한 스키마를 쓴다. 실험실이 바뀌어도 다음 공정이 그대로 받도록 하기 위한 것이다.

```json
{
  "plan_id": "PLAN-2026-0919-econ-01",
  "channel": "econ",
  "publish_at": "2026-09-19T19:00:00+09:00",
  "visibility": "private",
  "title": "",
  "description": "",
  "tags": [],
  "chapters": [
    { "t": "00:00", "label": "" }
  ],
  "lyrics": {
    "present": false,
    "language": "",
    "text": ""
  },
  "timeframe": {
    "longform_sec": 0,
    "short_1_sec": 0,
    "short_2_sec": 0
  },
  "thumbnail_text": "",
  "language": "ko",
  "captions": [],
  "sources": [],
  "notes": ""
}
```

## 규칙

- `visibility`는 처음에 반드시 `private`. 사람이 확인한 뒤 예약 공개로 바꾼다.
- `title`은 100자를 넘기지 않는다.
- `tags`는 15개를 넘기지 않는다.
- `lyrics.present`가 true면 `text`가 비어 있으면 안 된다.
- `sources`에는 본문에 쓴 수치와 인용의 출처 URL을 넣는다. 경제 채널은 비울 수 없다.
