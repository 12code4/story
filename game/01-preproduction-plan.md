# NIGHTWARD — Pre-production Plan (for approval)

**Gate discipline**: each phase ends at a review you approve before the next begins. No dates
— gates, not deadlines (solo cadence). This document is the thing to approve/amend; the
storyboard (`game/00-storyboard.md` + the published visual page) is its exhibit A.

---

## Phase A — Storyboard *(this deliverable — you are here)*

**Contents**: game shape + core loop, the 8-screen grammar, Chapter 1 slice in ten frames,
act-level flow, storyboard conventions for future chapters.

**Gate A (your review)**: approve the shape, or amend. The five decisions below are part of
this gate — each has a recommendation so a plain "approved" is enough to proceed.

### Decisions at Gate A

1. **Engine/tech** — *Recommended: TypeScript + PixiJS + Vite (web-first).* Runs in any
   browser, zero install for playtests, best fit for this vibe-coding workflow (I can build,
   run, and screenshot it in-session; every playable build is shareable as a URL/file).
   Alternative: Godot 4 — stronger editor tooling and native export, but iteration here is
   headless/clunkier and playtests need downloads. Web-first does not foreclose Godot later;
   the data format (below) is engine-neutral on purpose.
2. **Art direction** — *Recommended for the slice: silhouette-and-lamplight vector* (dark
   shapes, one warm light system doing the atmosphere; cheap to produce, hides asset-count
   weaknesses, matches the fiction's restraint). Candidates to test as style frames in
   Phase B: (a) silhouette vector, (b) two-tone pixel art with a light shader, (c) painted
   parallax (Banner Saga register — expensive; only if the style frame stuns us).
3. **Perspective** — *Recommended: side-view everywhere* (one art/traversal system; towns as
   street elevations). Alternative: top-down for settlements only (more spatial freedom,
   second system to build and art).
4. **Text volume** — *Recommended: terse dialogue + rich ambient barks* (book-flavored, but
   screens carry ≤3 short lines at a time; long-form prose lives in the paper-trail
   documents, which are diegetic reading).
5. **Slice scope** — *Recommended: Chapter 1 only, all ten frames, end-to-end.* Alternative:
   Ch. 1–2 (adds the Hearthfall hub early; roughly doubles slice cost for a question the
   slice doesn't need to answer yet).

## Phase B — Pre-production (target: a playable greybox slice)

Order matters; each step is independently reviewable.

1. **B1 — The Count prototype first.** The signature mechanic, feel-tested in isolation
   (rectangles and a metronome). Make-or-break: if holding the rhythm isn't quietly tense in
   a grey box, we redesign the verb before building anything around it.
   *Exit: you play it in a browser and it feels like care under pressure.*
2. **B2 — Data format + pipeline.** Engine-neutral content schema: chapters as structured
   scene scripts (JSON/YAML) with beats, dialogue, events, and triggers — authored to be
   generated *from* the book's chapter files, so writing and building stay one workflow.
   *Exit: Chapter 1's treatment exists as machine-readable scenes; a validator passes it.*
3. **B3 — Greybox slice.** All ten frames playable end-to-end with placeholder art (shapes,
   stand-in text, real audio stubs): title-house → recovery → line walk → Post 9 → long leg
   → bell → inbound → Elo dialogue → walk back → gate.
   *Exit: the slice acceptance test from the storyboard (F9 lands unprompted).*
4. **B4 — Style frames.** Three stills (travel, camp, recovery) in the candidate art styles;
   pick one. *Exit: art direction locked with a one-page style bible (palette, light rules,
   silhouette rules).*
5. **B5 — Audio sketch.** The slice's soundscape: wind bed, lamp hiss, boots, the count
   voice, the bell, room tone. Audio is this game's horror budget; it gets a real pass even
   in greybox. *Exit: the slice plays with sound on and the F6 silence beat works.*

**Gate B (slice review)**: you play the greybox slice with sound. Question on the table:
"does one shift on the line feel right?" Approve → production; amend → we iterate inside
Phase B.

## Phase C — Production (chapter-by-chapter)

The writing workflow and the build workflow merge: refine a chapter's treatment → generate/
author its scene script → build its frames → dress its art/audio → review. Cadence: one
chapter (or one hub) per cycle, in book order, because systems accrete in book order by
design. Part milestones = playable act builds (Part I build, Part II build, …).

Standing production rules (from the story bible, enforced at review):
- No jump scares; the dark is never a rendered creature; no bestiary.
- Count-UI corruption: 2 uses total (chs. 12, 26), already allocated.
- Discontinuity events: hand-authored, ≤4 per playthrough, never acknowledged by any system.
- Human factions stay human; no lore-dump collectibles about the truth (deferred-mysteries
  policy applies to the game harder than the book).

## Out of scope until after Gate B (parked, deliberately)

Save-system polish beyond autosave, options/accessibility menus (beyond volume + text size,
which ship in the slice), localization, controller support, performance targets beyond
"runs in a laptop browser," and anything Book Two.

## Risks (named now so they don't surprise us)

- **The Count doesn't feel good** → B1 exists to catch this first; fallback designs: breath-
  hold timing (single key held/released) or call-and-response taps.
- **Scope creep via towns** (settlements want to become RPGs) → each town's verb list is
  fixed at storyboard time; Saltcamp is the only shop in the game.
- **Art appetite outruns the pipeline** → silhouette style is the hedge; style frames decide
  with evidence, not hope.
- **The story outruns the build** (26 chapters is a lot of game) → Part builds are honest
  shipping points: Part I alone is a complete, sellable short game ("one shift, one muster,
  one departure") if we ever want an early release.
