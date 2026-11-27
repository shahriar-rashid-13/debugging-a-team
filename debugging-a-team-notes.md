# Style continuity — Debugging a Team

Companion to `debugging-a-team.html`. Related but **not** a clone of `decision-models-slide.html` / `slide-style-notes.md`.

## Design read

- **Artifact:** 6× 16:9 deck (1920×1080 stage, JS scale-to-fit)
- **Visual language:** incident-diagnostic / ops HUD — deep navy plane, orange↔blue fault signals, orbital diagnostics on cinematic slides; hairline tech panels on slides 2–5
- **Modes:** Cinematic (01, 06) vs Technical (02–05)
- **Temperature:** authoritative, slightly urgent; hopeful close
- **Density:** cinematic = low; technical = medium (one diagram job per slide)

## Palette (locked from brief)

| Token | Hex | Use |
|---|---|---|
| `--bg` | `#101936` | Base |
| `--bg-2` | `#17254B` | Gradient lift |
| `--text` | `#F3F5FF` | Primary type |
| `--muted` | `#A9B7D8` | Supporting copy |
| `--orange` | `#FF995C` | Primary accent / root-cause / DBG ids |
| `--blue` | `#648EFF` | Secondary accent / tech chrome |
| success / error | muted greens/reds | Status chips & badges only |

**Continuity with Decision Models:** same cosmic depth idea (nebula, orbs, grain, thin rings) but **different hue pair** (orange/blue vs teal/amber) and **different type system**. Do not reuse Bricolage/Sora/IBM Plex or teal/cyan/amber tokens on this deck.

## Typography

| Role | Family |
|---|---|
| UI / display | **Manrope** 400–800 |
| Diagnostic labels | **JetBrains Mono** 400–600 |

Scale (1080p): cinematic H1 ≈ 88–92px; technical H2 ≈ 42–48px; body ≈ 16–20px; mono meta ≈ 12–14px.

## Composition rules

1. Cinematic: large L/center headline + atmospheric diagnostic visual R (or centered close).
2. Technical: eyebrow → title → one diagram (stack / dual fault / decision log / DBG checklist).
3. No emoji; no card-shadow stacks; hairline borders + left/top accent rails only.
4. Status chips are monospace system signals, not marketing pills.

## Motion

- Cinematic: `reveal` blur-lift + orb/ring drift + optional parallax
- Technical: shorter `tech-in` stagger
- Always honor `prefers-reduced-motion: reduce`

## UX chrome

←/→/Space/click advance · `1`–`6` jump · `N` speaker notes · progress dots · `01 / 06` counter · localStorage slide index
