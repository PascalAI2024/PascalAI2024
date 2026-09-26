# Profile README draft and pinned repos — 2026-09-26

Draft only. Nothing here is published. Board item: `presence-github-profile-20260924`.

`README.proposed.md` is the live `README.md` (main `2eb24a1`, identical to
`origin/main` at fetch time) with three content edits. The header, typing
animation, SVG assets, logos, tables, Mermaid diagram and layout are untouched,
per the preservation rule in `CURRENT_WORK.md`.

## Changes against the live README

| # | Section | Change | Why |
|---|---|---|---|
| 1 | Products, IGD Dev Lab list | Removed **HVAC Recruit** | `https://hvac-recruit.com` returns 404 at the root (checked 2026-09-26, two user agents). A named product with no working surface reads as a dead claim. Restore it when the site is back. |
| 2 | In-house | Removed the PAL line (`pal-lang`) | Stub: 10 files, 3 commits, no declared license. The brief says never cite stubs. |
| 3 | In-house | Added **Agent cockpit** entry linking to `portfolio/case-studies/agent-cockpit.md` | The multi-agent cockpit is current flagship work and was absent. The link target does not exist yet; it goes live only if `CASE-STUDY-agent-cockpit.md` is published to the portfolio repo first. |

Not changed, but the owner should decide:

- **Client names.** The live README's "Client work" section names client sites.
  The brief for this item says never name clients in public-facing text. Those
  names were published earlier by the owner (commit `7349f11`), so this draft
  leaves the section as it is instead of overriding that decision. If the rule
  applies retroactively, the section would drop to the studio's own site plus
  anonymous descriptions ("an artist portfolio", "a med-spa storefront").
- **HerCircle** stays in the Dev Lab list: its web root returned 200 today. Its
  API host (`api.hercircle.igddev.com`) returns 404 at the root, but the README
  does not link it.

## Flagship check (by size and recency)

Public, non-fork repos on PascalAI2024, measured 2026-09-26:

| Repo | Files | Commits | Last push | Verdict |
|---|---:|---:|---|---|
| JarvisNano | 734 | 345 | 2026-09-25 | Flagship |
| ZiggyZag | 129 | 169 | 2026-09-22 | Flagship |
| fplbench | 92 | 57 | 2026-09-25 | Flagship |
| picoarmy | 99 | 49 | 2026-06-04 | Real, but idle since June and never deployed |
| kintunnel | 121 | 31 | 2026-09-25 | Real, active, runnable MVP with a project page |
| maple-preview-windows-cuda | 55 | 20 | 2026-09-22 | Flagship (measured results) |
| portfolio | 55 | 17 | 2026-09-22 | Index for the case studies |
| verrow | 134 | 2 | 2026-05-18 | Real code dump, thin history |
| qwen38-27b-quant-bench | 20 | 1 | 2026-08-15 | Finished research record, fine to cite |
| pal-lang | 10 | 3 | 2026-09-25 | Stub — do not cite |
| switchboard | 8 | 1 | 2026-08-27 | Stub — do not cite |
| Kaggle-Portfolio | 10 | 2 | 2026-08-08 | Stub — do not cite |
| VibeGotchi | 70 | 36 | 2026-06-01 | Kept out of the showcase by earlier owner direction |

The largest Ingenious-Digital-LLC repos (Aetheris, igd, Igdcrm, Asteria,
IGDgame, Foundry, polyhuntr) are all private, and so is the cockpit (it lives in
the private config repo). The only public org repo is a fork (rybbit). Private
work can be described on the profile, as the live README already does, but it
cannot be pinned for visitors.

## Proposed pinned repos (six slots)

Currently pinned: JarvisNano, ZiggyZag, maple-preview-windows-cuda, portfolio,
picoarmy, fplbench.

| Slot | Repo | Reason |
|---|---|---|
| 1 | JarvisNano | Largest and most active public repo; real firmware on real hardware. |
| 2 | maple-preview-windows-cuda | The strongest measured result: 52 → 377 tok/s, checked against a 103-case reference. |
| 3 | fplbench | A live benchmark that grades itself every gameweek, with a public dataset. |
| 4 | ZiggyZag | Steady history (169 commits) in a language few profiles show. |
| 5 | kintunnel | **Replaces picoarmy.** Active this week, runnable, and has its own project page. |
| 6 | portfolio | The index of case studies, including the private work that cannot be pinned. |

Dropped: **picoarmy**. It is real (99 files, 49 commits) but hasn't been pushed since
June and says "no deployment" itself. It stays in the README's project table.

## Owner actions

- Review `README.proposed.md` rendered (dark and light) before replacing `README.md`.
- Publish `CASE-STUDY-agent-cockpit.md` to `PascalAI2024/portfolio` before the
  README links to it, or drop the link line.
- Change the pins in GitHub profile settings (picoarmy → kintunnel).
- Decide whether the "never name clients" rule covers the existing Client work section.
