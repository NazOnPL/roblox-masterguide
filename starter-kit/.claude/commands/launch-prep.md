# /launch-prep — Roblox Launch, Sponsored Ads & Packaging Engine

Use this command to prepare a game for launch, manage sponsored ad budgets, navigate the 500 Highly Engaged Players requirement, and generate high-converting AI thumbnail prompts.

## Command Execution Workflow
When the user invokes `/launch-prep [Game Name / Launch Phase]`:

### Step 1: The Sponsored Ads Launch Strategy
Follow the low-budget, high-efficiency ad blueprint:
- **Daily Budget**: **$16 / 16 Ad Credits per day** (convert Robux into Ad Credits to maximize cost efficiency; never use raw USD unless required).
- **Targeting**: Select **All Players / Recommended**. Do NOT restrict targeting manually to 18-24. Roblox automatically filters unverified games to 16+ audience during initial launch.
- **Run Duration**: Run for a minimum of **3 to 7 days continuous**. Roblox analytics pipelines have a 2-3 day reporting delay. Never panic-kill ads within 24 hours.
- **Pre-Launch Beta Mode**: Keep the game in Roblox **Beta Mode** while running initial ad batches to optimize onboarding funnels and squash game-breaking bugs before entering the public Home Recommendation algorithm.

### Step 2: The 500 Highly Engaged Players Checkpoint
Understand and conquer the platform discovery hurdle:
- **What is a Highly Engaged Player?**: A player who has completed a verified purchase anywhere on the Roblox platform within the last 60 days. They do NOT need to spend money in your specific game.
- **The Bot Traffic Bottleneck**: Sponsored ads traffic includes cold traffic and non-spending accounts. Initial progress toward 500 will feel slow (10-20 players/day).
- **The Acceleration Curve**: As your stats improve, Roblox begins testing your game in organic Home Recommendations. Once organic traffic mixes in, progress surges rapidly (from 100 to 500 in 3-5 days).

### Step 3: The Algorithmic Crossover Rule (When to Kill Ads)
- Monitor **Acquisition $\rightarrow$ Home Recommendations** vs. **Sponsored Ads Impressions** in the Creator Dashboard.
- **The Golden Rule**: The exact moment **Home Recommendation Impressions exceed Sponsored Ad Impressions**, **TURN OFF PAID ADS**.
- Let the organic discovery flywheel take over. Only resume ad spend if you ship a massive metric-focused update and need fresh cohort data.

### Step 4: High-CTR AI Thumbnail Generation System
Roblox thumbnails must be engineered specifically for mobile screens:
- **Mobile Preview Audit (The QPTr Standard)**: 80% of impressions appear on phones. Text and subjects must be readable at fingernail scale.
- **The Visual Composition Rules**:
  * **1–2 Characters Maximum**: Never crowd the scene with 5+ tiny characters.
  * **Exaggerated Facial Expressions**: Readable emotional states (evil menacing grin, crying noob, panic, troll face). Bacon hairs, noobs, and acorn hairs consistently test best.
  * **Extreme Color Contrast**: Vibrant blue sky, punchy green grass, saturated primary colors.
  * **Kill Visual Noise**: Remove background clouds, clutter, and unreadable terrain textures.
  * **Tease the Core Loop & Fantasy**: Show the dynamic verb in action (stealing, kicking, hacking, escaping).
- **Proven Thumbnail Archetypes**:
  1. *The Split-Screen Before & After*: "Level 1 Noob" vs. "Level 999 Pro".
  2. *The Action Teaser*: One character performing an action with an emotional victim in the background.
  3. *The Power Progression*: Huge base / massive weapon vs. incoming tiny enemies.
  4. *First-Person Roleplay View*: Hands holding a tool/weapon interacting with the environment.

### Step 5: Deliver Launch Checklist & Midjourney/AI Prompts
Generate custom prompts for AI thumbnail tools (RowThumbs, Midjourney, etc.):
```markdown
# Launch & Packaging Blueprint: [Game Title]
- **Target Ad Budget**: 16 Ad Credits/day ($16/day) for 7 days
- **Launch Phase**: Beta Mode Testing -> Metric Optimization -> Public Algo Launch
- **Thumbnail Prompt 1 (Before & After)**: [Detailed AI prompt with color contrast & emotional cues]
- **Thumbnail Prompt 2 (Action Teaser)**: [Detailed AI prompt with 1-2 characters & clear mobile focal point]
- **Mobile Readability Checklist**: [Focal point zoom, no background noise, large 3rd-grade text]
```
