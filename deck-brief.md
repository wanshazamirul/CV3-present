# CV4 Presentation: Deck Brief

> **Status: brief + build, 2026-10-18** · full redo, from scratch (Wan's call, night session). The deck source lives here (`index.html`); the old CV3 deck stays in git history only.

## Goal & audience

Show **what CV4 is, how it runs daily, and how to start** to anyone new to it: a team, a pilot user, a curious engineer. Evidence-first, no sales theatre, sanitized (mock names only, no private data).

## Format

- Single-file `index.html`, offline, double-click to open. Assets are local (fonts, icons).
- Present with `→` / `Space` / click: each slide auto-plays its beats, then `→` moves on (press once to complete a playing slide, again to advance). `←` back, `R` replay slide, `F` fullscreen.
- Touch: swipe, on-screen arrows. `Ctrl+P` prints one slide per page (static, all layers shown).
- Hosted copy: https://wanshazamirul.github.io/CV3-present/

## Art direction (locked: "Paper & Signal", plus a working palette)

Wan's brief: minimalist, fades, typing, a lot of motion. One direction, no menus:

- **Paper**: warm white ground, ink text, hairline rules. Dark chapters (terminal, spec-kit) for contrast.
- **Signal set**: vermilion stays the "live" signal (cursors, traveling dots, key marks). Four working colors carry meaning everywhere else: blue = recall and reading, green = record and saving, amber = proof and versions, plum = the spec-kit work layer. The problem statement stays stark on purpose: color arrives with the solution.
- **Type**: Fraunces (display, 610 to 680), IBM Plex Sans (body, 500 for leads), IBM Plex Mono (labels, 500). All self-hosted woff2. Muted text sits at ink2, never lighter, small mono never under 18px.
- **Motion language** (the point of this deck):
  * each slide auto-plays its beats in order, about 780ms apart, then rests complete
  * first press of next while playing completes the slide, the next press moves on
  * typing = mono terminals with block cursor, one typo-and-fix moment for realism
  * diagrams draw themselves (`stroke-dashoffset`), staggered at ~75% of the previous segment
  * traveling dots ride the real paths (`offset-path`, same coordinates as the SVG)
  * ambient: bounded glow bloom, slow orbiting mark, caret blink
  * prefers-reduced-motion and `?still=1`: everything lands instantly, no waits

## Story arc (14 slides)

1. Title: CV4, typed tagline
2. The problem: your AI forgets everything
3. The idea: memory is a folder, not a feature
4. Bring your own agent
5. Two movements: recall and record (diagram)
6. A day with CV4 (timeline)
7. The two layers: companion and work (nested diagram)
8. What is in the box (folder list)
9. The ladder: hotlist, library, sub-skill, skill
10. Spec-driven by design (dark: terminal + pipeline + converge)
11. Proof: self-test + release rail (real versions)
12. Start in one line (dark: message to your agent)
13. Enrollment: three questions, then it exists
14. Close: memory is the product

## Gates (mechanical, before any push)

1. `tools/design-stack/preflight.sh` PASS (zero em/en dashes, no prose spaced hyphens, no generic fonts, favicon present)
2. Screenshot pass: every slide, desktop + phone, LOOK at them, fix, re-shoot
3. Smoke test: keyboard walk through all slides, zero console errors
4. Print check: one slide per page, no clipped content
5. Offline check: zero external requests

## Sanitization rules

- Only public facts: CV4 repo content, its changelog, its own README text.
- Mock names only (the companion in the story is "Mira"); no real people, no private numbers.
- No em-dashes anywhere (house copy filter). Prose uses colons, commas, middle dots.
