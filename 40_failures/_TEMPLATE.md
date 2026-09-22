# 실패 기록 양식

파일명: `FAIL-YYYY-MMDD-NNN__LAB-X__{channel}.md`

아래 필드를 쓴다. note 는 선택 필드다. 그 외 필드는 추가하지 않는다.
무엇을 하라는 권고는 쓰지 않는다. 일어난 일만 쓴다. 대응은 각 실험실이 스스로 정한다.

```
id:        FAIL-2026-0919-001
lab:       LAB-A
channel:   enka
           채널이 특정되지 않으면 none을 쓴다
stage:     research | script | music | video | thumbnail | plan | upload | other
symptom:   무엇이 관측되었나. 한 문장.
trigger:   그 직전에 무엇을 했나. 재현 가능하도록 구체적으로.
cause:     원인. 모르면 unknown이라고 쓴다. 추측을 단정으로 쓰지 않는다.
cost:      소모된 것. 크레딧, 다운로드, 시간, 지연 일수.
scope:     channel-only | all-channels | tool-wide | lab-only
status:    open | closed
closed_by: 닫힌 경우 그 근거 (FACT ID 또는 날짜)
note:      선택. 관련 기록 번호나 확인된 사실을 덧붙인다. 권고는 쓰지 않는다.
```

## scope 필드를 두는 이유

한 채널에서 난 실패가 네 채널 전체의 금지 규칙이 되면 몇 주 안에 아무것도 만들 수 없게 된다.
어디까지 적용되는 실패인지 제출자가 판단해서 밝힌다.

lab-only 는 한 실험실의 내부 절차에서 생긴 실패다. 다른 실험실의 제작 규칙으로 옮기지 않는다.

## 개정 이력

- 2026-09-22 note 선택 필드와 scope 값 lab-only 추가. 기존 기록의 stage 값 기타를 other 로 통일.

## 제출

양식대로 파일을 만들어 Philip에게 전달한다. 커밋은 Philip이 한다.
발생 후 24시간 안에 제출한다.
