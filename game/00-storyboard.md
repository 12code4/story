# NIGHTWARD — Game Storyboard

**Genre**: 2D expedition narrative (side-view). **Status**: for review — approval gates
pre-production. A visual version of this document (drawn panels) is published as the
"Nightward Storyboard" artifact; this file is the versioned source of truth.

Scoping note: this storyboard covers the **game grammar** (every screen type), the
**vertical slice** (Chapter 1, frame by frame), and the **act-level flow** of the whole book.
Full per-chapter storyboards are a pre-production/production activity, done chapter by chapter
with the frame template used here — same cadence as the writing.

---

## 0. The shape of the game

One sentence: *The Oregon-Trail skeleton wearing The Banner Saga's coat, about walking into
the dark politely.*

- **One perspective everywhere**: side-view 2D (travel, camps, towns, set-pieces). One art
  system, no perspective rework, parallax does the depth.
- **Heat is the master resource**: one flame meter for the expedition. Cold drains it; stoves,
  lamps, and towns restore it; several systems (trade, morale, events) price things in it.
- **The story mounts onto a loop**, it doesn't fight it: authored chapter beats trigger on
  route nodes, camps, and thresholds. Writing more chapters = making more game.
- **Player character**: Iyo. The party is authored (no recruitment system); party members are
  verbs (Brakes = repair, Solene = radio, Adder = security, Cistern = care) and scenes.

## 1. The core loop

```
        commit a leg                 events interrupt
  ROUTE MAP ──────────▶ TRAVEL ───────────────▶ ENCOUNTER
      ▲                    │                        │
      │                    ▼ arrive                 │ resolve
      │                 NODE: CAMP or SETTLEMENT ◀──┘
      │                    │  (talk / stove / radio / manifest / quests / sleep)
      └────────────────────┘  walk on
```

Chapters are authored sequences threaded through this loop; Parts change the map, the
weather table, and which systems bite hardest.

## 2. Screen grammar (the 8 screens)

Each screen listed as: WHAT YOU SEE / WHAT YOU DO / WHAT IT TEACHES.

**G1 — The Route Map ("the Line").** Hand-inked map strip; nodes (camps, stations, towns);
the traveled line drawn behind you, the plotted line dashed ahead; part title and day count.
Readouts: flame, supplies, souls. / Choose and commit the next leg; review party; read the
season-book. / Distance is a decision — every leg is priced in heat and days.

**G2 — Travel.** Side-scrolling caravan: parallax terrain, weather, Kettle's stove-glow (the
warm center of the screen), party walking in file, Tapper at flank. Ambient event toasts;
flame ticks down; barks fire. / Walk with the caravan (pace: push/steady/rest), trim lamps,
respond to events (investigate / press on). / The journey is the game; warmth is a broadcast
— brighter is safer *and* more visible. (Late game inverts the meaning without changing
the mechanic.)

**G3 — Camp.** Fixed diorama: stove at center, its light-radius drawn as an actual ring;
party members at their spots; the dark past the ring is *rendered*, not implied. Verb bar:
TALK / STOVE / RADIO / MANIFEST / WATCH / SLEEP. / Spend the evening: character scenes,
fuel choices, watch roster, then sleep to advance. / Everything warm is kept warm by hands;
scenes are the reward for spending resources on people.

**G4 — Settlement.** Roamable side-view street(s): facades, doors, window-lamps, NPCs,
notice boards, market stalls (Saltcamp prices heat by the hour and the UI shows the paid
zones). / Explore, take side quests (Manifest names), trade, trigger chapter beats. /
Towns are heat economies with manners; each town's lighting *is* its politics.

**G5 — Encounter / Dialogue.** Lower-third dialogue over the dimmed scene; portrait, name,
choices. No skill checks, no dice — choices are moral/informational, in the book's grammar.
Returner dialogue obeys the speech rules (never lie, never answer *why*, only ever ask
invitations) — the player learns the grammar by ear, and the game never annotates it. /
Choose what to say and what to ask; asking *why* of a returner is always available and never
works. / Language is the horror surface.

**G6 — Recovery ("the Count") — the signature verb.** A walker in the grey; the lamplight
gradient across the screen is the playing field. Stages: approach from the lit side
(positioning), speak the name (address choice), take the left hand, then walk them home
holding a breath/step rhythm — a beat bar with a drifting tempo the player must stay inside.
Failure is quiet: the rhythm slips, the hand is not in yours, the field is empty. / Hold a
rhythm under pressure while the screen and audio try to detach you from it. / The count is
care made mechanical; the game may corrupt this UI **exactly twice, ever** (ch. 12, ch. 26).

**G7 — The Radio.** Full-screen diegetic set: tuning dial, band scope, signal log, message
queue home. Nightly camp ritual; content is authored (never procedural), including the wrong
things the band sometimes carries. / Tune, hail, log; send the families' messages when
you have signal. / Listening is an act; the log is Solene's integrity, and yours.

**G8 — The Manifest of the Missing.** Book UI: carried names, tokens drawn as objects,
status lines that fill across the game (walking / returned / answered / —). Doubles as the
side-quest log; also the frame for reading paper-trail documents. / Accept names at muster,
resolve what you can, fail to resolve the rest; the endgame reads your own log back to you. /
Quests are grief with bookkeeping.

**HUD (persistent, minimal)**: flame meter, supply chips, day counter, party strip (small
portraits; frost creeps on the strip as members suffer). Everything else diegetic.

## 3. Vertical slice storyboard — Chapter 1, "The Cold-Line"

Ten frames, one playable shift. Each frame: BEAT / INPUT / TEACHES / AUDIO.

- **F1 — The window.** Title screen is a house interior: a window, a lamp in it, the dark
  beyond. "NIGHTWARD" stenciled like a freight label. / Unlatch the door to begin. /
  The menu is the theme. / Room tone, wind under the door, the latch.
- **F2 — Cold open, mid-recovery.** No menu-to-gameplay seam: the player is already holding
  Duna's hand on the line, count bar live. / Hold the rhythm (tutorial by doing; generous
  window). / The signature verb, before any context. / The count spoken under breath; boots;
  her bare feet in snow (wrongness in the foley, not the text).
- **F3 — Walking her home.** The line's geography scrolls past: lamp-posts and their halos,
  the berm, moths at the lights. / Keep the rhythm to Post 9; small drift events. / The
  light gradient = the safety gradient; moths = ambient normalcy (their absence will be a
  signal the game never flags). / Count continues; moth flutter; distant bell marking shift
  time.
- **F4 — Post 9 hand-off.** The post hut; Duna's family; the lamp-log. / Dialogue (first
  choices); log the recovery; read the wick-hours column (6.4 and climbing). / Dialogue
  screen; the world's quiet data (the thinning light) planted as furniture. / Family voices
  low; the log's pen scratch.
- **F5 — The long leg.** Iyo alone; wider lamp spacing; her father's culvert, Maren's bend —
  landmarks with no prompts, no codex, one-line barks if the player stops at them. / Walk;
  idle triggers Iyo counting lamp-posts under her breath. / Environmental storytelling; the
  count as *her*, not as UI. / Wind; her voice small; the lamps' oil hiss.
- **F6 — The bell at Post 11.** A double ring that fits no code (the ringer unsure); the
  last lamp; the dark field beyond, and something far out in it. / Choose to step past the
  last lamp (flame meter visibly dips as you leave the halo). / Leaving light has a price
  the HUD states plainly; courage is spending heat. / The hesitant bell; then no wind at
  all (silence as event).
- **F7 — Inbound.** A figure walking *toward* the light, steady, unhurried. / Approach from
  the lit side (the game validates the linewalker discipline silently — position matters). /
  Reuse of the recovery approach, wrong direction; the rote has no page for this and the UI
  offers no verb. / Footsteps in crust, arriving at a walking pace that never changes.
- **F8 — Elo.** He stops at the correct distance and waits. Dialogue: courteous, truthful;
  asks for Warrant Officer Kiln, by rank; "You're the one who counts. Good." / Talk; the
  [ask why] option exists, is chosen by everyone, and returns the first taste of the
  grammar (he declines, kindly). / Returner speech rules, live. / His voice: ordinary. That
  is the design note in full — ordinary.
- **F9 — The walk back.** Two figures homeward; the count bar's slot is empty — he is not
  being recovered, and the missing UI is the storytelling. / Just walk; no inputs asked. /
  Absence as dread; the game withholding its own mechanic. / Under her breath count — and
  under his, half a step ahead. (Audio-only beat. Never referenced.)
- **F10 — The gate.** Hearthfall's gate at shift's end; warmth; the Manifest board with its
  papers; title card: BOOK ONE — THE WALKED. / Log the shift; slice ends (or continues to
  ch. 2's hub in production). / The hub tease; the loop's home node. / The city's Hum —
  first time; the sound of normal.

**Slice acceptance test**: a cold player finishes one shift, can articulate "hold the count,
stay in the light, heat is spent to act," and reports the F9 audio beat unprompted in at
least some playtests. If F9 lands, the game works.

## 4. Act-level flow (the whole book on the loop)

- **Part I (chs. 1–6) — Learn the light.** Hearthfall hub + cold-line tutorial shifts +
  mustering quests (each recruit = a small errand teaching their verb). Ends: departure,
  first camps, moth-silence. Dominant screen: settlement/camp. Systems taught: all, gently.
- **Part II (chs. 7–12) — The Reach.** Route-map legs + Saltcamp hub + three spoke dioramas
  (Lighthouse 9 = crafting set-piece; Cinder Row = no-combat schedule-town; Glass Fields =
  toll negotiation and the first grave). Ends: Reachgate, rotation, failed recovery
  (count-lie #1). Dominant: route map + settlement. Systems peaking: trade, Manifest.
- **Part III (chs. 13–18) — The Sea.** Linear gauntlet, no towns: ice-song navigation,
  radio ritual, the Anchorage cable-walk, the one-room storm (all-cast chamber scene), the
  Lead bridge build, Ghost. Ends: Farside lights. Dominant: travel/camp. Systems peaking:
  heat, watch, radio. (Kettle's loss converts the camp system mid-part: warmth becomes
  carried.)
- **Part IV (chs. 19–23) — Night Country.** Farside hub (town sim inverted: everything home
  fears is furniture) → the Approach (verbs stripped; weapon/tool wheel disabled by design)
  → the Errand (census payoff: every resolved Manifest name renders at a station) → the
  Question (the game's one authored ending-choice) → Tapper's NO. Dominant: settlement/
  dialogue. Systems peaking: Manifest, dialogue grammar.
- **Part V (ch. 24) — The Return.** The same map walked home with changed world-state
  (serviced bridge, dressed grave, lit lighthouse, waived tolls; survival systems
  consciously relaxed — the absence of pressure as unease). Ends: Lantern relit (the
  audiovisual budget's one blowout).
- **Coda (chs. 25–26) — The accounting.** Door-to-door (the player's own quest log read
  back), then one last shift on the line with the new rote, Elo's wave, and the walk home
  that counts one high (count-lie #2). Credits from inside the house, looking out.

## 5. Storyboard conventions (for future per-chapter boards)

Frame template: **BEAT / INPUT / TEACHES / AUDIO** (+ optional SEE sketch). One frame per
player-facing beat; 8–14 frames per chapter; side-quest chapters get their own boards.
Count-UI corruption budget: 2 uses total, already allocated (chs. 12, 26). Jump scares: 0,
enforced at review. The dark is never rendered as a creature; the Benthos gets one silhouette
(ch. 16) and no bestiary entry.
