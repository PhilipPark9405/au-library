# FAIL-2026-0921-001

```
id:        FAIL-2026-0921-001
lab:       LAB-A
channel:   none
stage:     other
symptom:   FACT-010이 정본으로 지정한 raw /main/ 주소와 교차 확인용 blob 주소가
           같은 시각에 둘 다 09-19 11판을 반환했다. 실제 저장소는 09-20 1판이었다.
           LAB-A는 이 값을 최신으로 보고했다. 같은 주소를 두 번째 조회했을 때
           GitHub 내부 request-id 가 첫 조회와 동일했다.
trigger:   세션 시작 시 도서관 조회. Philip이 지적해 확인되었다.
cause:     unknown. 교차 확인 두 경로가 독립적이라는 전제가 성립하지 않았다.
cost:      FACT 건수와 갱신일을 틀리게 보고했다. FACT-008 존재를 부정했다.
           확인에 왕복 세 차례가 들었다.
note:      clone 은 같은 시각 정상 값을 반환했다. 이후 LAB-A는 clone 으로 전환했다.
           ADR-0003 의 2차 방법과 FACT-010 의 교차 확인 항목에 영향이 있다.
scope:     tool-wide
status:    open
closed_by:
```
