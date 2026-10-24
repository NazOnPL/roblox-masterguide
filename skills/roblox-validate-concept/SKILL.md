---
name: roblox-validate-concept
description: Audit a Roblox game idea for demand, saturation, 80/20 twist and title before building anything
---

# Roblox concept validation

Use this before writing any Luau code or spending Robux on assets. This audits an idea against proven platform demand, market saturation, and viral packaging laws.

## Workflow
Input: Game Concept or Idea.

### Step 1: Demand Signal Verification (Off-Platform & On-Platform)
Evaluate whether the core loop and fantasy have pre-existing, validated consumer demand:
- **Off-Platform Signals**:
  * **Steam**: Are there emerging hits with 100k-200k+ wishlists (e.g., *Totally Secure Airport*, *Mecha Chameleon*)?
  * **Flash / Web (CrazyGames, CoolMathGames, AddictingGames)**: Check 3D Unity web games with 200k+ player votes or millions of plays (e.g., *Airport Security*, *Tiny Fishing*, *Jacksmith*).
  * **TikTok / Short-Form Trends**: Are there viral challenges with massive view counts (e.g., *Bomb Chip*, *Lying Challenge*, *Rubber Band Watermelon*)?
  * **Social Proof & Intent Signals**: Do YouTube comments on off-platform gameplays contain high-intent comments like *"Where can I play this? I don't have a PC/money"*?
- **On-Platform Baseline**: Search Creator Exchange and RoTrends for visits and CCU across the primary keyword.

### Step 2: Ocean Saturation Audit (Blue vs. Red vs. Purple)
Classify the market space:
- **Blue Ocean**: Zero market competition, unvalidated demand (High risk of failure).
- **Red Ocean**: Saturated market of clones (e.g., 500 identical fishing tycoons or "Don't Wake The..." clones). Roblox discovery algorithms actively suppress repetitive metadata and duplicate place files.
- **Purple Ocean (The Sweet Spot)**: High existing audience demand paired with poor, buggy, or abandoned execution.
  * Look for rising games on RoTrends with high CCU relative to total visits.
  * Look for games created recently where the developer stopped updating and the community page is flooded with bug complaints.

### Step 3: The 80/20 Mutation Strategy
Identify how to take the proven 80% foundation and inject a 20% meaningful twist:
1. **80% Proven Foundation**: What is the established core loop being borrowed (e.g., *Grow a Garden* plot layout, *Steal a Brain Rot* base locks, *Escape Tsunami* linear pressure-valve)?
2. **20% Meaningful Twist**: Choose at least one primary axis of innovation:
   - **Fantasy Twist**: e.g., instead of generic tycoon, make it "Hack a Business" (McDonald's / Apple hacking).
   - **Unique Mechanic Twist**: e.g., combining peaceful base building with real-time PvP raiding/stealing.
   - **Level Design Twist**: e.g., moving flat plots into a floating sky-island map where players can be hit into the void.
   - **Audience Twist**: e.g., converting a male-dominated survival genre into an animal rescue experience for female demographics.

### Step 4: Packaging & Titling Audit
Evaluate title and marketing hook:
- **Reading Level Rule**: Must be readable at a **3rd Grade reading level** (e.g., "Hack a Business" > "Sell Your Data" or "Cyber Security Simulator").
- **Proven Structural Formulas**:
  * `[Verb] a [Noun]` (*Build a Base*, *Hack a Business*, *Grow a Garden*, *Steal an Egg*)
  * `Be a [Noun]` (*Be a YouTuber*, *Be a Nurse*, *Be a Lucky Block*)
  * `Escape the [Noun]` (*Escape Tsunami*)
  * `[Implied Challenge]` (*99 Nights in the Forest*, *Hide from the Villain*)
- **Emotional Promise**: Does the title immediately convey what emotional state the player will experience (power, fear, sneaky triumph, wealth)?

### Step 5: Deliver the Concept Scorecard
Return a structured Markdown report:
```markdown
# Concept Validation Report: [Game Title]
- **Market Classification**: [Purple Ocean / Red Ocean / Blue Ocean]
- **Demand Signals**: [Summary of Steam/Web/TikTok/Creator Exchange metrics]
- **The 80% Foundation**: [Proven mechanics borrowed]
- **The 20% Innovation**: [Specific differentiator]
- **Titling & Fantasy Grade**: [A/B/C/F based on 3rd grade reading level & action verb]
- **Potential CCU Ceiling**: [Estimate based on comparable niche games]
- **Go / No-Go Verdict**: [Actionable greenlight or specific pivot recommendations]
```

## Use Naz's own notes too

If the roblox-masterguide repo or the project files are available, also read the matching `notes.md` and any relevant `competitors/*.md` playtest notes, and prefer Naz's own observations where they are more specific.