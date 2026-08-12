# Module F assets

Competitor-facing media and copy for the SwapLoop public marketing site.

## Layout

```text
assets/
  texts/copy-deck.md                 # Required copy and data tables
  prompts/image-generation-prompts.md
  images/                            # Raster / web images
  icons/                             # SVG icons
```

## Required vs optional

| File / set | Status | Used on |
| ---------- | ------ | ------- |
| `texts/copy-deck.md` | **Required** | All pages |
| `images/logo-swaploop.svg` (or PNG) | **Required** | Header / footer |
| `images/hero-home.jpg` | **Required** | Home |
| `images/station-haitang.jpg` | **Required** | Stations (+ Home teaser) |
| `images/station-canal-view.jpg` | **Required** | Stations |
| `images/station-morning-bridge.jpg` | **Required** | Stations |
| `images/og-default.jpg` | **Required** | Home Open Graph |
| `images/favicon.svg` (or `.ico`) | **Required** | All pages |
| `icons/icon-swap.svg` | **Required** | How it works / types |
| `icons/icon-charge.svg` | **Required** | How it works / types |
| `icons/icon-hybrid.svg` | **Required** | Types |
| `icons/icon-rider.svg` | **Required** | Home / riders |
| `icons/icon-fleet.svg` | **Required** | Home / fleets |
| `icons/icon-safety.svg` | **Required** | Safety notes |
| `images/map-vignette.svg` | Optional | Stations / Home |
| `images/priority-windows.svg` | Optional | For fleets |
| `videos/home-loop.mp4` | Optional | Home only |

If a binary file is missing, generate it from [`prompts/image-generation-prompts.md`](./prompts/image-generation-prompts.md) and place it at the path above before assessment. Competitors must still reference these paths (or clearly equivalent names documented in their submission).

## Notes for authors

- Prefer Module C station names and hours for public copy.
- Do not ship real operator logos.
- Keep the featured station count at **three** to limit repetitive markup (no JS).
