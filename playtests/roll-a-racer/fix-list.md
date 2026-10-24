# Roll a Racer: playtest fix list

Playtest 2026-10-24 by Naz, alt account (fresh save), PC, played through Area 1 to Sandy Shores.
Hand this whole file to the roll-a-racer project. Prompts at the bottom are grouped into batches so each one is a sensible single task.

Severity: **P0** = kills the fun or makes players quit, **P1** = hurts retention or revenue, **P2** = polish.

## The verdict in one line

The best moment in the game is the boss race (chase cam, passing cars), and the worst is the normal race, which is supposed to be the core. Fix the race first; everything else is polish on a loop that isn't fun yet.

## Fix table

| # | Sev | Area | What's wrong | Suggested fix |
|---|-----|------|--------------|---------------|
| 1 | P0 | Race / camera | Normal races use a high top-down camera. It feels distant and not fun. The boss race chase cam is great. | Use the boss race chase cam (low, behind the car, slight FOV kick on boost) for every race. |
| 2 | P0 | Race / track | Tracks are tiny, a lap takes about 5 seconds, and they look bad. | Bigger tracks per area (30 to 60s laps), real turns that reward drifting, themed to the area. |
| 3 | P0 | Race / flow | About 8 seconds of waiting before a race starts. | Cut to 3s countdown. If you keep a wait for multiplayer, give it a job (rocket-start minigame, see ideas). |
| 4 | P0 | FTUE / flow | Tutorial sends the player to Garage and the Skill Tree before they've raced. Lots of walking from plot to race area. | FTUE = roll, buy, place, then straight into a race. Defer Garage and Skills to contextual prompts later. |
| 5 | P1 | Race / controls | Drift is not explained on PC. No key shown. | Show a key hint (Shift / Space icon) on the HUD on PC, the button on mobile. Teach it on the first corner of the first race. |
| 6 | P1 | Race / boss | Boss is far too easy: Naz won in 16s, boss finished in 26s. No tension. | Rubber-band the boss so it stays within 1 to 2s of the player, with a photo-finish feel. Easy to win, never feels free. |
| 7 | P1 | Race / visuals | Opponent cars are the exact same red model as the player's. | Randomize opponent body colors (or give each racer NPC a signature car). |
| 8 | P1 | Bosses | Each boss offers two choices (race and time trial). Confusing. | One prompt per boss: Challenge. Move time trials elsewhere or cut them. |
| 9 | P1 | Lighting | Too much bloom, can't see far. | Lower Bloom intensity/size a lot; check the far end of the track is readable. |
| 10 | P1 | FTUE / spawn | Player spawns to the right of the roll button, not facing it, so they walk and turn before anything happens. | Spawn 3 to 4 studs in front of the roll button, camera facing it. |
| 11 | P1 | FTUE / tutorial | Screen stays dimmed after pressing roll. Two roll panels shown at the start. | Undim the instant the step completes. Only one roll panel during the tutorial. |
| 12 | P1 | FTUE / first roll | First roll has no oomph. | First-roll cutscene: camera zooms to the panel, shake + VFX build-up, car spawns, FOV punch out, back to normal, then point to Buy. |
| 13 | P1 | Map / nav | No quick way back to base, race area or market. | Top-of-screen teleport buttons: Plot, Race, Market. |
| 14 | P1 | Map / layout | Plots are far from the race area. Too much walking even with the pad. | Pull plots and race entry close together, or put the race entrance at each plot. |
| 15 | P1 | Roll UI | Rolling a car shows name, rarity, price, but not speed or earnings. | Show Speed and $/s on the roll card, big. Speed is the fantasy; make it the headline stat. |
| 16 | P1 | Car billboard UI | Billboard above each car: black text on dark background (unreadable top bar), about 5 separate frames. | Condense into one card: name + rarity color, speed, $/s, one action. White text with stroke. |
| 17 | P1 | Store | Store uses tabs; some passes lack icons; cosmetics and odds live in the store. | One long scrolling store with section headers (Passes, Boosts, Packs, Cash). Icon for every pass. Move cosmetics and odds out. |
| 18 | P1 | Level design | Boss podium blocks the path to the wall after you beat it. | Move the podium off the path, or make it non-collidable after the win. |
| 19 | P2 | FTUE / tutorial | Tutorial frame border is yellow; highlight is on the inner part of the button, which looks off. Arrow points left of the roll button. | White border on the tutorial frame. Remove the inner-part highlight, or use a Highlight with DepthMode AlwaysOnTop on the whole button model. Re-center the arrow. |
| 20 | P2 | FTUE / buy | After buying the go-kart the panel still shows "Just bought". | Clear the panel with a short pop-out tween after purchase. |
| 21 | P2 | Skill tree | Prices only show on hover. | Show the price on every node. |
| 22 | P2 | Prompts | Native Roblox ProximityPrompts look stock. | Custom ProximityPrompt UI (Style = Custom) in the game's style. Simple, similar layout to Roblox's. |
| 23 | P2 | UI motion | Skills opens static; Build pops less than Garage. | One shared open/close tween for every menu (Garage is the reference). Skills: slight zoom in on Racer HQ, tiles settle in with a quick wave. |
| 24 | P2 | UI layout | X buttons don't sit on the header corner (Tracks, Plot Shop, Build, Locker, Garage). Build has empty space to the right of the X. | Make the X slightly bigger and anchor it to the top-right corner, overhanging the header a little, the same on every menu. |
| 25 | P2 | UI motion | Notifications (e.g. car bought) vanish instantly. | Every notification tweens out (fade + slide or pop). Nothing appears or disappears without motion. |
| 26 | P2 | Index | Text on the right detail card is small; lots of unused space. | Scale up name, rarity, "1 in 7 at your luck", shine rates, description. Fill the card. |
| 27 | P2 | Map / NPCs | Ambient racer NPCs only drive the outer edge, and clip through a building. | Random routes across the whole map, including diagonals; fix collision with buildings. |
| 28 | P2 | Map / art | Area 1 looks bland and cramped compared to Area 2. | Open up Area 1 and give it a stronger theme. It's the first impression. |
| 29 | P2 | Cosmetics | Nameplates in the Locker are good but plain. | Add animated ones: moving rainbow gradient, shimmer, rotating effects. Great cheap Robux / reward items. |
| 30 | P2 | VFX | VFX are stock Roblox sparkles and smoke. | VFX pass with the vfxskill in the boilerplate. Make 3 to 4 variations per effect (roll reveal, boost, drift sparks, win) for Naz to pick from. |
| 31 | Feature | Race | Races have nothing that mixes them up. | Mystery-box power-ups on track (see ideas.md). |
| 32 | Feature | Tracks | One small track per area. | Several themed tracks per area, each with a quirk (ice, lasers, lightning). |

## Ready-to-paste prompts

Paste one batch at a time into the roll-a-racer project. Do A and B first.

### Batch A: Make the race fun (issues 1, 2, 3, 5, 6, 7, 9)

```
Playtest feedback: the normal race is not fun, and it is the core of the game. The boss race is the most fun part because of its chase camera. Fix the race in this order:
1. Use the boss race chase camera for every race: low and right behind the car, smooth follow, small FOV kick on boost. Remove the top-down race camera.
2. Cut the pre-race wait from ~8s to a 3s countdown. If multiplayer needs a lobby wait, show the countdown with a rocket-start: pressing accelerate in the last 0.3s before GO gives a short boost; too early gives a stall.
3. Explain drift: show the drift key on the HUD on PC (and the button on mobile), and pop a one-line hint at the first corner of the first race. Make a held drift build sparks that release as a mini-boost.
4. Boss balance: rubber-band the boss so it stays within 1-2 seconds of the player for the whole race. The player should still win the first boss, but it must feel close. Currently the player wins in 16s and the boss takes 26s.
5. Give opponent cars random body colors so they don't all match the player's car.
6. Turn bloom way down so the far end of the track is readable.
Before changing track layouts, list the current tracks with lap times and propose larger layouts (30-60s laps, turns that reward drifting) themed to each area, and wait for my okay.
```

### Batch B: Cut FTUE friction (issues 4, 10, 11, 12, 19, 20)

```
Playtest feedback on the first 2 minutes. Goal: roll, buy, place, then straight into a first race, with nothing else in between.
1. Spawn the new player 3-4 studs in front of the roll button, with the camera facing it.
2. Only one roll panel during the tutorial. Undim the screen the instant a step completes.
3. Tutorial highlight: white border instead of yellow. Remove the highlight on the inner part of the button; instead put one Highlight on the whole button model with DepthMode = AlwaysOnTop. Fix the arrow so it is centered on the roll button (it currently points to the left of it).
4. First roll only: a short cutscene. Camera tweens to the spawn panel, small shake and a VFX build-up, the car spawns with a burst, FOV punches out and returns to normal, then the tutorial points to Buy.
5. After buying, clear the "Just bought" panel with a quick pop-out tween instead of leaving it.
6. Remove the tutorial steps that send the player to Garage and the Skill Tree. Replace them with contextual prompts that fire later when the player can actually use them (e.g. first time they can afford a skill).
7. After the first car is placed, point the player straight to the race and make the walk short (see map batch).
Show me the new tutorial step list before building it.
```

### Batch C: Map and navigation (issues 13, 14, 18, 27, 28)

```
Playtest feedback on the map:
1. Add top-of-screen teleport buttons: Plot, Race, Market. Short fade transition.
2. Plots are too far from the race area; players want to drive immediately. Propose a layout that puts race entry within a few seconds of every plot (or an entrance at each plot). Show me before moving things.
3. After beating a boss, its podium blocks the path to the wall. Move it off the path or make it non-collidable after the win.
4. Ambient racer NPCs only drive the outer edge and clip through a building. Give them random routes across the whole map, including diagonals through the middle, and avoid buildings.
5. Area 1 looks bland and cramped compared with Area 2. Suggest how to open it up and give it a stronger theme; it's every player's first impression.
```

### Batch D: UI cleanup and motion (issues 15, 16, 21-26)

```
Playtest feedback on UI. Keep the current art style, make it cleaner and more alive:
1. Roll card: show Speed and $/s prominently, not just name, rarity and price. Speed is the headline stat.
2. Car billboard above each placed car: currently ~5 frames and a top bar with black text on a dark background. Condense into one card: name in rarity color, speed, $/s, one action. White text with a dark stroke.
3. Skill tree: show the price on every node, not only on hover.
4. Replace native ProximityPrompts with a custom prompt UI (ProximityPrompt.Style = Custom) in the game's style, similar layout to Roblox's.
5. One shared open/close tween for every menu, using Garage's pop as the reference. Build currently pops less. Skills: small zoom in on Racer HQ and tiles settle in with a quick wave.
6. X buttons: same size and position on every menu, a bit larger, anchored to the header's top-right corner and overhanging it slightly. Fix Tracks, Plot Shop, Build (empty space right of the X), Locker, Garage.
7. Notifications must animate out (fade + slide or pop), never vanish instantly.
8. Index detail card: scale up name, rarity, odds, shine rates and description to fill the empty space.
Also: audit the game for features added since the last UI overhaul that have no icon or have placeholder UI, and give me a list with a one-line art prompt per item I can hand to an image generator.
```

### Batch E: Store and cosmetics (issues 17, 29)

```
Playtest feedback on monetization UI:
1. Replace the tabbed Robux store with one long scrolling list with section headers: Passes, Boosts, Packs, Cash.
2. Every game pass needs its own icon. List the ones missing one, with an art prompt each.
3. Move cosmetics (nameplates etc.) out of the store into the Locker, and move odds out of the store.
4. Nameplates: propose animated variants (moving rainbow gradient, shimmer sweep, rotating/pulsing effects) as earnable rewards and a few Robux ones.
```

### Batch F: VFX pass (issue 30)

```
The game's VFX are stock Roblox sparkles and smoke. Using the VFX skill in .claude/skills, make 3-4 variations each for: first roll reveal, rare roll reveal, boost, drift sparks, race win. Show me each set so I can pick. If you want to use Creator Store VFX packs, list them for me to review first; don't insert or upload anything without my okay.
```

### Batch G: Power-ups and themed tracks (issues 31, 32)

See ideas.md for the design. Hand it over after Batch A, because power-ups on a 5-second track won't work.
