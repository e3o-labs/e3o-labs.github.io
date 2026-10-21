# Homepage hero v2 — attentive care at home

- Date: 2026-10-22 (Asia/Seoul)
- Request: replace the main illustration at https://e3o-labs.github.io/pet-readiness/ with a more purposeful, credible illustration.
- Selected/staged: `LANDING-HERO-002`; current published: `LANDING-HERO-001`.
- Source: `e3o-labs/e3o-labs.github.io`, `pet-readiness/index.html`, original blob `3e4e850152012d7ca461e320557b49d53f3f7d7e`.
- Generated with built-in imagegen; no paid API/CLI fallback was used. Exact final prompt: `docs/design/assets/landing/landing-hero-v2-prompt.txt`.
- Generated master: `landing-hero-v2-care-at-home.png`, 1254 × 1254, retained intact. Optimized 1024px/640px WebP derivatives are under `web/landing-site/pet-readiness/assets/`.

## Design and implementation

The previous walking silhouette is preserved in `landing-hero-v1-original.html`. The replacement shows an adult caregiver meeting the dog's eyes at home, supported by food/water bowls, a walking leash and a seven-mark journal. Soft sage, forest and ivory connect it to CONCEPT-001. The scene communicates daily attention and preparation without approval seals, scores or medical authority.

The local homepage replaces only the inline hero SVG and its framing/caption. The figure includes descriptive alternative text, responsive image sources, intrinsic dimensions to reserve layout space, and high fetch priority. The square artwork is shown in full. Existing navigation, service descriptions, CTA targets and release status remain the upstream values.

Caption: “밥을 챙기고, 산책을 준비하고, 하루를 돌아보는 연습.”

## Validation and publication boundary

- `scripts/agent-harness.sh`: passed; full output in `outputs/landing-hero-v2/harness.log`.
- The harness initially skipped one feedback API test because the sandbox blocked loopback binding. `python3 scripts/test_service_feedback_api.py` was rerun with local-port access and passed (1 test, no skip). No automated check remains failed or skipped.
- `python3 scripts/validate_design_governance.py`: passed after registry/document changes.
- Browser: desktop 1265px; image loaded, page width equals viewport width; visual review passed.
- Browser: 390px iframe viewport; visual review of text, buttons, uncropped square artwork and caption passed. Evidence: `mobile-top.png`, `mobile-lower.png` under `outputs/landing-hero-v2/`.
- The mobile check is a responsive browser preview, not physical iPhone or Safari verification. Cross-device rendering and user perception of trust remain unverified.
- The original HTML, master and both derivatives have recorded SHA-256 hashes in the design registry or publication manifest.
- Focused static checks passed: unchanged navigation/CTA targets, unique IDs, alternative text, intrinsic/responsive dimensions, asset hashes and exactly three publication files. Manifest and ZIP are under `outputs/landing-hero-v2/`.
- Remote push/deployment and post-publication URL verification are pending owner approval, as required by AGENTS.md. No live files changed.
- Local preview privacy/support destinations are not bundled; those existing remote folders must remain untouched when publishing.

## Publication plan

Publish exactly `pet-readiness/index.html`, `pet-readiness/assets/care-at-home-v2.webp`, and `pet-readiness/assets/care-at-home-v2-640.webp` from `web/landing-site/` to `e3o-labs/e3o-labs.github.io`. Exclude `mobile-preview.html`. Before writing, compare the remote index blob with the recorded original; reconcile any intervening edits. After publication, verify the live hero, image URLs, mobile layout and unchanged CTA targets. Preserve the old source and all design assets.

Reconsider if the scene is mistaken for real adoption inventory, reads as a training course rather than virtual care practice, becomes illegible on mobile, or real users report weak purpose/trust comprehension. Record any revision as LANDING-HERO-003 or later.
