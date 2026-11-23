# Game Plan: Rough Draft v0.4

Status: idea stage. Nothing gets built until this plan feels right.
Working title: none yet.

## The Pitch
Melvor Idle's skilling and crafting, Old School RuneScape's feel, and Diablo 3's gear chase, in a shared world where you click to step across a map through biomes and dimensions. Built so a total beginner can pick it up. Runs in a browser, so one link works on phone and PC.

## What Iain Wants
* Leveling skills toward a max level
* Crafting chains: gather, process, make gear, use it to go further
* Combat and gear, chasing better drops, min maxing builds
* Progress while away
* A light shared world: chat, trading, leaderboards, clans
* A mix of idle and active
* A normal fantasy world with lots of biomes, terrains, and dimensions, like Terraria or Minecraft
* Text menus with pixel art. Click to take a step, move across a map, explore the biome
* Beginner friendly. This is the big one OSRS and Melvor miss
* Lots of bosses: mini bosses, group bosses, world bosses
* Diablo 3 ideas: gear, min maxing, dungeons, raids
* PvP only with level brackets or a level cap
* Classes
* Seasons, for sure
* No max level, like SimpleMMO
* One account, two free character slots. More slots cost Jems, the paid currency

## The Gap in the Market
* **Melvor Idle** proved the idea sells. Estimated 424K copies on Steam at $9.99, around $3.6M gross (third party estimate, not official). Jagex picked it up as publisher. Weakness: no other players.
* **Idle Clans** is the closest to this idea. Small, about 600 to 700 players online on Steam, 74% positive, complaints about stability.
* **SimpleMMO** shows the click to step idea works. It says it has 500K+ players and 240M+ steps taken (their own numbers). Each step gives a small random event. Weakness: very basic visuals and shallow depth.
* **Brighter Shores** (from RuneScape's creator) lost most of its players. Reviewers blamed a huge grind and thin multiplayer.

Takeaway: nobody has combined SimpleMMO's easy stepping, Melvor's skilling depth, and Diablo's gear chase in one shared world that's easy to learn.

## The Hook
1. **Easy to start, deep to master.** Beginners never need a wiki. Hardcore players get Diablo level min maxing.
2. **Dimensions.** The world keeps opening up. New dimension, new resources, new monsters, new bosses, new gear tier.
3. **The server does it together.** The economy is fully player made, like the OSRS Grand Exchange. World events have the whole server working toward one goal (example: everyone gathers materials to open a portal to a new dimension, then a world boss spawns on the other side).

Point 3 is my suggestion, not locked.

## The World
* Starts in a normal fantasy overworld split into biomes: forest, plains, desert, snow, swamp, caves, ocean.
* Dimensions sit beyond the overworld (ideas: underground, sky, fire, void). Each one is harder and is basically the next gear tier.
* Each biome has its own resources, monsters, mini boss, and a biome boss.

## How It Looks and Plays
* Text menus for skills, bank, gear, and crafting, like Melvor.
* A pixel art map where you click to take a step, like SimpleMMO but with better visuals.
* Each step can turn up something: a tree to chop, an ore vein, a monster, a mini boss, an item, a traveler, a funny bit of text.
* Find a resource and you can start gathering it. That keeps running while you're idle.

## Beginner Friendly (top priority)
* A Guide character, like Terraria's, who tells you what to do next and answers "what's this for?"
* Click any item to see where it comes from and what it makes. No wiki needed.
* A short first quest that teaches step, gather, craft, equip, and fight in about 10 minutes.
* A clear goals list that always shows your next step.
* Systems unlock a few at a time, never all at once.

## Combat and Gear (Diablo 3 influence)
* **Gear rarity tiers:** common up to legendary and set items.
* **Legendary powers:** items that change how your abilities work, so builds feel different.
* **Set bonuses:** wear the full set, get a big power spike.
* **Min maxing:** stats that matter, rerolling stats, upgrading gear.
* **Dungeons:** short runs with a boss at the end. Solo or group.
* **Raids:** big group fights for the best loot.
* **Endless scaling challenge:** like Diablo's Greater Rifts. Push as deep as your build allows, with a leaderboard.

Recommendation: regular fights run on their own and your build decides the result. On bosses, active players can trigger abilities for an edge. That keeps it idle friendly and still rewards being on. Flagged for Iain.

## Classes
* Pick a class when you make a character. Your class decides how you fight: your abilities, your gear, your role in a group.
* Every class can do every gathering and making skill. Class is about combat, not about locking anyone out of woodcutting.
* Launch with 3 classes: melee, ranged, and magic (working names: Warrior, Ranger, Mage). Locked for now. Add more classes over time, a good fit for new seasons.
* Each class gets its own legendary powers and set items, so builds feel different between classes and inside each class.
* Groups need a mix of classes for raids and group bosses, which gives players a reason to team up.

## No Max Level
* Levels go up forever, for your character and for every skill.
* Each level takes more XP than the last, so numbers keep climbing without breaking the game.
* Milestones every so often (example: every 10 levels) unlock things like new areas, titles, or perks, so there's always a next target.
* Hiscores show who's highest, which matters more when there's no ceiling.

## Seasons
* Every season starts a fresh seasonal world: new characters, everyone starts at zero, new leaderboards.
* Each season brings a theme or new feature (a new class, a new dimension, a new boss, a rule twist).
* Season rewards: cosmetics and titles you keep forever. Never power.
* When a season ends, seasonal characters move over to the permanent world, like Diablo 3.
* Seasons run 3 months. Locked.
* Bonus: every season launch is a natural video and a reason for old players to come back.

## Bosses
* **Mini bosses:** random finds while stepping through a biome
* **Biome bosses:** solo bosses that guard each biome
* **Dungeon bosses:** end of every dungeon
* **Group bosses and raids:** need a party
* **World bosses:** timed, server wide, everyone pitches in, loot for everyone who helped

## PvP
Optional, inside level brackets so high levels can't farm new players. Assumption: arenas you choose to enter, not open world. Flagged for Iain.

## Idle vs Active
* **Idle:** gathering, crafting, and regular fights keep running, even with the game closed. Offline progress capped (start with 12 hours) so checking in still matters.
* **Active:** stepping and exploring, bosses, dungeons, raids, world events.
* Rule: active play should feel rewarding, never required.

## Starter Skills (first playable version)
Small on purpose.
* Gathering: Woodcutting, Mining, Fishing
* Making: Smithing, Cooking
* Combat: one combat skill plus Hitpoints, kept simple at first

## Shared World Features (in order)
1. Accounts and cloud saves
2. Hiscores
3. Global chat
4. Player market
5. Parties for dungeons and group bosses
6. Clans with a shared bank
7. World bosses and server wide events
8. Raids and PvP arenas

## Tech (rough)
* Browser first web app. Works on phone and PC from day one.
* A real server is required for the shared world and to stop cheating. The server decides how much progress you earned, not the player's device.
* Later: wrap the same code as phone apps and a Steam version. No rebuild.
* Specific tools get picked when we start building, after more research.

## Money (rough)
* Free to play in the browser.
* The paid currency is **Jems**, named after Iain's middle name, Jem. It ties into the Hidden Jem Supply brand.
* Jems look like a bright pink purple gem. Exact shade gets picked with the art.
* Players can buy Jems with real money, and free players can earn small amounts by playing (season rewards, achievements). Free players matter: the game needs them for the economy and for bosses.
* Every account gets 2 free character slots. More slots cost Jems.
* Other things Jems could buy: cosmetics (outfits, pets, map icons), extra bank space, a membership.
* Rule: Jems never buy power, XP, or gear. That would wreck the player market, the leaderboards, and seasons.

## Rules
* 100% original. No RuneScape, Diablo, Terraria, or SimpleMMO names, art, items, maps, or music. Same kinds of ideas, our own world.
* Every build session is video content. Build in public.

## Reality Check
This is a big game. What's written here is the full vision, and it gets built a piece at a time. Version one is one biome, a handful of skills, and stepping on a map. If that small version isn't fun, the rest won't save it.

## Phases
0. **Plan** (now): lock the idea, the hook, the name, the look
1. **Solo prototype:** one biome, click to step, one gathering skill, a bank, offline progress, the Guide
2. **Core loop:** starter skills, crafting chains, basic combat and gear, mini bosses and a biome boss
3. **Shared world:** accounts, hiscores, chat, market
4. **Public alpha:** real players, real feedback, start building an audience
5. **Expand:** dungeons, parties, world bosses, more biomes, the first new dimension
6. **Endgame:** raids, set items, endless scaling challenge, PvP arenas, phone apps, Steam

## Open Questions for Iain
* Game name: still open

## Sources
* Melvor Idle sales estimate: https://raijin.gg/app/1267910/Melvor_Idle
* Jagex publishing Melvor: https://mein-mmo.de/en/idle-games-are-the-trend-on-steam-now-a-large-mmorpg-studio-is-entering-the-clicker-business,739780
* Idle Clans player counts and reviews: https://raijin.gg/app/2103530/Idle_Clans
* Idle Clans Steam page: https://store.steampowered.com/app/2103530/Idle_Clans
* SimpleMMO about page: https://simple-mmo.com/about
* SimpleMMO stepping mechanic: https://www.mobygames.com/game/154893/simplemmo/
* Games like Melvor (IdleOn, Brighter Shores, IdleMMO): https://www.ranker.com/list/games-like-melvor-idle-ranked/gabriel-cook
* Brighter Shores player drop: https://www.mmobomb.com/from-launch-to-life-support-brighter-shores-lost-97-of-players
* Brighter Shores grind review: https://massivelyop.com/2024/11/06/first-impressions-brighter-shores-has-gobs-of-potential-buried-under-mountains-of-grind/
* Brighter Shores multiplayer review: https://www.sportskeeda.com/mmo/brighter-shores-early-access-review
* Diablo 3 Greater Rifts: https://maxroll.gg/d3/resources/greater-rift-explained
* Diablo 3 Paragon levels: https://blizzardwatch.com/2021/01/13/paragon-levels-diablo-3/
* Diablo 3 gear loop: https://us.forums.blizzard.com/en/d3/t/how-hard-is-d3-endgame/46583
