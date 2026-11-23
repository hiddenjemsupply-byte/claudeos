# Game Plan: Rough Draft v0.1

Status: idea stage. Nothing gets built until this plan feels right.
Working title: none yet.

## The Pitch
Melvor Idle's skilling and crafting with Old School RuneScape's feel, in a shared world where you can see, trade with, and compete against real players. Runs in a browser, so one link works on phone and PC.

## What Iain Wants (from our first Q&A)
* Leveling skills toward a max level
* Crafting chains: gather, process, make gear, use it to go further
* Combat and gear, chasing better drops
* Progress while away
* A light shared world: chat, trading, leaderboards, clans. You mostly play your own character
* A mix of idle and active. Idle skilling, plus active stuff when you're on

## The Gap in the Market
* **Melvor Idle** proved the idea sells. Estimated 424K copies on Steam at $9.99, around $3.6M gross (third party estimate, not official). Jagex picked it up as publisher. Its big weakness: no other players. It's a single player game.
* **Idle Clans** is the closest to this idea, a multiplayer idle MMO with clans. It's small, about 600 to 700 players online on Steam, 74% positive reviews, with complaints about stability.
* **IdleOn** is the most popular "MMO squeezed into an idle game," but it's busy and spread across many characters.
* **Brighter Shores** (from RuneScape's creator) lost most of its players. Reviewers blamed a huge grind and thin multiplayer.

Takeaway: people want Melvor with other people in it, and nobody has nailed it yet. The ones that tried were either too small, too buggy, or too grindy with nobody around.

## My Recommendation for the Hook
A shared world where the economy is fully player made, like the OSRS Grand Exchange, plus world events where everyone's idle work feeds one big goal (example: the whole server gathers materials to rebuild a bridge, which opens a new area and boss for everyone). That makes other players matter even when you're idle, which is what Melvor and Idle Clans are missing.

This is my suggestion, not locked. Flagged for Iain to react to.

## Core Loop
1. Pick a skill and let it run (chop, mine, fish)
2. Turn raw stuff into better stuff (smelt, cook, craft)
3. Use what you made to fight harder monsters
4. Get drops and gold, sell or trade with other players
5. Unlock new areas, new skills, new gear tiers
6. Close the game, come back to progress waiting

## Idle vs Active
* **Idle:** skills tick on their own, including while the game is closed. Offline progress capped (start with 12 hours) so checking in still matters.
* **Active:** being on gives something extra. Ideas: faster XP, rare finds, bosses you have to fight live, timed world events.
* Rule: active play should feel rewarding, never required.

## Starter Skills (first playable version)
Small on purpose. More skills come later.
* Gathering: Woodcutting, Mining, Fishing
* Making: Smithing, Cooking
* Combat: one combat skill plus Hitpoints, kept simple at first

## Shared World Features (in order)
1. Accounts and cloud saves
2. Hiscores (leaderboards per skill)
3. Global chat
4. Player market
5. Clans with a shared bank
6. Server wide world events

## Tech (rough)
* Browser first web app. Works on phone and PC from day one.
* A real server is required, because of the shared world and to stop cheating. The server decides how much progress you earned, not the player's device.
* Later: wrap the same code as phone apps and a Steam version. No rebuild.
* Specific tools get picked when we start building, after more research.

## Money (rough)
Recommendation: free to play in the browser, with a paid membership or one time unlock for extra content. Never pay to win. OSRS and Melvor players hate it, and it would kill the trading economy.

## Rules
* 100% original. No RuneScape names, art, items, map, or music. Same kind of game, our own world.
* Every build session is video content. Build in public.

## Phases
0. **Plan** (now): lock the idea, the hook, the name, the look
1. **Solo prototype:** one skill, a bank, offline progress. Prove the core feels good.
2. **Core loop:** starter skills, crafting chains, basic combat and gear
3. **Shared world:** accounts, hiscores, chat, market
4. **Public alpha:** real players, real feedback, start building an audience
5. **Expand:** clans, world events, more skills, phone apps, Steam

## Open Questions for Iain
* Setting and vibe: classic medieval fantasy like OSRS, or something different (pirate islands, post apocalypse, sci fi, something tied to skate culture)?
* Look: pure text and menus like Melvor, simple pixel art, or a small visible map you walk around on?
* Max level: 99 like OSRS, or something else?
* What do you hate in OSRS or Melvor? (grind walls, pay to win, bad UI, anything)
* Do you want PvP at all, or keep it friendly?
* Single character per account, or several like IdleOn?
* Any names floating around in your head?

## Sources
* Melvor Idle sales estimate: https://raijin.gg/app/1267910/Melvor_Idle
* Jagex publishing Melvor: https://mein-mmo.de/en/idle-games-are-the-trend-on-steam-now-a-large-mmorpg-studio-is-entering-the-clicker-business,739780
* Idle Clans player counts and reviews: https://raijin.gg/app/2103530/Idle_Clans
* Idle Clans Steam page: https://store.steampowered.com/app/2103530/Idle_Clans
* Games like Melvor (IdleOn, Brighter Shores, IdleMMO): https://www.ranker.com/list/games-like-melvor-idle-ranked/gabriel-cook
* Brighter Shores player drop: https://www.mmobomb.com/from-launch-to-life-support-brighter-shores-lost-97-of-players
* Brighter Shores grind review: https://massivelyop.com/2024/11/06/first-impressions-brighter-shores-has-gobs-of-potential-buried-under-mountains-of-grind/
* Brighter Shores multiplayer review: https://www.sportskeeda.com/mmo/brighter-shores-early-access-review
