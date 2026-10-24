# /design-loop — Core Loop & High-Retention Gameplay Architect

Use this command to engineer core game loops, onboarding flows, and progression balancing engineered for maximum Average Session Time and Day-1 (D1) retention.

## Command Execution Workflow
When the user invokes `/design-loop [Game Type / Feature Details]`:

### Step 1: The Core Loop Architecture
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

### Step 2: The First-Time User Experience (FTUE) Blueprint
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

### Step 3: Contextual Tutorials (Post-90 Seconds)
Never dump advanced systems upfront. Defer tutorials until the exact moment of player need:
- *Trigger 1*: Player cash reaches 0 or inventory fills up $\rightarrow$ fire mini-prompt showing upgrade path.
- *Trigger 2*: Player plot reaches maximum capacity $\rightarrow$ fire prompt showing how to expand plot.
- *Trigger 3*: Player runs out of consumable resource (food, fuel, ammo) $\rightarrow$ fire prompt pointing to the resource shop.

### Step 4: Progression Pacing & Milestone Balancing
Map out the exact timeline for a player's first 15 minutes:
- **Minute 1**: First minor upgrade / purchase (cost: low, reward: immediate visual jump).
- **Minute 2.5**: Common drop-off zone. Ensure an exciting milestone or "wow moment" hits right here (e.g., first pet feed makes it grow 5x larger than normal).
- **Minute 5**: First new zone or tier unlocked.
- **Minute 10**: Transition to mid-game loop; introduce social competition / leaderboards.
- **Funnel Milestone Tracking**: Define explicit backend tracking events:
  * `join` $\rightarrow$ `tutorial_step_1` $\rightarrow$ `tutorial_step_2` $\rightarrow$ `first_purchase_open` $\rightarrow$ `first_purchase_complete` $\rightarrow$ `zone_1_enter`.
  * Track individual button clicks (e.g. `open_gear_shop` $\rightarrow$ `bought_bat` $\rightarrow$ `closed_gear_shop`) to isolate UI drop-offs.

### Step 5: Sunk Cost & Social Retention Hooks
Integrate psychological retention drivers:
- **Sunk Cost Fallacy**: Give players customizable bases, plots, or pet collections where effort invested creates emotional attachment that prevents churn.
- **Social Flex**: Ensure high-tier progress is instantly visible to other players in the server (glowing titles, giant base structures, rare block skins, chat broadcast messages).
- **Free Private Servers**: Allow players to build or farm in peace without griefing, driving word-of-mouth friend invites.
