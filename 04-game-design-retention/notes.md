# Game design, FTUE and retention: Naz's notes

Brain dumps, playtest observations and your own rules for this topic. Newest first.

## 2026-10-24 (from Roll a Racer playtest, see playtests/roll-a-racer/)

- The verb in the title must be the most polished thing in the game. Roll a Racer's racing was the weakest part; the best moment was a side mode (boss race).
- Camera sells the fantasy. A chase cam right behind the car beat a top-down race view by a mile.
- Every wait needs a job. An 8s pre-race wait should be a rocket-start minigame or cut to 3s.
- A boss you beat by 10 seconds is not a boss. Rubber-band so it ends close; win easily, never feel free.
- One interaction = one choice. Two options on a boss (race vs time trial) is complexity, not depth.
- Friction audit for FTUE: spawn facing the first button, no leftover dim, one panel, no detours to menus the player can't use yet, short walk to the main action.
- Simple to play, with elements that change every round (power-ups, track quirks). Without variation the loop is solved in one lap.
- Nothing static: every menu opens with the same tween, every notification animates out, no hard pops.
- UI consistency: X buttons in the same corner on every menu; readable text (no dark on dark); show the stat the fantasy is about (speed) where the player gets the item.
- Custom ProximityPrompt UI is a cheap, big polish win over native prompts.
- Check the map with players in mind: no podiums blocking paths, ambient NPCs that use the whole map and don't clip.

## 2026-10-24 (from Fake an Egg, see competitors/fake-an-egg.md)

- Pre-point the camera at the next tutorial goal so the player never searches for it.
- Teach the premise with a short cutscene, not text.
- Right after the tutorial, offer a rebirth the player already qualifies for, with a reward.
- Right after the tutorial, prompt an RSVP to the next event (native Events UI).
- Give a free item on a short timer at spawn (3-minute egg) so players stay to see the result.
- Keep Beam arrows on the next goal after the tutorial ends.
- Juice every small thing: hatch zoom + shake, VFX + SFX on buy/pickup, pop-in tween on $/s labels.
- Never make a core step depend on another player choosing to act. Always have an NPC or timeout fallback.
