# Palworld Base Planner

Adjustable base planner for Palworld 1.0.x. Set your level, how many bases you can place, your worker cap and whether the World Tree is unlocked. The base roles, unlock ladder, carry list, build checklist and material totals all follow.

Live at [gorgon.live/palworld-planner/](https://gorgon.live/palworld-planner/).

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole tool. One file, no build step. |

## Behavior

- **Setup panel:** level (quick-set 20 / 45 / 65 / 78), bases 1 to 4, worker cap 15 to 50, World Tree, wiping bases, building the Ancient Furnace.
- **Base layouts:** 4 bases is ore, ancient, breeding, oil. Fewer bases merge roles (3 folds oil into ancient, 2 drops oil, 1 holds everything). Worker gauges show when a merged base runs over your cap.
- **Unlock ladder:** 16 entries with levels (structures, the Paloxite and Coralum Ingot recipes, and the Plasma Multicutter), plus three structures whose level I couldn't verify. The Paloxite chain gates on the Lv 74 ingot recipe, not the Lv 66 furnace.
- **Carry list:** only the hand-carried moves your layout needs.
- **Checklist and totals:** locked steps are greyed. Totals are a planning figure and can include locked structures.
- **Confidence marks:** ● two or more sources or game data, ◐ one source or sources disagree, ○ unverified.

## Data

Checked 9 to 11 Nov 2026 against Pindrop's game-data pages, palworld.tools and several guides. Palworld changes often, so the "What I couldn't confirm" section lists what to verify in game. Change history is in `CHANGELOG.md`. Worker counts and the 1, 2 and 3 base layouts are estimates, not sourced.

## Persistence

`localStorage` only, keys `palworld-base-planner-v2-settings` and `palworld-base-planner-v2-checks`. Nothing leaves the browser. Clearing site data resets it.

## Stack

Pure HTML, CSS and vanilla JS. Google Fonts is the only external request. Loads `../nav.js` for the hub bar and does nothing if it's absent.

## Standing

Unofficial fan tool. Not affiliated with or endorsed by Pocketpair.
