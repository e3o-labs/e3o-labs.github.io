# Homepage hero v3 — restrained illustration of everyday care

- Date: 2026-10-22 (Asia/Seoul)
- Decision: UXD-2026-10-22-027
- Owner clarification: improve the quality in the original restrained illustration style while conveying the reality of care; do not keep the original image unchanged.
- Selected/staged: LANDING-HERO-003. Published: LANDING-HERO-001. LANDING-HERO-002 stays archived.

## Design

Flat forest/sage/ivory color fields and an arched backdrop preserve the original visual language. A caregiver crouches to wipe spilled water while the dog holds a sock. Bowls, scattered kibble, a dustpan, a clock and a hanging leash make ordinary work and time legible. Refined anatomy, coherent silhouettes and limited contour lines replace the crude original figures. There is no luxury interior, idyllic lighting, certification, shame or punishment.

The small dots are decorative, not a numbered or interactive progress indicator. The existing seven-day copy and actual 1–7 progress section remain the source of the duration information.

Caption: “산책 준비부터 작은 실수 정리까지, 돌봄이 더해진 하루.”

## Files and preservation

- New original PNG: `docs/design/assets/landing/landing-hero-v3-everyday-care.png` (1254 × 1254).
- Built-in imagegen generation; exact final prompt: `docs/design/assets/landing/landing-hero-v3-prompt.txt`. No CLI/API fallback.
- New local homepage: `web/landing-site-v3/pet-readiness/index.html`.
- Responsive derivatives: `web/landing-site-v3/pet-readiness/assets/everyday-care-v3.webp` (1024px), `everyday-care-v3-640.webp` (640px).
- Preview-only wrapper: `web/landing-site-v3/mobile-preview.html`.
- The original and v2 images, HTML, prompts and evidence remain intact. The new root prevents overwriting the v2 exploration.
- Registry, master brief, decision log and worklog record the clarified direction.

## Validation

- `python3 scripts/validate_design_governance.py`: passed.
- `git diff --check`: passed for the changed tracked design files.
- Focused HTML/asset checks: passed for unchanged navigation and CTA destinations, unique IDs, existing content outside the hero, alternative text, intrinsic dimensions, responsive sources, source hashes and the exact three-file publication bundle.
- Desktop 1265px: image loaded, document width equals viewport width, visual review passed. `outputs/landing-hero-v3/desktop-preview.png` and `desktop-check.json`.
- Mobile 390px iframe: visually checked first screen, complete uncropped illustration and caption. `outputs/landing-hero-v3/mobile-top.png` and `mobile-lower.png`.
- No failed focused check remains. Local server initially could not bind in the sandbox and was successfully started with local-port permission.
- Full application regression suite was not repeated for this isolated static image/content revision; the earlier v2 full harness and feedback API rerun passed. Physical iPhone/Safari, user comprehension and post-publication verification remain unperformed.

## Publication boundary

The live site has not changed. AGENTS.md requires approval before push/deployment. After approval, publish only `pet-readiness/index.html`, `pet-readiness/assets/everyday-care-v3.webp`, and `pet-readiness/assets/everyday-care-v3-640.webp` from the new local root to `e3o-labs/e3o-labs.github.io`. Preserve remote privacy/support folders. Compare the current remote index with original blob `3e4e850152012d7ca461e320557b49d53f3f7d7e` before writing; reconcile any intervening edits. Then verify the live image, mobile layout and CTA destinations.

Reconsider through a new version if small-screen readability, the daily-care meaning, emotional tone or style alignment fails owner/user review. Local rendering does not prove user trust or real-device quality.
