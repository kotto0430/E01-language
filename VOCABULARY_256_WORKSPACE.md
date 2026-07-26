# English0.1 Vocabulary 256 Workspace

This file is the working area for expanding English0.1 from 128 words to 256 words.

The current 128 words remain unchanged during the selection process. Candidate words are not official vocabulary until they pass review and testing.

## Goal

Select 128 additional words mainly for:

- sandbox games
- survival and crafting games
- first-person shooters
- cooperative multiplayer games
- simple online communication

The goal is not to collect many game nouns. The goal is to add words that create the largest number of useful messages.

## Selection Method

Each candidate receives five scores from 0 to 5.

| Factor | Question |
|---|---|
| Frequency | How often will players need this word? |
| Meaning gain | How many new messages become possible? |
| Genre range | Is it useful across several game genres? |
| Simplicity | Is the meaning easy for beginners to understand? |
| Replaceability | Can current E01 words already express it easily? |

`Replaceability` is reversed during scoring: difficult-to-replace words receive more points.

Maximum score: 25.

## Decision Labels

- `A` — likely addition
- `B` — useful, but must compete for space
- `C` — situational or replaceable
- `D` — probably reject
- `TEST` — requires sample-dialogue testing

## Important Design Questions

Before accepting a word, test these questions:

1. Can existing E01 words express the same meaning clearly?
2. Does the word work in both sandbox and FPS games?
3. Will beginners recognize or learn it easily?
4. Does it combine well with other E01 words?
5. Is a more general word better than a specific word?

Example:

```text
furnace
```

may be useful in one sandbox game, but:

```text
fire box
```

may already communicate enough. A general word such as `inside` may deserve the space more.

## Candidate Pool — Draft 1

The following 320 words are candidates only. They are deliberately broader than the final 128 additions.

### 1. Pronouns and Basic Reference

I, you, we, they, it, this, that, these, those, someone, something, other, each, both, own, another

### 2. Questions and Logic

what, where, when, who, why, how, which, yes, maybe, because, if, then, before, after, same, different

### 3. Space and Position

inside, outside, above, below, behind, beside, between, around, across, through, toward, away, corner, edge, entrance, exit

### 4. Places and Terrain

room, hall, tunnel, cave, tower, hill, mountain, river, lake, road, field, forest, island, ground, sky, area

### 5. Movement and Body Position

walk, jump, climb, crawl, crouch, hide, dodge, turn, enter, escape, return, cross, swim, drive, ride, land

### 6. Combat Actions

shoot, aim, hit, damage, kill, reload, throw, guard, defend, flank, retreat, revive, mark, ping, search, find

### 7. Weapons and Combat Items

gun, rifle, pistol, shotgun, sniper, knife, sword, bow, grenade, bomb, bullet, magazine, scope, minefield, trap, explosive

### 8. Health and Danger States

alive, hurt, wounded, sick, poison, bleeding, full, empty, broken, locked, unlocked, weak, strong, stuck, lost, found

### 9. Team Tactics

scout, spread, split, group, line, circle, zone, route, point, objective, checkpoint, position, backup, support, leader, player

### 10. Buildings and Structures

wall, door, window, roof, floor, stairs, ladder, bridge, gate, fence, bunker, shelter, tower, platform, path, room

### 11. Materials

stone, wood, metal, glass, dirt, sand, clay, brick, iron, gold, coal, oil, fuel, paper, cloth, leather

### 12. Tools and Containers

hammer, axe, pickaxe, shovel, saw, key, rope, torch, chest, box, barrel, bottle, bucket, machine, engine, wheel

### 13. Sandbox Actions

place, dig, chop, plant, grow, harvest, cook, melt, repair, upgrade, remove, rotate, connect, fill, pour, burn

### 14. Environment and Weather

day, night, rain, snow, storm, wind, fire, smoke, gas, ice, hot, cold, wet, dry, dark, bright

### 15. Resources and Inventory

resource, material, stack, slot, storage, chest, supply, part, piece, seed, meat, fish, drink, medicine, bandage, battery

### 16. Vehicles and Travel

car, truck, bike, boat, helicopter, plane, tank, train, vehicle, engine, wheel, seat, station, fuel, passenger, driver

### 17. Game Systems

score, round, match, mode, server, save, load, restart, setting, menu, mission, task, reward, rank, skill, power

### 18. Trade and Ownership

price, cost, free, coin, cash, store, market, vendor, pay, share, keep, own, borrow, return, cheap, expensive

### 19. Social Communication

hello, bye, please, welcome, yes, maybe, correct, wrong, easy, hard, funny, happy, sad, angry, afraid, lucky

### 20. Time and Quantity

today, tomorrow, yesterday, morning, evening, night, minute, hour, second, soon, early, late, more, less, enough, half

## Duplicate and Conflict Notes

Some candidates intentionally appear in more than one conceptual category because their importance crosses categories. Before scoring, the list will be normalized into one unique master list.

Potentially important conflicts include:

- `gun` versus more specific weapon names
- `hurt` versus `wounded`
- `room` versus `area`
- `mission` versus the existing word `quest`
- `store` versus the existing word `shop`
- `support` versus the existing expression `team help`
- `return` as movement versus returning an item
- `minefield` versus the existing word `mine`

## First-Pass Priorities

These words appear especially difficult to replace and will receive early testing:

```text
I you we they this that
what where when who why how
inside outside behind between through
jump climb crouch hide enter exit
shoot aim reload throw revive
wall door window floor stairs ladder
stone wood metal dirt sand
key rope chest box
place dig chop plant repair
alive hurt empty broken locked
night fire smoke gas ice
room tunnel cave hill road
score round player save load
more less enough
```

## Testing Plan

Candidate words will be tested in at least these scenarios:

1. FPS enemy callouts
2. FPS team commands
3. ammunition and healing requests
4. entering and clearing buildings
5. sandbox resource gathering
6. crafting and construction
7. inventory management
8. survival threats and weather
9. vehicle travel
10. trade and item exchange
11. joining, leaving, saving, and restarting a game
12. short friendly conversation

A word should normally solve several communication failures before it is accepted.

## Kotto Review Role

Kotto does not need to score every English word.

Kotto will mainly decide:

- which situations matter most in actual play
- whether two short messages feel meaningfully different
- which word feels easier or more fun to use
- final tie-breaks between similarly ranked candidates

Yomi will manage candidate collection, English meaning, duplicate detection, scoring, dialogue tests, and the first 128-word shortlist.

## Current Status

- [x] Preserve the existing 128-word vocabulary
- [x] Define selection rules
- [x] Create a broad candidate pool
- [ ] Normalize duplicate candidates
- [ ] Score all unique candidates
- [ ] Produce a provisional top 128
- [ ] Test the top 128 in sample conversations
- [ ] Ask Kotto to resolve close decisions
- [ ] Publish the official 256-word vocabulary
