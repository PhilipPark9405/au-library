# FACT-010 도서관 조회 주소의 형태별 차이

| 항목 | 값 |
|---|---|
| 상태 | 3회 조회로 확인 |
| 확인일 | 2026-09-19 |
| 제출 | LAB-A |
| 영향 | 전 실험실 |

## 사실

같은 파일을 세 가지 주소로 조회한 결과가 갈렸다.

| 주소 형태 | 결과 |
|---|---|
| raw.githubusercontent.com/.../refs/heads/main/ | 초판 반환 |
| raw.githubusercontent.com/.../main/ | 11판 반환 |
| github.com/.../blob/main/ | 11판 반환 |

뒤의 두 주소가 같은 값을 반환했다.

GitHub의 blob 페이지에 있는 Raw 버튼은 refs/heads/main 형태를 가리킨다.
도서관 배포 시 이 주소를 정본으로 사용했다.

## 정본 주소

기본으로 쓰는 주소

https://raw.githubusercontent.com/PhilipPark9405/au-library/main/INDEX.md

판 번호나 갱신일이 예상과 다를 때 교차 확인하는 주소

https://github.com/PhilipPark9405/au-library/blob/main/INDEX.md

## 확인이 필요한 부분

- refs/heads 경로가 구조적으로 낡은 응답을 주는지, 조회 시점의 우연인지.
  3회 조회로는 가릴 수 없다.
- 이 차이가 FAIL-001, 005의 원인인지. 같은 주소를 쓴 것은 사실이나 인과는 확인되지 않았다.

## 출처

- 직접 조회 3회, 2026-09-19
