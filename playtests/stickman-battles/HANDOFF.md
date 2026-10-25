# Stickman Battles: handoff from the masterguide project (2026-10-25)

Paste or upload this file first. It sums up a playtest + planning conversation. The other files in this folder have the detail:

- `notes.md`: what the game is today, what works, what doesn't
- `fix-list.md`: 12 fixes with severity + paste-ready prompt batches (A: controls and feel, B: first minute, C: look and lobby)
- `differentiation.md`: how to stand apart from Stick Wars
- `questions.md`: questions for Naz (Part 1) and for you to answer about the code (Part 2)
- `../../competitors/stick-wars.md` + screenshots: what the competitor does well
- Screenshots: `meet-your-stickmen.png`, `arena-lobby-view.png`, `match-hud.png`

## Context

Stickman Battles is ~80 to 90% done. A game with the same premise, Stick Wars, shipped first and has ~2,000 CCU. Naz playtested his game on a fresh alt next to Stick Wars. Goal: polish, and a clear reason to play this one instead.

## Where the decisions landed (latest wins)

The plan moved a lot during the conversation. Current direction:

1. **Matches: side-view.** Stickmen run, jump, dodge, block and slash on a stage with platforms and little walls, no more circles/balls. Reason: side-view is much easier to read when spectating other players' matches. (Naz also said he likes circular shapes again; confirm whether that means the match arena or only the map.)
2. **Aim: click-and-drag** instead of mouse-follow + lock-aim button.
3. **Every player has their own home base** on a circular map. Everyone's stickmen auto-battle CPU opponents at their base, earning XP and passive cash (less than PvP), and other players can see those battles.
4. **The center of the map** has the duel pads and crates.
5. **Look: lighter.** The current map is too dark and too neon. Brighten it; neon as accents only.
6. **Real PvP pays more** than the base: more cash, plus better rewards (rank, crate keys, exclusive items).
7. **First minute:** much less text; MM2-style 3-strip roll reveal for the first three stickmen; a more polished pick-your-stickman screen.
8. **UI:** custom art (Naz generates it), replacing the generic look.
9. **Keep:** how matches play out, the class triangle (Brawler > Trapper > Shooter > Brawler), slow-mo on match point, Rival Road.

## Still open (ask Naz)

- Bases in a ring around the edge with duel pads + crates in the center?
- Base size (small stage vs buildable) and players per server (6 or 8)?
- What's on a base besides the auto-battle (stickmen display, upgrades, stats)?
- How to spectate (walk up to bases? big screens in the center for PvP?)
- Auto-battle: whole squad or one stickman, and what CPU they fight?
- Reference game for the lighter colors?
- Spawn at your base with a teleport-to-center button?
- Twist ideas not yet picked: squad of 3 with mid-match swapping, King of the Neon event (winner stays on), crowd powers, arena modifiers, weapons as their own collection, 2v2.

## First step for this project

Answer Part 2 of `questions.md` about the current code (don't change code yet), then work through the open questions above with Naz before running the fix-list batches.
