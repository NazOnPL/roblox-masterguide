# Stickman Battles: playtest fix list

Playtest 2026-10-25 by Naz, fresh alt, PC (Studio), compared against Stick Wars.
Hand this whole file to the stickman-vs-stickman project. Prompts at the bottom are grouped into batches so each one is a sensible single task.

Severity: **P0** = kills the fun or makes players quit, **P1** = hurts retention or revenue, **P2** = polish.

## The verdict in one line

The match is fun. What's missing is the stickman fantasy (they're stuck in balls), a first minute that shows instead of tells, and polish on every screen, because a game with the same premise is already live with 2,000 players.

## Fix table

| # | Sev | Area | What's wrong | Suggested fix |
|---|-----|------|--------------|---------------|
| 1 | P0 | Match / feel | Stickmen sit inside circles and act like balls. Doesn't feel like stickmen. | Remove the circles. Stickmen run, jump, dodge, block and slash with real animations, and the arena has obstacles to run on and around. Switch to a side-view stage with platforms and little walls (decided 2026-10-25; easier to spectate). Give it its own color identity (lighter than now, neon accents) so it doesn't read as Stick Wars. |
| 2 | P0 | Match / controls | Aim follows the mouse; clicking the lock-aim button moves the mouse down and ruins the aim. | Click-and-drag to aim (slingshot style): press anywhere, drag to set direction and power, release to launch. Remove the lock button. On mobile, same with touch. |
| 3 | P1 | FTUE / text | Too much text on the first screens ("Meet your stickmen" is a wall of words). | Max one short line per screen. Show, don't tell: the class triangle becomes three icons with arrows, no paragraph. |
| 4 | P1 | FTUE / reveal | First three stickmen just appear on a card. Stick Wars rolls them in. | First-join reveal: screen split into three horizontal strips, each spins like an MM2 crate (stickmen scroll past), they land one after another with a hit sound, shake and rarity flash. Then one line: "These are yours." |
| 5 | P1 | UI / style | UI looks generic and AI-made. | Custom UI art pass, same pipeline Naz uses on his other games (ChatGPT image prompts for buttons, frames, icons), keeping the neon theme. |
| 6 | P1 | UI / pick screen | Choosing your stickman feels flat next to Stick Wars. | Big character cards with idle animation, class color, one stat line; selected card pops forward with a tween and glow. |
| 7 | P1 | Visuals / readability | Map is too dark and too neon (Naz). Grid and glow compete with the fighters. | Brighter map lighting overall, neon only as accents; calmer floor; fighters get a bright outline in team color; glow only on arena walls and hits. Test at phone size. |
| 8 | P1 | Lobby / HUD | Check against Stick Wars: centralized PLAY + INVITE (with a free-crate tag), playtime reward bar, daily quests, timers. | Make sure the lobby has one huge Play button and Invite next to it with a reward on it. Naz isn't sure what his lobby has yet; verify. |
| 9 | P2 | Match / finish | Slow-mo on match point is great. | Keep. Add hit-stop and a quick camera punch on the final blow. |
| 10 | P2 | Assets | Studio output: `rbxassetid://203785492 failed: Asset type does not match requested type`. | Find what references that ID and use the right asset type (likely an image/sound ID mismatch). |
| 12 | Feature | Base / idle | Naz's idea: your stickmen auto-fight CPUs at your base for passive cash; PvP earns better rewards. | See differentiation.md, "your base fights for you". |
| 11 | Feature | Events | Stick Wars has a Server Brawl every few minutes with prizes. | Our own version of a server-wide event, see differentiation.md (don't clone it 1:1). |

## Ready-to-paste prompts

### Batch A: Controls and stickman feel (issues 1, 2, 9)

```
Playtest feedback on matches. The match flow is fun; keep the balance and the slow-mo on match point.
1. Aim: replace mouse-follow aim + lock button with click-and-drag aim. Press anywhere in the arena, drag to set direction (and power if relevant), release to commit. Show a trajectory/arrow while dragging. Remove the lock-aim button. Same with touch on mobile.
2. Stickmen should feel like stickmen, not balls: switch matches from top-down to a side-view stage with a few platforms and little walls. Remove the circles. Give each stickman run, jump, dodge, block and attack animations. Side-view also makes matches easy to spectate on the lobby screens. Keep neon as accents on a lighter map.
3. On the final blow, add a short hit-stop (~0.1s) and a small camera punch on top of the existing slow-mo.
Before changing movement, describe the current movement/physics system and propose how to move from top-down balls to side-view running stickmen, and wait for my okay.
```

### Batch B: First minute (issues 3, 4, 6)

```
Playtest feedback on the first minute: too much text, no excitement.
1. First join: reveal the three starting stickmen with a roll. Split the screen into three horizontal strips; each strip spins like an MM2 crate with stickmen scrolling past, then lands one after another (left to right) with a hit sound, a small shake and a rarity-colored flash.
2. Cut the "Meet your stickmen" text. Show the class triangle as three icons with arrows, one short line max.
3. Rework the pick-your-stickman screen: big cards with the stickman idle-animating, class color, one stat line. The selected card tweens forward and glows.
Show me the new first-minute flow step by step before building it.
```

### Batch C: Look and lobby (issues 5, 7, 8, 10)

```
1. Readability: the map is too dark and too neon. Brighten the lighting overall and keep neon as accents only. Calm the arena floor grid, give fighters a bright outline in their team color, keep strong glow only for walls and hits. Check at phone resolution.
2. List every UI screen in the game so I can make custom art for each one (I'll generate it). Note the size and states each button needs.
3. Lobby check: confirm there is one large central PLAY button with INVITE next to it (invite shows a reward tag), a playtime reward bar, and daily quests. List what's missing.
4. Find what references rbxassetid://203785492 (Studio says the asset type doesn't match) and fix it.
```
