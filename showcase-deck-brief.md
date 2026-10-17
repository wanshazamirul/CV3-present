# CV3 Showcase: Deck Brief (Japan team presentation)

> **Status: shipped** · brief from 2026-10-16 · kept with the deck; the companion design doc lives in the CV4 (COGNITIO-SKELETON) repo under `docs/enterprise-edition.md`

## Goal & audience

Show the team **what CV3 is, how it runs daily, what the enterprise edition looks like**, and invite a pilot.
Audience: their dev team (maybe leadership). Markdown/AI-pragmatic culture → **evidence-first, structured, not salesy.**

## Format

- Self-contained folder with `index.html`; Wan opens it, presents with keyboard nav, works **offline** (this repo).
- Print stylesheet → **export to PDF** straight from the browser (1 slide per page).
- Optional: **PNG export per slide** via our screenshot tool (drop into any doc/tool).

## Story arc (chapters)

1. **Hook**: "Your knowledge walks out the door every Friday."
2. **What CV3 is**: a protocol, not an app: persona + memory + skills + review loops.
3. **A day with CV3**: timeline with real (sanitized) samples.
4. **The engine**: auto-capture, memory layers, continuous improvement, the guard-catch proof.
5. **Skills**: SKILL.md standard, Claude Code native, suggested-not-forced catalog.
6. **Live artifacts**: sanitized screenshots of the running system.
7. **CV3 Enterprise Edition**: trust layers, concurrency doctrine, init interview.
8. **Their stack mapping**: Azure DevOps + Pipelines + Static Web Apps, and JP/EN handling.
9. **Roadmap + pilot ask**: P1→P4, one team, two weeks.
10. **Close**: the invitation.

## Slide list (~18)

| # | Slide |
|---|-------|
| 1 | Title |
| 2 | The problem (knowledge dies between projects; AI gives chat, not memory) |
| 3 | CV3 in one picture (protocol diagram) |
| 4 | A day with CV3 (timeline visual) |
| 5 | Auto-capture: a real log block writes itself |
| 6 | Memory layers: hot/warm/cold rotation diagram |
| 7 | Continuous improvement: observe → review → trust order |
| 8 | The guard catch: "we audit ourselves" proof story |
| 9 | Time-aware & continuity: greeting/recency examples |
| 10 | Care & companionship: sanitized, care-dial framing |
| 11 | Skills & hats: SKILL.md sample + catalog |
| 12 | Live artifacts: brain viz, fleet, search (sanitized screens) |
| 13 | Enterprise: trust layers |
| 14 | Enterprise: concurrency doctrine (one file, one writer) |
| 15 | Enterprise: init interview, name your AI |
| 16 | Their stack: Azure mapping |
| 17 | Roadmap + pilot ask |
| 18 | Close |

## Art direction options (pick one)

- **A. Zen Blueprint (recommended)**: light washi-paper cream, ink navy + vermilion accent, thin precise technical line diagrams, generous whitespace (*ma*), print-quality. Reads like a beautifully bound spec; fits a Japanese corporate room, prints great to PDF, ages well.
- **B. Mission Control**: near-black slate, OKLCH teal + amber, monospace data accents, glowing wireframe diagrams, terminal snippets. Engineers will grin; less "formal handout".
- **C. Cosmic Brain**: deep space gradient, orbital/planetary visual language (matches our brain viz), subtle motion, dramatic hero. Most memorable, most showy.

*Hybrid allowed, e.g. Zen Blueprint base with one dark "living system" chapter.*

## Assets & sanitization rules

**Use (real, with scrubbing):** a log block sample · the guard-catch story · HOTLIST sample · a SKILL.md sample · brain viz screenshot · review-loop diagram, all rebuilt from our live system.

**Scrub:**
- ❌ no phone numbers, tokens, server IPs/paths
- ❌ no real names; family/friends → roles ("a family member", "a fleet user")
- ❌ no health specifics
- ⚠️ brain-viz screenshot → crop/blur logs or rebuild as clean mock

Where a screenshot would leak private content, rebuild it as a **styled mock with realistic-but-fake data** (same look, zero exposure).

## Build approach

- Standalone HTML folder (`index.html` + `assets/`), offline-safe (system fonts or embedded, no CDN dependency).
- Diagrams as **hand-polished inline SVG** (from the design doc mermaid flows).
- Minimal JS: keyboard nav, progress, subtle motion. Chart.js vendored locally only if a chart earns its place.
- Iterate visually with our screenshot tool before hand-off; verify print → PDF path.
- JP accents: key terms bilingual where useful (記憶 / memory, ガードレール / guardrails, 改善 / kaizen), sparing.

## Open before build

- **Art direction pick** (Wan): A / B / C.
- Language mix: EN core + JP glossary assumed unless told otherwise.
- Include the audit chapter? Recommend **yes**: "we audit ourselves" is trust material.
