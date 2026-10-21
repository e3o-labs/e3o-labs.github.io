# Website hero decisions

## UXD-2026-10-22-025 — 홈페이지 메인 이미지를 일상 돌봄 일러스트로 개선

- Date: 2026-10-22 (Asia/Seoul)
- Actor: product owner request + design implementation
- Selected/staged website hero: `LANDING-HERO-002`
- Published website hero: `LANDING-HERO-001` until publication approval
- Decision: 홈페이지의 단순 사람·강아지 산책 실루엣을, 집에서 눈높이를 맞추는 보호자와 강아지, 식기·산책줄·7일 기록장이 보이는 성숙한 회화풍 일러스트로 교체할 로컬 구현을 준비한다. 사용자 요청의 목적 적합성과 신뢰감을 시각적 완성도와 구체적인 돌봄 단서로 전달한다.
- Preservation: 현행 원본 HTML과 새 PNG 원본, 최종 생성 프롬프트, WebP 파생본을 별도 버전으로 보존한다. `CONCEPT-001`, `ICON-004`, `INTRO-001`, `BRAND-NAME-006`, `COMPANION-010`의 앱 선택·적용 상태는 그대로다.
- Implementation: `web/landing-site/pet-readiness/index.html`, `web/landing-site/pet-readiness/assets/care-at-home-v2.webp`, `web/landing-site/pet-readiness/assets/care-at-home-v2-640.webp`
- Accessibility/performance: 이미지 전체 노출, 대체 텍스트, figure/figcaption, 반응형 640/1024px 소스, 크기 예약과 초기 로딩 우선순위를 적용한다.
- Evidence: `docs/design/assets/landing/landing-hero-v2-implementation.md`, `outputs/landing-hero-v2/desktop-preview.png`, `outputs/landing-hero-v2/mobile-top.png`, `outputs/landing-hero-v2/mobile-lower.png`, `outputs/landing-hero-v2/harness.log`
- Publication boundary: 대상은 별도 `e3o-labs/e3o-labs.github.io` 저장소다. AGENTS.md의 git push/배포 전 승인 규칙에 따라 원격 게시 전 단계에서 대기한다. 실제 공개 사이트는 변경하지 않았다.
- Reconsideration trigger: 실제 입양 동물·훈련 서비스 오해, 모바일 식별성, 목적 이해 또는 신뢰감 피드백에 문제가 확인되면 새 버전을 추가한다.
- Proof boundary: 로컬 이미지 로딩, 데스크톱·390px 반응형 시각 검토와 프로젝트 자동 검증만 증명한다. 실제 사용자 신뢰도, 물리 iPhone/Safari, 원격 게시 후 동작 또는 서비스 오픈 준비를 증명하지 않는다.

## UXD-2026-10-22-026 — 기존 홈페이지 이미지를 유지하고 이상화된 v2 시안을 보류

- Date: 2026-10-22 (Asia/Seoul)
- Actor: product owner feedback
- Selected/published website hero: `LANDING-HERO-001`
- Staged website hero: none
- Decision: 사용자가 환상보다 현실을 표현하는 기존 방식도 지금은 나쁘지 않다고 피드백했다. 현재 공개된 담백한 일러스트를 유지하고, 정돈된 가정과 이상적 교감을 강조한 `LANDING-HERO-002`는 archived로 보존한다. 추가 제작·배포를 진행하지 않는다.
- Preservation: 원본, v2 생성 자산·프롬프트·로컬 구현·검증 증거와 최초 결정 기록을 그대로 보존한다. v2 publication manifest는 보류 상태로 변경한다.
- Future direction: 기존의 절제된 표현을 바탕으로 반복 돌봄의 시간과 책임이 전달되도록 다듬는다.
- Reconsideration trigger: 사용자가 v2 방향의 재검토를 요청하고 과도한 이상화를 줄여 돌봄의 현실을 전달할 수 있을 때 새 버전을 만든다.
- Evidence: `docs/design/assets/landing/landing-hero-v2-deferred-20261022.md`
- Proof boundary: 디자인 선택·보류 기록만 갱신한다. 공개 사이트와 앱은 변경하지 않는다.

## UXD-2026-10-22-027 — 담백한 일러스트를 유지하며 돌봄의 현실로 완성도를 높임

- Date: 2026-10-22 (Asia/Seoul)
- Actor: product owner clarification + design implementation
- Selected/staged website hero: `LANDING-HERO-003`
- Published website hero: `LANDING-HERO-001` pending publication approval
- Clarification: 직전의 ‘기존 이미지 유지’ 해석을 정정한다. 사용자 요청은 기존처럼 담백한 일러스트 스타일로 실제 돌봄의 수고가 느껴지는 새 이미지를 만드는 것이다.
- Decision: 녹색·아이보리 색면과 아치형 배경을 계승하고 인체·강아지 윤곽과 구도를 정교하게 다듬는다. 쏟아진 물을 닦는 보호자, 양말을 문 강아지, 식기·시계·산책줄로 작은 실수 정리와 반복 돌봄의 시간을 보여준다.
- Preservation: 기존 원본과 이상화된 `LANDING-HERO-002`의 자산·로컬 구현·프롬프트·증거를 모두 보존한다. 새 구현은 `web/landing-site-v3/`에 둔다. 앱 아이콘·인트로·브랜드·동반자 선택은 그대로다.
- Evidence: `docs/design/assets/landing/landing-hero-v3-implementation.md`, `outputs/landing-hero-v3/desktop-preview.png`, `outputs/landing-hero-v3/mobile-top.png`, `outputs/landing-hero-v3/mobile-lower.png`
- Publication boundary: 로컬 교체안을 준비했으며 원격 사이트는 변경하지 않았다. push/배포는 AGENTS.md에 따른 별도 승인 후 진행한다.
- Reconsideration trigger: 모바일에서 정리 행동을 읽기 어렵거나 죄책감·훈육 장면으로 오해하거나 기존의 절제된 스타일과 맞지 않으면 새 버전으로 개선한다.
- Proof boundary: 로컬 화면·정적 자산 검증만 증명한다. 사용자 신뢰감·실기기 Safari·게시 후 동작은 미검증이다.

## UXD-2026-10-22-028 — 승인된 담백한 돌봄 일러스트 v3를 공개 홈페이지에 게시

- Date: 2026-10-22 (Asia/Seoul)
- Actor: product owner approval (“반영”) + implementation
- Selected/published website hero: `LANDING-HERO-003`; staged hero: none
- Decision: 사용자가 검토한 v3 시안을 공개 홈페이지에 반영했다. `pet-readiness/index.html`과 WebP 두 파일만 변경했다.
- Remote evidence: `e3o-labs/e3o-labs.github.io` commit `38a2ac117f6a9d4857cbb76fd83b2a7e75514269`; GitHub Pages run `39626433189` completed/success.
- Validation: 원격 홈페이지 기준 blob 일치와 세 파일 변경 범위를 확인했다. 공개 HTML·이미지 두 파일의 HTTP 200 및 SHA-256 일치, 기존 링크 목적지, 개인정보·고객지원 200, 데스크톱 및 390px 공개 페이지 시각 검토를 통과했다.
- Preservation: 이전 원본·v2·v3 마스터·프롬프트·로컬 구현과 모든 결정 이력을 보존한다. 앱 아이콘·인트로·동반자·정식명 선택은 변경하지 않는다.
- Evidence asset: `docs/design/assets/landing/landing-hero-v3-published-20261022.md`
- Reconsideration trigger: 실제 모바일 화면에서 상황을 읽기 어렵거나 돌봄의 현실·정서적 톤·브랜드 이해에 문제가 확인되면 기존 기록을 보존한 새 버전으로 개선한다.
- Proof boundary: 공개 배포와 브라우저 폭별 렌더만 증명한다. 물리 iPhone/Safari, 실제 사용자 신뢰도나 서비스 오픈 준비는 증명하지 않는다.
