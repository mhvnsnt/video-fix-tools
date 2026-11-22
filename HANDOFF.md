# HANDOFF — video-fix-tools

**Last updated: 2026-11-22 (America/New_York).**
**Repo:** `mhvnsnt/video-fix-tools` (PUBLIC), default branch `main`.
**Purpose of this file:** any agent that picks up work here reads this FIRST, then the linked docs. It states what we've done, where we're at, and what we're working toward — so the owner can say "go to this repo, pick up the work" and you just know. Update this file in the same PR whenever the state changes (add, don't delete).

## 1. What this repo is

The Open Source Animation Pipeline — tools for fixing AI-generated video back to 2D cartoon style. The repo holds the pipeline code for taking AI video that came out wrong and getting it back to clean cartoon frames. Small repo (~19 KB on main).

Current contents: `ai-body-replace/` (the body-replace tool), `AGENTS.md`, `WORKING-METHOD.md`, `README.md`.

## 2. Where we're at

### DONE
- **Archive release vft-archive-2026-10-15 (2026-10-15):** the pipeline snapshot as a release.
- **Anti-clobber laws (2026-10-17, PR #2 merged):** the owner's anti-clobber laws landed in `AGENTS.md` after the DXMMII 54k-file wipe.
- **Working method statement (2026-10-27):** `WORKING-METHOD.md` landed.

### IN PROGRESS
- Nothing is actively in progress in this repo that the repo itself records. Last push was the 2026-10-27 sweep commit (via the 2026-11-20 push batch).
- **PRE-MADE PARTS FIRST rule (open PR #3).** Standing-rule PR, unmerged.

### BLOCKED
- Nothing recorded as blocked in this repo.

## 3. What we're working toward

A pipeline that reliably turns AI video back into real 2D cartoon style — clean, solid drawings, no ghostly interpolation, no warp-and-smear. The bar (owner): tweening, not interpolation — each in-between a clean solid drawing on a tween curve, never a blend of two keys. No stills with pans and zooms standing in for movement.

## 4. Standing rules that apply here

- **Branch → PR → merge, always.** Never push to main directly. Add-only, zero-conflict PRs, no force pushes.
- **Checkpoint-and-save law:** CHECKPOINT.md first, update after every step; the repo is the save; resume, never restart.
- **No-temp-storage law:** nothing in /tmp or any wipeable location, ever.
- **Real-source-only:** build from the real sources, wired up fully — no hand-tooled lookalikes.
- **No shortcuts:** use the best tools available, not the quickest hack. No warp-and-paste when the ask is AI.
- **Tweening, not interpolation.** No ghostly AI frame interpolation — no warping, smearing, melting, or double images.
- **Never kill in-progress work.**

## 5. Key files and paths

| What | Where |
|---|---|
| Body-replace tool | `ai-body-replace/` |
| Agent rules | `AGENTS.md` |
| Method doc | `WORKING-METHOD.md` |
| Releases | `vft-archive-2026-10-15` |
| Open PR | #3 (PRE-MADE PARTS FIRST rule) |
| Related repos | `mhvnsnt/cape-jones` and `mhvnsnt/dream-girl` (the shows this pipeline serves) |

## 6. Open decisions needing the owner

- No decisions are recorded in this repo. What the pipeline fixes next is driven by the shows' needs — his call.

## 7. How to pick up

1. Read this HANDOFF.md first, then `README.md` and `WORKING-METHOD.md`.
2. Check what the shows actually need fixed before changing the pipeline (never rebuild it blind).
3. Check what other agents are already doing before starting anything.
4. Resume from the stated next step — never restart, never re-derive finished work.
5. Land work branch → PR → merge, add-only. Stage finished work to the repo as it lands.
6. Update this HANDOFF.md in the same PR when the state changes. Verify with your own eyes before claiming anything fixed.
