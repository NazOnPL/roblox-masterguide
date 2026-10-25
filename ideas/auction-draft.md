# Idea: $20 auction draft (from the TikTok trend)

Status: validated 2026-10-25, **pivot before building**. Open questions for Naz at the bottom.

## The pitch (Naz, 2026-10-25)

Two players, $20 each. A category (animals, soccer players, anime). One item shows at a time, both bid, the higher bid takes it. At the end, compare teams and see whose is better. Plan: make lots of themed versions fast (soccer, animals, anime...).

## Concept Validation Report: $20 Draft

- **Market classification: Red Ocean, 3 months in.** The trend broke on TikTok in summer 2026 and Roblox clones landed within weeks (August). At least 9 live games already copy it 1:1, several from studios doing exactly the "one theme per game" plan.
- **Demand signals: real and still strong, but already being harvested.**
  - TikTok: "20 dollar draft" tags in the tens of millions of posts; creators like @waterboyzshow and @9kamz run themed drafts (restaurants, rooms, teams). On TikTok the *comment section judges* the winner.
  - Roblox (checked 2026-10-25):

    | Game | Studio | Created | Now | Peak | Visits | Note |
    | --- | --- | --- | --- | --- | --- | --- |
    | Choose the Stronger Anime! | Epic Party Games! | Aug 2026 | 3.3K CCU | 5.3K (today) | 12.2M | Still climbing, #24 Party & Casual, 12 min sessions, 80% likes |
    | Choose the stronger soccer! | Triple T party Games | Aug 21 | 229 CCU | 3.2K (Sep 12) | 4.8M | **Died: -93% in 6 weeks**, not updated in 4 weeks |
    | Bid Draft | One More Bid! | 2026 | ~800 CCU | n/a | 2.8M in 28d | 7-day CCU down 42%, 9 min sessions |
    | Choose your favorite! | Burnt Pancake | Aug 6 | n/a | n/a | n/a | 1v1, 30-player servers, sells chairs 49-199 R$ + 2x passes |
    | Choose the Stronger Animal! | Aphiphany Studios | 2026 | n/a | n/a | n/a | 72 animals, 10-item auction, hidden power revealed at end |
    | Draft Wars | Party Mini Games | 2026 | n/a | n/a | n/a | Twist: you *build* something with the items, then it's judged |
    | Draft The Best Team! | ? | 2026 | n/a | n/a | n/a | Twist: 3 secret value hints each, bluff to drain the other's budget |
    | $20 Bid Or Lose!, 20 Dollar Draft [BETA], Draft Club | various | 2026 | n/a | n/a | n/a | More clones |

- **What the data says about "pump out themed versions":** it's already being done, and the results split hard. Anime held and is still growing; soccer spiked and collapsed. A reskin is a lottery ticket on the theme, not a business. Late reskins also fight Roblox's duplicate-metadata suppression and the incumbents' head start in search ("Choose the Stronger X" now owns the keyword).
- **Why anime won and soccer died (best guess, not proven):** anime has an existing *power-scaling* argument culture ("who'd win"), so "whose team is stronger" is a debate kids already have. Soccer has FIFA ratings, so the answer is obvious and the draft is solved fast. **Pick themes where the answer is arguable, not looked up.**
- **The 80% foundation:** the TikTok format as is: $20, one item at a time, open bidding, max team size, reveal at the end. Plus the party-game table lobby (30-player server, 1v1 at tables, chairs as cosmetics) the incumbents already use.
- **The 20% innovation (pick one, don't stack):**
  1. **The server is the comment section (recommended).** Duels happen at tables in a shared lobby; when both teams are done, the whole server votes on who drafted better (big on-screen side-by-side, 5-second vote). Spectators bet free coins on the winner before the reveal. This copies what actually made the TikTok trend work (public judging), fixes "who judges", and makes 2-player matchmaking a non-issue because spectators are always playing. Proof the vote format works on its own: *6 Boys Vs 6 Girls - Vote for the BEST* sits at 3.1K CCU in the same category.
  2. **Teams actually fight.** After the draft, the two teams auto-battle in a 10-second animated fight with hidden stats revealed one by one. This is the payoff moment the clones skip (they just compare numbers). Costs more to build per theme.
  3. **Many themes in one game.** Each round the lobby votes the category (animals, food, anime-style, cars, brainrot). One place builds all the retention, favorites and algorithm history instead of splitting it across 8 games. New themes become your update cadence.
- **Titling and fantasy grade: B.** "Choose the Stronger [X]" is clunky but owns search now. Options at 3rd-grade reading level: **"Draft the Best Team"** (taken), **"Bid to Win"**, **"$20 Draft"** (keyword match, weak fantasy), **"Who Drafts Better?"** (matches the vote twist). The emotional promise is *outsmarting your friend*: lead with that.
- **Potential CCU ceiling:** a plain reskin: 200 to 3K, gone in ~6 weeks (soccer's curve). The top of this niche today is ~5K. A real twist that also works with crowds could beat that, but no game in the niche has proven a higher ceiling.
- **Go / No-Go: No-go on the "pump out reskins" plan. Conditional go on one game with twist #1 (crowd vote), ideally combined with #3 (themes rotate inside one game).** Ship fast: the trend is ~3 months old and the window is closing.

## The three questions Naz asked about

### IP risk (soccer players, anime characters)
- Real footballers: names and faces are licensed (FIFPRO, clubs, leagues). Roblox enforces DMCA takedowns, and a strike hits the account, not just the game. Images are the bigger risk; plain text names are lower but not zero.
- Anime: fan art of Goku, Naruto etc. is unlicensed IP. Incumbents get away with it until they don't; you'd be building on something that can be removed overnight, and you'd be the smaller target only until you work.
- Safer: themes nobody owns (animals, food, mythical creatures, cars by type, brainrot memes, "anime-style" original characters), or Roblox's own licensed IP programs if a deal ever exists. Per the boilerplate rule: screen every asset pack before upload.

### How "whose team is better" gets judged
Three options, in the order I'd rank them:
1. **Crowd vote** (TikTok's comment section, live). Subjective, fun, social, needs other people in the server.
2. **Hidden power stats revealed at the end** (Choose the Stronger Animal does this). Works solo, but once players learn the values the bidding is solved; you'd need to reroll or randomize stats each round.
3. **Rules/synergies** (e.g. "need 1 striker, 1 keeper" or type bonuses). Deepest strategy, slowest to learn: bad for "hook in seconds".
Best combo: hidden stats as a fallback when the server is empty, crowd vote when it isn't.

### 2-player matchmaking
- Don't make the player wait for a match. Per Naz's own rule (Fake an Egg note): never make a core step depend on another player choosing to act.
- Sit down at any table, and if no human joins in ~5 seconds, a bot with a personality fills the seat ("Greedy Gary always overbids on the first item"). Bots also teach the game in the first round.
- Use Roblox party/friend invites as the 1v1 path; 30-player social servers for everything else.

## Hook in seconds (first 30s)
- Spawn already seated at a table, round 1 starts, first item flips with a drum roll. No menu.
- Bid buttons: +$1, +$3, ALL IN. Countdown 5s with ticking SFX. The winning bid slams the item onto your side of the table.
- End: big side-by-side reveal, crowd vote, confetti, winner's chair rises.

## Monetization notes (design-and-monetize lens)
- What incumbents sell: chairs (49-199 R$), VIP, 2x cash/wins/streak passes.
- Fits the fantasy better: table themes, bid hammer skins, victory emotes, "reroll this item" product (once per match, sold at the moment of pain), extra $1 budget token (pay-to-win risk: keep it out of ranked).
- Spectator bets (free coins) give a currency sink and a reason to stay between your own matches.

## Update 2026-10-25: Naz picks "they actually fight" as the twist

Naz's idea: at the end the teams go head to head (soccer: a simulated match; animals: each player's 1st animal fights the other's 1st, and so on).
This is twist #2 above, now the lead twist. The fight is the judge; the crowd's job becomes betting free coins on each matchup.

What makes or breaks it:
1. **Lineup phase after the draft.** 10 seconds to order your team, blind reveal. Fixed slot-vs-slot means the bidding decides everything; ordering adds counter-pick strategy (sacrifice the cheap pick to the opponent's best).
2. **Luck in every fight** (dodge, crit, type/arena matchups). Pure stats get learned in a few rounds and the auction is solved; upsets of a $2 pick over a $9 pick are the clip moments.
3. **Short and cheap.** ~5 seconds per 1v1, best of 5. Soccer: 3 highlight moments (shot, save, goal), not a full match sim. Animals share animation sets by body type, so a new theme doesn't cost weeks.

Open: arena with 3D models walking out, or cards fighting on the table?

## Open questions for Naz
1. Why this over your current games? Is it a quick cash-grab you'd ship in a week, or something you'd run live ops on?
2. Are you fine dropping real footballers/anime for unowned themes?
3. Which judging feels right to you: crowd vote, hidden stats, or both?

## Sources
- Choose the Stronger Anime stats: https://rivalducks.com/apps/radar/games/10759594563-choose-the-stronger-anime
- Choose the stronger soccer stats: https://www.rolimons.com/game/84526099099491
- Bid Draft stats: https://creatorexchange.io/roblox-game/10742246265/bid-draft
- Choose your favorite: https://www.roblox.com/games/125291129308897/Choose-your-favorite and https://chooseyourfavorites.wiki/updates/
- Choose the Stronger Animal: https://www.roblox.com/games/108481366788727/Choose-the-Stronger-Animal
- Draft Wars: https://www.roblox.com/games/108079595771676/Draft-Wars
- Draft The Best Team: https://medal.tv/games/roblox/experiences/1b9Ct3DbuyvwcA/draft-the-best-team
- Trend rules and origin (self-reported by an app maker): https://dronkapp.com/20-dollar-draft/
