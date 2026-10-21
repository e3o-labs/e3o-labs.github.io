# 홈페이지 일러스트 v3 공개 반영

- 날짜: 2026-10-22 (Asia/Seoul)
- 결정: UXD-2026-10-22-028
- 승인: 사용자가 검토한 v3 시안에 “반영”이라고 명시적으로 승인했다.
- 선택·공개: LANDING-HERO-003. 게시 대기 시안 없음.
- 공개 URL: https://e3o-labs.github.io/pet-readiness/
- 저장소: e3o-labs/e3o-labs.github.io
- 반영 커밋: 38a2ac117f6a9d4857cbb76fd83b2a7e75514269
- GitHub Pages 실행: https://github.com/e3o-labs/e3o-labs.github.io/actions/runs/39626433189 — completed / success.

## 반영 범위

`pet-readiness/index.html`을 수정하고 `pet-readiness/assets/everyday-care-v3.webp`, `pet-readiness/assets/everyday-care-v3-640.webp`를 추가했다. 정확히 세 파일의 변경이며 다른 서비스와 개인정보·고객지원 폴더는 변경하지 않았다. 게시 직전 홈페이지 원격 blob이 검토 기준 `3e4e850152012d7ca461e320557b49d53f3f7d7e`와 같음을 확인하고, 기존 main을 부모로 한 커밋을 생성한 뒤 예상 head 검사를 포함한 일반 fast-forward로 적용했다.

## 게시 후 검증

- 공개 HTML과 이미지 두 개: HTTP 200, 승인된 로컬 파일과 SHA-256 일치.
- 개인정보·고객지원 페이지: HTTP 200.
- 실제 공개 페이지: 이미지 로딩, 대체 텍스트, 새 설명, 기존 링크 목적지와 데스크톱 가로 넘침 없음 확인.
- 실제 공개 URL을 390px iframe에서 열어 첫 화면, 이미지 전체와 설명을 시각 검토했다.
- `python3 scripts/validate_design_governance.py`, `git diff --check`: 통과.
- 실패하거나 제외된 게시 검증 없음. 전체 앱 회귀 테스트는 정적 홈페이지 자산만 게시하여 재실행하지 않았다.
- 물리 iPhone/Safari 및 실제 사용자 이해도는 별도 검증이 필요하다. 서비스 오픈 준비 판정을 변경하지 않는다.

증거는 `outputs/landing-hero-v3/publication-evidence.json`, `live-http-check.json`, `live-browser-check.json`, `live-desktop.png`, `live-mobile-top.png`, `live-mobile-lower.png`에 보존한다. 최초 구현 문서의 미게시 상태는 당시 이력이며, 현재 상태는 이 문서와 디자인 등록부를 따른다. 기존 모든 자산과 탐색 기록을 보존한다.
