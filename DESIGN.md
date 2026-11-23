# DESIGN.md: Kaushal Tatkare portfolio (v3)

**Direction:** a dark, high-contrast personal site. Its structure and feel follow john-ellison.com: an uppercase hero ringed by floating tiles, a problem grid, a playbook with stats, "ways to work" cards, featured work, an about section with a journey, and a closing CTA. All copy, visuals and code are original to Kaushal.

## Colour
| Token | Value | Role |
|---|---|---|
| `--bg` | `#000000` | Hero and footer |
| `--bg1` / `--bg2` | `#050507` / `#0B0B0F` | Alternating sections |
| `--card` | `rgba(255,255,255,.02)` | Card fill, rising to `.04` on hover |
| `--line` / `--line2` | `rgba(255,255,255,.06 / .12)` | Borders |
| `--ink` / `--ink70` / `--ink55` / `--ink40` | white at 100 / 70 / 55 / 42% | Text levels |
| `--g1` | `#7C3AED → #3B82F6 → #2DD4BF` | Signal gradient for key words and stats |
| `--g2` | `#EF4444 → #F59E0B → #FCD34D` | Second gradient, for one word in the hero and problem titles |
| Violet `#A78BFA` | — | Eyebrows, badges, icons |
| Green `#34D399` | — | "Live" status, the open-to-work dot |

## Typography
- **Archivo Expanded** (Google Fonts, 800–900 weight, width 120%, uppercase) for the hero headline. **Clash Display** (Fontshare) for other headings, falling back to Outfit. **Satoshi** (Fontshare) for body, falling back to Manrope. JetBrains Mono only in the API tile.
- Hero: clamp(30–60px) on desktop, clamp(22–30px) on phones; four lines on phones.
- Section titles: clamp(34–58px), 600 weight, -.02em.
- Eyebrows: 12.8px uppercase, .12em tracking.
- Body: 17.5px, 300–400 weight.

## Components
- **Buttons:** 48px tall, 8px radius, uppercase labels with .12em tracking. Three variants: solid white, outline, and violet-tint.
- **Cards:** 12–16px radius with a 1px white/6% border. Hover adds a violet border.
- **Flagship card:** violet gradient wash plus a gradient "Primary" tag.
- **Work cards:** a 16:10 gradient "shot" area showing a big metric, with role and status pills.
- **Experience:** `<details>` accordions.

## Motion
Floating tiles drift slowly, and sections fade up on scroll. Both are disabled under `prefers-reduced-motion`.
