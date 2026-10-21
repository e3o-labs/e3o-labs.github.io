# 나란히 걸어봄 홈페이지 일러스트

현재 선택·공개 자산은 `LANDING-HERO-003`이다. 초록색·아이보리의 담백한 색면을 유지하면서, 쏟아진 물을 닦는 보호자와 양말을 문 강아지, 식기·산책줄·시계로 돌봄의 현실을 표현한다.

실제 페이지는 `pet-readiness/index.html`, 반응형 파생본은 `pet-readiness/assets/everyday-care-v3.webp`와 `everyday-care-v3-640.webp`다. 페이지 figure의 `data-hero-asset-id`와 `pet-readiness/assets/hero-v3-manifest.json`을 통해 원본·프롬프트·파일 해시를 추적할 수 있다. 이 식별자는 화면·접근성 읽기·동작을 바꾸지 않는다.

이미지는 사용자의 ‘반영’ 승인 후 커밋 `38a2ac117f6a9d4857cbb76fd83b2a7e75514269`로 먼저 게시되었다. 이 후속 PR은 직접 게시된 이력을 되돌리지 않고, 적용 식별자·manifest·원본·탐색 이력을 같은 저장소에 동기화한다. PR 전후 이미지와 설명은 동일하다.

`history/`에는 공개 전 원본 HTML, 보류한 v2와 선택된 v3의 원본 PNG·생성 프롬프트·각 시점의 구현/상태 기록을 보존한다. 당시 문서의 경로와 미게시 상태는 원래 작업 공간과 작성 당시를 기준으로 한다. 현재 상태는 이 문서, `design-registry.json`, `decision-log.md`와 실제 배포 이력을 따른다. 과거 자산을 덮어쓰지 않고 새 버전과 결정을 추가한다.

검증은 공개 HTML·이미지 해시, 고객지원·개인정보 HTTP 응답, 데스크톱·390px 브라우저 렌더를 확인했다. 물리 iPhone/Safari와 실제 사용자 이해도는 별도 검증 대상이다. 이 변경은 앱의 서비스 오픈 준비 판정을 변경하지 않는다.
