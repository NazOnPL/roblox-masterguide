# Roblox Masterguide

Naz's knowledge base for everything around a Roblox game except the code: ideation, validation, design, monetization, packaging, launch, live ops and competitor research. Scripting, project setup and asset-upload rules live in [roblox-game-boilerplate](https://github.com/NazOnPL/roblox-game-boilerplate) (`AGENTS.md`), not here. Every folder is one topic you can hand to a new game on its own.

## How to use it on a new game

1. Copy `starter-kit/` into the new repo. It gives you `CLAUDE.md` and the five slash commands (`/validate-concept`, `/design-loop`, `/monetize`, `/launch-prep`, `/live-ops`).
2. Copy any topic folder you need into the repo's `docs/` (for example `05-monetization/`), and tell Claude to read it.

## Topics

| Folder | What's in it | Slash command |
| --- | --- | --- |
| `01-mindset/` | Producer mindset, the 5-year-old rule | none |
| `02-ideation-validation/` | Purple ocean, 80/20 twist, demand signals | `/validate-concept` |
| `03-packaging/` | Titles, thumbnails, icons, mobile CTR | none |
| `04-game-design-retention/` | Core loop, FTUE, juice, retention | `/design-loop` |
| `05-monetization/` | Dev products, passes, purchase pathways, pricing | `/monetize` |
| `06-launch-algorithm/` | Sponsored ads, beta, discovery algorithm | `/launch-prep` |
| `07-live-ops/` | Patches vs updates, metrics, team | `/live-ops` |
| `inspiration/` | Clips of cool systems, mechanics, UI and VFX, plus useful tools | none |
| `ideas/` | Your game ideas, each with its validation report and open questions | `/validate-concept` |
| `competitors/` | One file per game you playtested: what to steal | none |
| `playtests/` | Playtests of your own games: fix lists, ready-to-paste prompts, ideas | none |
| `inbox/` | Raw brain dumps waiting to be sorted | none |
| `skills/` | The kit's slash commands as 3 Claude skills (validate concept, design + monetize, launch + live ops) | none |
| `sources/` | Original master guide and kit zip, untouched | none |

Inside each topic: `guide.md` is the Tizzy RBLX material, `notes.md` is your own observations and rules, and `command-*.md` is the matching slash command.

## How brain dumps get filed

Dump anything in the chat. It gets saved to `inbox/` with the date, then sorted: game-specific observations go to `competitors/<game>.md`, general rules go to the topic's `notes.md`.
