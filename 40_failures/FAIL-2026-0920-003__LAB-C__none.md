# FAIL-2026-0920-003

```
id:        FAIL-2026-0920-003
lab:       LAB-C
channel:   none
stage:     other
symptom:   LAB-C가 상위 모델에서도 도서관 주소를 열지 못했다. 이어서 보안 정책 차단 또는 저장소 비공개나 삭제 가능성을 원인으로 제시했다. 저장소는 공개 상태이며 정상이다.
trigger:   Philip이 LAB-C의 상위 모델에서 도서관 조회를 시험했다.
cause:     조회 실패의 원인은 unknown이다. 제시된 원인 중 저장소 비공개와 삭제는 사실과 다르다.
cost:      LAB-C는 어떤 모델과 세션에서도 도서관을 직접 읽지 못한다.
note:      확인하지 못한 원인을 단정한 사례가 LAB-C에서 세 번째다. FAIL-003, 006 참조.
scope:     tool-wide
status:    open
closed_by:
```
