---
name: roblox-launch-and-live-ops
description: Plan a Roblox launch (ads, 500 engaged players, thumbnails) and run live ops (update cadence, metrics, hypotheses)
---

# Roblox launch and live ops

Run Part 1 before and during launch, Part 2 once the game is live.

# Part 1: Launch, ads and packaging

Use this to prepare a game for launch, manage sponsored ad budgets, navigate the 500 Highly Engaged Players requirement, and generate high-converting AI thumbnail prompts.

## Workflow
Input: Game Name / Launch Phase.

### 1.1 The Sponsored Ads Launch Strategy
Follow the low-budget, high-efficiency ad blueprint:
- **Daily Budget**: **$16 / 16 Ad Credits per day** (convert Robux into Ad Credits to maximize cost efficiency; never use raw USD unless required).
- **Targeting**: Select **All Players / Recommended**. Do NOT restrict targeting manually to 18-24. Roblox automatically filters unverified games to 16+ audience during initial launch.
- **Run Duration**: Run for a minimum of **3 to 7 days continuous**. Roblox analytics pipelines have a 2-3 day reporting delay. Never panic-kill ads within 24 hours.
- **Pre-Launch Beta Mode**: Keep the game in Roblox **Beta Mode** while running initial ad batches to optimize onboarding funnels and squash game-breaking bugs before entering the public Home Recommendation algorithm.

### 1.2 The 500 Highly Engaged Players Checkpoint
Understand and conquer the platform discovery hurdle:
- **What is a Highly Engaged Player?**: A player who has completed a verified purchase anywhere on the Roblox platform within the last 60 days. They do NOT need to spend money in your specific game.
- **The Bot Traffic Bottleneck**: Sponsored ads traffic includes cold traffic and non-spending accounts. Initial progress toward 500 will feel slow (10-20 players/day).
- **The Acceleration Curve**: As your stats improve, Roblox begins testing your game in organic Home Recommendations. Once organic traffic mixes in, progress surges rapidly (from 100 to 500 in 3-5 days).

### 1.3 The Algorithmic Crossover Rule (When to Kill Ads)
- Monitor **Acquisition $\rightarrow$ Home Recommendations** vs. **Sponsored Ads Impressions** in the Creator Dashboard.
- **The Golden Rule**: The exact moment **Home Recommendation Impressions exceed Sponsored Ad Impressions**, **TURN OFF PAID ADS**.
- Let the organic discovery flywheel take over. Only resume ad spend if you ship a massive metric-focused update and need fresh cohort data.

### 1.4 High-CTR AI Thumbnail Generation System
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

### 1.5 Deliver Launch Checklist & Midjourney/AI Prompts
Generate custom prompts for AI thumbnail tools (RowThumbs, Midjourney, etc.):
```markdown
# Launch & Packaging Blueprint: [Game Title]
- **Target Ad Budget**: 16 Ad Credits/day ($16/day) for 7 days
- **Launch Phase**: Beta Mode Testing -> Metric Optimization -> Public Algo Launch
- **Thumbnail Prompt 1 (Before & After)**: [Detailed AI prompt with color contrast & emotional cues]
- **Thumbnail Prompt 2 (Action Teaser)**: [Detailed AI prompt with 1-2 characters & clear mobile focal point]
- **Mobile Readability Checklist**: [Focal point zoom, no background noise, large 3rd-grade text]
```

# Part 2: Live ops

Use this to establish weekly update schedules, patch routines, community feedback pipelines, and data-driven hypothesis testing to scale and sustain 10k-50k+ CCU.

## Workflow
Input: Game Status / Metric Problem.

### 2.1 The Live Ops Architecture (Patches vs. Updates)
Distinguish clearly between hotfix patches and scheduled updates:
- **Daily Patches (Launched on the Fly)**:
  * Anticheat hotfixes, exploit patches, game-breaking bug resolutions, economy balance tweaks, micro-buffs/nerfs.
  * Never wait for a scheduled weekend update to fix game-breaking bugs or exploits. Ship daily.
- **Weekly / Bi-Weekly Updates (Targeted Metric Sprints)**:
  * Scheduled for Saturday mornings.
  * Every major update must target ONE specific metric on your dashboard (Play Time, D1, D7, or 7-Day Spend Days).

### 2.2 The Weekly Production Cadence
Implement the high-velocity live ops calendar:
- **Saturday**: Launch weekly update / event $\rightarrow$ Review immediate CCU peak $\rightarrow$ Brainstorm next week's focus.
- **Sunday**: Assign scope to builders/modelers via strict Trello cards & contracts.
- **Monday–Wednesday**: Team builds assets and UI; producer reviews and iterates.
- **Thursday**: Update is fully integrated into private test place.
- **Friday**: Internal playtesting (team) followed by playtesting with the **Core Council**.
- **Saturday Morning**: Public launch.

### 2.3 The 3-Pillar Data Research Method
Before planning any update, synthesize three data sources:
1. **Qualitative Data (Voice of the Player)**:
   * Discord bug reports & suggestions channel.
   * Creator Dashboard Feedback tab (AI summary of player sentiments).
   * **The 9-Year-Old iPad Test**: Search YouTube for low-view screen recordings of kids playing your game on an iPad. Watch where they get confused, tap erratically, or hesitate.
2. **Quantitative Data (The Dashboard Numbers)**:
   * Analytics $\rightarrow$ Engagement $\rightarrow$ New User First Session Retention.
   * Funnel Tracking: Milestone drop-offs (e.g. Zone 1 unlock, plot upgrade completion).
   * Benchmark against **Experiences with Similar Players** (NOT the broad genre benchmark).
3. **Competitor Research**:
   * Study top games in your subgenre. What features do they share? How do they handle inventory, level design, and event loops?

### 2.4 The Scientific Method for Metric Optimization
Every single update is a testable hypothesis:
$$\text{If I } [\text{Add / Remove / Modify Feature } Y], \text{ then } [\text{Metric } X] \text{ will improve because } [\text{Evidence } Z].$$

- *Example Hypothesis*: "If we add a build-mode feature where new players can construct bases without PvP raiding, then Play Days Per User and D1 retention will increase because new players won't churn from instant griefing."
- **Review Cycle**: Check rolling 7-day data.
  * If the metric improves: Keep the feature and build on it.
  * If the metric degrades: Revert the change immediately and formulate a new hypothesis.

### 2.5 The Core Council & Dedicated Test Place
- **The Core Council**: Maintain an elite group of 8–10 dedicated "sweat" players in a private Discord channel.
- Bounce update ideas off them, give them exclusive playtest roles, and let them stress-test economies.
- **Dedicated Live Test Place**: ALWAYS publish updates to a separate live Roblox test place first. Live Roblox servers have replication bugs and physics nuances that never show up in local Studio.

## Use Naz's own notes too

If the roblox-masterguide repo or the project files are available, also read the matching `notes.md` and any relevant `competitors/*.md` playtest notes, and prefer Naz's own observations where they are more specific.