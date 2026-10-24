# /live-ops — Scientific Live Operations & Game Health Engine

Use this command to establish weekly update schedules, patch routines, community feedback pipelines, and data-driven hypothesis testing to scale and sustain 10k-50k+ CCU.

## Command Execution Workflow
When the user invokes `/live-ops [Game Status / Metric Problem]`:

### Step 1: The Live Ops Architecture (Patches vs. Updates)
Distinguish clearly between hotfix patches and scheduled updates:
- **Daily Patches (Launched on the Fly)**:
  * Anticheat hotfixes, exploit patches, game-breaking bug resolutions, economy balance tweaks, micro-buffs/nerfs.
  * Never wait for a scheduled weekend update to fix game-breaking bugs or exploits. Ship daily.
- **Weekly / Bi-Weekly Updates (Targeted Metric Sprints)**:
  * Scheduled for Saturday mornings.
  * Every major update must target ONE specific metric on your dashboard (Play Time, D1, D7, or 7-Day Spend Days).

### Step 2: The Weekly Production Cadence
Implement the high-velocity live ops calendar:
- **Saturday**: Launch weekly update / event $\rightarrow$ Review immediate CCU peak $\rightarrow$ Brainstorm next week's focus.
- **Sunday**: Assign scope to builders/modelers via strict Trello cards & contracts.
- **Monday–Wednesday**: Team builds assets and UI; producer reviews and iterates.
- **Thursday**: Update is fully integrated into private test place.
- **Friday**: Internal playtesting (team) followed by playtesting with the **Core Council**.
- **Saturday Morning**: Public launch.

### Step 3: The 3-Pillar Data Research Method
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

### Step 4: The Scientific Method for Metric Optimization
Every single update is a testable hypothesis:
$$\text{If I } [\text{Add / Remove / Modify Feature } Y], \text{ then } [\text{Metric } X] \text{ will improve because } [\text{Evidence } Z].$$

- *Example Hypothesis*: "If we add a build-mode feature where new players can construct bases without PvP raiding, then Play Days Per User and D1 retention will increase because new players won't churn from instant griefing."
- **Review Cycle**: Check rolling 7-day data.
  * If the metric improves: Keep the feature and build on it.
  * If the metric degrades: Revert the change immediately and formulate a new hypothesis.

### Step 5: The Core Council & Dedicated Test Place
- **The Core Council**: Maintain an elite group of 8–10 dedicated "sweat" players in a private Discord channel.
- Bounce update ideas off them, give them exclusive playtest roles, and let them stress-test economies.
- **Dedicated Live Test Place**: ALWAYS publish updates to a separate live Roblox test place first. Live Roblox servers have replication bugs and physics nuances that never show up in local Studio.
