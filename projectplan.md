# Project plan — s17-sitc2026-module-f (Process 1: content update)

## Goal

Standardize `project-description.md`, `metadata.json`, and `README.md` for Module F against the MITS Project Task Creation Guide, **without changing task meaning or omitting requirements**.

## Current state

- Content already authored as a full competitor brief (HTML/CSS public site for SwapLoop).
- Structure mostly matches MITS (`Competition time` → `Introduction` → `General Description` → `Requirements` → `Assessment` → `Mark distribution`).
- `metadata.json` and `README.md` exist but need light alignment with Module C style and the latest description.
- Author-only file `AUTHOR-TODO-missing-assets.md` stays out of Process 1 (not competitor content).
- Marking scheme is **out of scope** for this process.

## Planned changes (form + clarity only)

### `project-description.md`

| Item | Action |
| ---- | ------ |
| Title | Keep `# Test Project Outline – Module F – SwapLoop Public Website` (aligned with Module C naming style). |
| Out of scope | Restore a `### Not part of this module` section under Requirements (was dropped in earlier edits). Content = existing exclusions (no JS, no rewriting required text, no APIs/apps, English only, max 3 stations). |
| Harder CSS hints | Trim leftover implementation hints (exact timing examples / sample HTML comments) — keep required behaviour only. |
| Assessment / Mark distribution | Keep; note mark table is draft pending marking-scheme process. Minor wording polish only. |
| Language | Keep clear English; no new scope. |

### `metadata.json`

| Field | Action |
| ----- | ------ |
| `description` | Refresh to match current required features (5 pages, fixed breakpoints, provided text, sticky header, CSS-only tabs, timeline, overlapping images, sticky prices, a11y/SEO, motion). Start with **Build**. |
| Other fields | Keep name, displayName, url, estTime 3, authors, technologies, tags (small tag polish if needed). |

### `README.md`

| Item | Action |
| ---- | ------ |
| Style | Align with Module C: short description, `## Task origin`, richer Content links (`project-description.md`, `assets/texts/copy-deck.md`, `assets/`, marking). |
| About | Keep Erasmus+ blurb (minor casing to match Module C if needed). |

## Requirement traceability checklist

| Original / current requirement | Where it stays |
| ------------------------------ | -------------- |
| 3 hours | Competition time + metadata `estTime` |
| HTML/CSS only; CSS frameworks OK; no JS | General Description + Technology rules + Not part of this module |
| 5 pages: Home, How it works, Stations, For riders, For fleets | General Description + Requirements → Pages |
| Breakpoints: &lt;768 / 768–1023 / ≥1024 | Technology rules + Assessment |
| Required text from `copy-deck.md`; extras allowed if not overwriting | Provided text + Requirements intro |
| Provided assets list (logo, hero, stations, og, icons, optional map/video) | Provided files |
| Common: skip link, header/logo, nav, footer, responsive chrome | Site structure |
| Home: hero, why outdoor, 3-step preview, station teaser, optional video below hero | Home #### |
| How it works: intro, timeline steps, comparison, safety, rider app line | How it works #### |
| Stations: CSS-only tabs, 3 featured stations, coverage, optional coming soon/map, desktop overlap images | Stations #### |
| For riders: intro, PAYG table + sticky desktop, pay per use, Alipay line, checklist, optional monthly note, app link | For riders #### |
| For fleets: intro, Partner plans, volume discounts, priority windows, funding, optional partners, contact | For fleets #### |
| Sticky header; CSS tabs; timeline; overlap images; sticky prices; hover/focus transitions; hero fade-in; `prefers-reduced-motion` | Harder CSS and animation |
| Accessibility + SEO requirements | Accessibility + SEO |
| Draft marks 5 / 70 / 25 | Mark distribution |
| README + metadata describe the task | README.md + metadata.json |

## Out of scope for this process

- Creating/downloading missing binary images (see `AUTHOR-TODO-missing-assets.md`)
- Marking scheme generation/conversion (Process 2)
- Process 3 review.md

## Approval

Approved with one change: **do not** restore `### Not part of this module`.

## Review (Process 1 complete)

### Done

- [x] Trimmed implementation hints in Harder CSS / navigation (kept required behaviour only)
- [x] Did **not** restore “Not part of this module” (per approval)
- [x] Updated `metadata.json` `description` to match current required features
- [x] Aligned `README.md` with Module C style (task origin, content links)

### Coverage check

All requirements from the approved plan’s traceability checklist remain in `project-description.md` (pages, breakpoints, provided text rule, common layout, page sections, harder CSS, a11y, SEO, draft mark distribution). No requirement was removed for form cleanup.

### Gaps / next steps (outside Process 1)

- Missing binary images still listed in `AUTHOR-TODO-missing-assets.md`
- Marking scheme still draft in the description — run Process 2 (`mits-marking-scheme-creator` / marking-scheme updater) when ready
- Optional Process 3 review when content + marking are stable
