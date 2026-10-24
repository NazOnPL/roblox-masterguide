# /monetize — High-Conversion Roblox Monetization Architect

Use this command to structure Developer Products, Game Passes, and conversion purchase pathways engineered to maximize Payer Conversion Rate (PCR), Average Revenue Per Paying User (ARPPU), and 7-Day Spend Days Per User.

## Command Execution Workflow
When the user invokes `/monetize [Game Economy / System Details]`:

### Step 1: Core Monetization Principles
- **The Customer is Usually Right**: Prioritize sustainable gameplay over predatory pay-to-win. Excessive P2W kills CCU and ruins game longevity.
- **Solve Real Frustrations**: The bestselling products always solve direct player pain points:
  * Pain of Effort / Time: Speed boosts, instant hatch, offline collection boosters.
  * Pain of Loss / Raiding: 24-hour base protection locks against AFK griefing.
  * Pain of Status: Limited-stock flex items (RGB antennas, exclusive titles).
- **Never Sell Game-Breaking Economy Crashers**: Avoid direct massive cash packs or unmetered auto-grinders that allow players to finish all content in 3 hours.

### Step 2: The Consumable-First Engine (Driving 7-Day Spend Days)
Game Passes are one-time payments. Consumable Developer Products generate recurring revenue and drastically pump the algorithmic **7-day spend days per user** metric:
- **Temporary Protection**: e.g., 24-Hour Base Lock (purchased daily by active players).
- **Offline Multipliers**: e.g., 2x Offline Earnings prompt triggered when collecting accumulated currency (19 Robux).
- **Session Consumables**: Instant hatching, luck potions (15 minutes), instant teleports, raid shields.

### Step 3: The 3-Tier McDonald's Pricing Model ("Small, Medium, Large Fries")
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

### Step 4: The 3+ Purchase Pathways Architecture
Never hide products behind a single static shop menu. Implement at least three purchase pathways:
1. **Pathway 1 (HUD Access)**: Standard clean shop icon in screen GUI.
2. **Pathway 2 (Inline '+' Buttons)**: Direct '+' button positioned right next to the currency/stat display in the HUD.
3. **Pathway 3 (Smart Error Trigger / Contextual Prompt)**:
   - When a player attempts to purchase an in-game item with insufficient funds:
     * Attempt 1: Subtle warning ("Not enough cash").
     * Attempt 2: Subtle warning.
     * Attempt 3: Contextual popup opens the cash shop directly with the exact missing amount highlighted.
     * Safety Cap: Limit this error prompt to 3–5 times per play session to prevent user annoyance.
4. **Pathway 4 (Physical Points of Interest - POI)**:
   - Place physical prompt parts directly in high foot-traffic world areas (e.g., place the 24-hr lock prompt right at the base front entrance where players walk every session).

### Step 5: Deliver the Monetization Catalog
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
