# Card Shop Tycoon: Game Design v0.1

Working title. Change it any time.

## The pitch
You own a trading card shop. Open packs, pull rare cards, put them on display to earn coins while you're away, and rebirth to grow faster.

## Core loop
1. Earn coins (tap the register, plus passive income from displayed cards)
2. Buy packs
3. Open packs and pull cards of different rarities
4. Put your best cards on display shelves to earn more coins every second
5. Rebirth: reset your coins and shop for a permanent multiplier and better packs
6. Repeat, faster each time

## First card set (assumption, change if you want)
"Street Ballers": 40 original basketball characters with exaggerated styles. No real players, no real teams, no league branding.

## Rarity
| Rarity | Base odds | Coins per second on display |
|---|---|---|
| Common | 60% | 1 |
| Uncommon | 25% | 3 |
| Rare | 10% | 10 |
| Epic | 4% | 40 |
| Legendary | 0.9% | 200 |
| Mythic | 0.1% | 1,500 |

**Variants** roll on top of rarity and multiply income:
* Gold: 1 in 50, 3x
* Rainbow: 1 in 500, 10x

Variants add a lot of chase without needing new art (a frame and a shader on the same card).

## Packs
| Pack | Cost | Open time | Notes |
|---|---|---|---|
| Starter | 100 coins | Instant | Common to Rare only |
| Pro | 1,000 coins | 30 seconds | Can hit Epic |
| Elite | 25,000 coins | 5 minutes | Can hit Legendary |
| Legend | 500,000 coins | 1 hour | Best Mythic odds. Unlocks at Rebirth 1 |

Timed packs keep opening while you're offline, so players have a reason to come back.

## Shop
* Display shelves: start with 5 slots, buy up to 30
* Register: tap for coins, upgradeable
* Offline earnings: 50% of your income rate for up to 8 hours

## Rebirth
* Resets coins, shelf slots and register upgrades
* Keeps all cards
* Gives +50% permanent income per rebirth, and unlocks the next pack tier
* Cost rises steeply each time

## Album
Every unique card (including variants) you've ever pulled is logged. Completing rarity rows gives permanent bonuses. This rewards collecting over and above income.

## Monetization (prices are placeholders)
* Game passes: 2x Coins, Auto Open, 2x Luck, VIP Shelf (+5 slots)
* Developer products: 15 minute Luck Boost, coin bundles, instant pack open
* Odds for every pack shown in game, as Roblox policy requires for paid random items

## Version 1 scope
**In:** one shop per player (6 players per server), register, shelves, 4 packs, 40 cards, rarity and variants, offline earnings, rebirth, album, saved progress, leaderboard, game passes.

**Not yet:** trading, raiding other shops, events, limited time packs. These come after real players have tested Version 1.

## Milestones
1. Project set up, a pack opens and gives a card
2. Shelves and passive income working
3. Saving, offline earnings, rebirth
4. Game passes, polish, card art
5. Soft launch to real players, look at the data, then iterate

## Technical choices
* Code lives in GitHub, synced into Studio with Rojo (the standard pro workflow)
* Player data saved with ProfileStore (the standard library for safe Roblox saving)
* All rewards and rolls happen on the server, so exploiters can't cheat in cards
