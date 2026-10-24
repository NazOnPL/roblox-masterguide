---
name: roblox-design-and-monetize
description: Design a Roblox core loop, FTUE and progression, and its monetization catalog and purchase pathways
---

# Roblox game design and monetization

Run Part 1 for loop, onboarding or retention questions, Part 2 for products, pricing or purchase pathways, and both for a full game plan.

# Part 1: Core loop and retention

Use this to engineer core game loops, onboarding flows, and progression balancing engineered for maximum Average Session Time and Day-1 (D1) retention.

## Workflow
Input: Game Type / Feature Details.

### 1.1 The Core Loop Architecture
Construct a closed-loop mechanical framework:
$$\text{Action} \longrightarrow \text{Sensory Reward} \longrightarrow \text{Progression Upgrade} \longrightarrow \text{Social Flex / Sunk Cost}$$

- **Action**: Must be intuitive for a 7-year-old on mobile (tap, hold, walk over pad, swing).
- **Sensory Response (Juice)**: Every single action must trigger immediate feedback:
  * Crisp sound effect (SFX) with pitch variation.
  * Subtle camera shake.
  * Dynamic visual effects (VFX): floating numbers, particle bursts, squash-and-stretch.
- **Depth vs. Complexity Check**:
  * *Complexity* = 10 convoluted sub-menus (Bad).
  * *Depth* = 1 simple mechanic that produces endless variations (Good). Examples: voxel building layouts, RNG rolling with visible teaser carousels, dynamic PvP stealing and juking.
- **Anti-Solved Strategy**: Ensure the game has dynamic elements (PvP threats, player raiding, RNG mutation, shifting center-island biomes) so the optimal strategy cannot be solved in 5 minutes.

### 1.2 The First-Time User Experience (FTUE) Blueprint
Design the onboarding sequence down to the exact second:
- **0–5 Seconds (Level Design Guidance)**:
  * Show the ultimate threat or goal immediately via level design (e.g., giant incoming tsunami, towering villain, locked laser base). Zero explanation needed.
- **0–30 Seconds (Title Promise Delivery & Cutscene Hook)**:
  * Deliver the exact promise of the title immediately (if title is *Build a Base*, start them building within 10 seconds).
  * Use a short, dynamic 3-to-5 second cutscene to drop bounce rate (proven to drop bounce rate from 22% down to 15%). E.g., showing a pet get stolen or a monster attacking.
- **30–90 Seconds (Frictionless Single-Mechanic Teaching)**:
  * Teach **ONE** mechanic at a time.
  * **Show, Don't Tell**: Let the player see direct cause and effect. No multi-paragraph text boxes.
  * Auto-equip items directly into their hotbar upon completing an action (e.g. auto-equip hatched egg/tool so players never fumble with mobile inventory menus).
  * Strip away all non-essential HUD elements during onboarding. Do NOT show cash shop packs, VIP banners, or 2x boosts during the tutorial.

### 1.3 Contextual Tutorials (Post-90 Seconds)
Never dump advanced systems upfront. Defer tutorials until the exact moment of player need:
- *Trigger 1*: Player cash reaches 0 or inventory fills up $\rightarrow$ fire mini-prompt showing upgrade path.
- *Trigger 2*: Player plot reaches maximum capacity $\rightarrow$ fire prompt showing how to expand plot.
- *Trigger 3*: Player runs out of consumable resource (food, fuel, ammo) $\rightarrow$ fire prompt pointing to the resource shop.

### 1.4 Progression Pacing & Milestone Balancing
Map out the exact timeline for a player's first 15 minutes:
- **Minute 1**: First minor upgrade / purchase (cost: low, reward: immediate visual jump).
- **Minute 2.5**: Common drop-off zone. Ensure an exciting milestone or "wow moment" hits right here (e.g., first pet feed makes it grow 5x larger than normal).
- **Minute 5**: First new zone or tier unlocked.
- **Minute 10**: Transition to mid-game loop; introduce social competition / leaderboards.
- **Funnel Milestone Tracking**: Define explicit backend tracking events:
  * `join` $\rightarrow$ `tutorial_step_1` $\rightarrow$ `tutorial_step_2` $\rightarrow$ `first_purchase_open` $\rightarrow$ `first_purchase_complete` $\rightarrow$ `zone_1_enter`.
  * Track individual button clicks (e.g. `open_gear_shop` $\rightarrow$ `bought_bat` $\rightarrow$ `closed_gear_shop`) to isolate UI drop-offs.

### 1.5 Sunk Cost & Social Retention Hooks
Integrate psychological retention drivers:
- **Sunk Cost Fallacy**: Give players customizable bases, plots, or pet collections where effort invested creates emotional attachment that prevents churn.
- **Social Flex**: Ensure high-tier progress is instantly visible to other players in the server (glowing titles, giant base structures, rare block skins, chat broadcast messages).
- **Free Private Servers**: Allow players to build or farm in peace without griefing, driving word-of-mouth friend invites.

### 1.6 Playtest Audit: Fantasy, Feel and Friction
Use this when the game already exists and Naz is playtesting it (fresh alt account). Score each item pass/fail and log every fail as severity, area, problem, fix, and a ready-to-paste prompt for the game project.
- **Fantasy Test**: Is the verb in the title (race, build, hatch) the most fun and most polished thing in the game? If a side mode is more fun than the core, fix the core first and copy what the side mode does.
- **Camera Test**: Does the camera sell the fantasy (chase cam for driving, close zoom for reveals)? A distant or top-down view kills a driving game.
- **Wait Test**: List every wait over 3 seconds (pre-race lobby, countdowns, walks). Each one is cut or given a job (rocket-start minigame, preview, tip).
- **Variation Test**: Does the second round feel different from the first? If one lap or one round "solves" it, add simple round-to-round variety (power-ups, track quirks, events) without adding menus.
- **Challenge Test**: Bosses and rivals must end close. Rubber-band so the player wins, but by a hair.
- **One-Choice Test**: Every interaction (boss, NPC, pad) offers one action. Two options = complexity.
- **Friction Walk**: Time the walk from spawn to the first action and from base to the core activity. Spawn facing the first button. Add top-bar teleports (Plot, Core Activity, Shop).
- **Motion Test**: Nothing appears or disappears without a tween. Every menu uses the same open/close animation. Notifications animate out.
- **UI Consistency Test**: Close buttons in the same corner on every menu. No dark text on dark backgrounds. No price or key stat hidden behind hover. Show the stat the fantasy is about (e.g. speed) at the moment the player gets the item.
- **Polish Signals**: Custom ProximityPrompt UI instead of native; custom VFX instead of stock sparkles and smoke; restrained bloom.
- **Level Sanity**: Nothing blocks a path after an event (podiums, doors); ambient NPCs use the whole map and never clip.

# Part 2: Monetization

Use this to structure Developer Products, Game Passes, and conversion purchase pathways engineered to maximize Payer Conversion Rate (PCR), Average Revenue Per Paying User (ARPPU), and 7-Day Spend Days Per User.

## Workflow
Input: Game Economy / System Details.

### 2.1 Core Monetization Principles
- **The Customer is Usually Right**: Prioritize sustainable gameplay over predatory pay-to-win. Excessive P2W kills CCU and ruins game longevity.
- **Solve Real Frustrations**: The bestselling products always solve direct player pain points:
  * Pain of Effort / Time: Speed boosts, instant hatch, offline collection boosters.
  * Pain of Loss / Raiding: 24-hour base protection locks against AFK griefing.
  * Pain of Status: Limited-stock flex items (RGB antennas, exclusive titles).
- **Never Sell Game-Breaking Economy Crashers**: Avoid direct massive cash packs or unmetered auto-grinders that allow players to finish all content in 3 hours.

### 2.2 The Consumable-First Engine (Driving 7-Day Spend Days)
Game Passes are one-time payments. Consumable Developer Products generate recurring revenue and drastically pump the algorithmic **7-day spend days per user** metric:
- **Temporary Protection**: e.g., 24-Hour Base Lock (purchased daily by active players).
- **Offline Multipliers**: e.g., 2x Offline Earnings prompt triggered when collecting accumulated currency (19 Robux).
- **Session Consumables**: Instant hatching, luck potions (15 minutes), instant teleports, raid shields.

### 2.3 The 3-Tier McDonald's Pricing Model ("Small, Medium, Large Fries")
Every monetization catalog must offer three psychological tiers:
1. **Tier 1: The Loss Leader / Starter Pack (5–19 Robux)**
   - Purpose: Break the psychological player-to-payer threshold. Once a player spends 10 Robux, their likelihood of returning and spending again increases exponentially.
   - Examples: Tier 1 Speed Multiplier (5 Robux), Beginner Starter Pack (19 Robux).
2. **Tier 2: The Core Value / Pro Pack (99–399 Robux)**
   - Purpose: Deliver substantial utility for dedicated mid-game players.
   - Examples: Extra plot slots, exclusive utility tools, permanent QoL enhancements.
3. **Tier 3: The Whale Sinks & Limiteds (1,000–5,000+ Robux)**
   - Purpose: Maximize ARPPU from top 1% spenders.
   - Enforce **Strict Artificial Scarcity**: Release limited stock (e.g. "Only 100 in stock"). Do NOT restock continuously. Display live remaining stock counters in the UI.

### 2.4 The 3+ Purchase Pathways Architecture
Never hide products behind a single static shop menu. Implement at least three purchase pathways:
1. **Pathway 1 (HUD Access)**: Standard clean shop icon in screen GUI. The shop itself is one long scrolling list with section headers (Passes, Boosts, Packs, Cash), not tabs, and every product has its own icon. Cosmetics live in a Locker, not the Robux shop.
2. **Pathway 2 (Inline '+' Buttons)**: Direct '+' button positioned right next to the currency/stat display in the HUD.
3. **Pathway 3 (Smart Error Trigger / Contextual Prompt)**:
   - When a player attempts to purchase an in-game item with insufficient funds:
     * Attempt 1: Subtle warning ("Not enough cash").
     * Attempt 2: Subtle warning.
     * Attempt 3: Contextual popup opens the cash shop directly with the exact missing amount highlighted.
     * Safety Cap: Limit this error prompt to 3–5 times per play session to prevent user annoyance.
4. **Pathway 4 (Physical Points of Interest - POI)**:
   - Place physical prompt parts directly in high foot-traffic world areas (e.g., place the 24-hr lock prompt right at the base front entrance where players walk every session).

### 2.5 Deliver the Monetization Catalog
Return a structured pricing table:
```markdown
# Monetization Matrix: [Game Title]
| Product Name | Type (DevProduct / GamePass) | Price (Robux) | Target Audience | Problem Solved / Psychological Trigger | Placement & Purchase Pathway |
|---|---|---|---|---|---|
| Starter Pack | DevProduct | 19 R$ | New Players | Player-to-Payer Conversion | HUD Banner (Post-FTUE) |
| 24-Hr Base Shield | DevProduct | 49 R$ | Active Players | Pain of Loss (AFK Raiding) | Entrance Door Physical POI |
| 2x Offline Boost | DevProduct | 19 R$ | Returning Players | FOMO on Offline Gains | Collection Pad Prompt |
| Whale Limited Item | GamePass/Limited | 1,500 R$ | Whales / Flex | Social Status / Scarcity (Stock: 100) | Center Island Leaderboard |
```

## Use Naz's own notes too

If the roblox-masterguide repo or the project files are available, also read the matching `notes.md` and any relevant `competitors/*.md` playtest notes and `playtests/<game>/` fix lists, and prefer Naz's own observations where they are more specific.