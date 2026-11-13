# Changelog — palworld-planner

All notable changes to the Palworld Base Planner (gorgon.live/palworld-planner/).

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

---

## 2026-11-13 — Ranch base redesign

### Changed
- Base roles rebuilt around the 20-Pal cap: ore and oil, ancient and breeding, a ranch base, and a food base. One base for ranching, breeding and crops filled the cap too fast (a Ranch holds 4 Pals, breeding needs 2+).
- Ranch base: four Ranches of four Pals with a roster (Staples, Sweets, Gear, Organs). Output rates in 1.0 are unpublished, so the roster is a starting point.
- Food base: plantations, Mill and kitchens. Cakes (Cake, Mushroom, Vegetable, Extravagant Vegetable, Special) and kitchen levels are in the ladder (one source, flagged).
- Carry list now routes through the Guild Chest (Lv 41, 54 slots, one per base). It corrects the earlier assumption that items can't move between bases.
- Totals add Guild Chest costs and an Ancient Civilization Parts line. Four chests, the Recycler and the Hatchery come to about 100 Parts.
- Layouts for 1, 2 and 3 bases merge roles; the 1-base layout has no Guild Chest.

### Merged
- Rebased onto the 2026-11-11 accuracy review: unlock levels, Lv 74 Paloxite gating, World Tree coordinates and source list are all kept.

## 2026-11-11 — Accuracy review

Full fact check against Pindrop's per-structure game-data pages, palworld.tools, the Palworld wiki and several guides.

### Fixed
- World Tree location: the ancient-site note said "Foot of the World Tree (about 841, 639)", which is the northeast. The Base of the World Tree fast travel point is in the far northwest at about -838, 689 (two guides). The 841, 639 figure came from guides that dropped the sign.
- Unlock levels were 1 too high: Sulfur Quarry 47 → 46, Pure Quartz Quarry 53 → 52, Hexolite Quartz Mine 63 → 62, High-Pressure Crude Oil Extractor 52 → 51 (each confirmed by two sources).
- Paloxite chain gating: the chain, World Tree carry run and mining steps opened with the Ancient Furnace at Lv 66. The Paloxite Ingot recipe unlocks at Lv 74 (four sources), so they now gate on Lv 74.
- Ancient Furnace and Ancient Workbench no longer require the World Tree toggle. Neither build cost uses World Tree materials, and the furnace makes Soralite Ingots from Lv 66.
- Ancient Workbench: unlock level 67 (two sources) replaces the guess that tied it to the furnace.
- Recycler output no longer lists Cores as a regular return. Mythical Wood and Paloxite are guaranteed; Cores come only from tier 4 and 5 relics.
- Holy Water source corrected from "fishing, drops" to Teafant Springs in the World Tree (one guide, flagged).
- Removed the claim that Astegon works nights because it's a Dark type. No source supports it.
- Removed "Lv 6+" work-suitability minimums. Sources disagree (Lv 1+ vs Lv 10), so the planner now names the suitability only.

### Changed
- Hatchery cost (100 Paloxite Ingots, 50 AI Cores, 30 Parts, 20 Cores) is now marked confirmed. Pindrop and the wiki both match it, so the "one guide" caveats are gone.
- Coal Quarry Lv 37 marked confirmed (two sources).
- Ladder adds the Crude Oil Extractor (50), Plasma Multicutter (54), Coralum Ingot recipe (62), Ancient Workbench (67) and Paloxite Ingot recipe (74).
- Mining Pal note now lists Mining levels: Aegidron 8, Astegon and Blazamut 7, Anubis 6.
- Hatchery note: it runs on cake and collects its own eggs, so Grintale and Broncherry partner skills don't apply (wiki).
- Holy Water steps mention the World Tree passive alternative. Plasma Multicutter is "fastest", not required.
- Ore ridge note now cites the Sealed Realm of the Guardian at about 180 to 190, -40, and marks "raids can't path up" as one guide's claim.
- "What I couldn't confirm" rewritten: added World Tree coordinates, Paloxite Ingot station, Synthesizer cost conflict, work-suitability levels and Holy Water source. Removed items now resolved.
- Sources list expanded.

---

## 2026-11-10 — Initial release

### Added
- Single-file planner: setup panel (level, bases, worker cap, World Tree, wipe, furnace), base cards, unlock ladder, Paloxite chain diagram, carry manifest, build checklist, material totals, recipes and doubts list.
- localStorage keys `palworld-base-planner-v2-settings` and `palworld-base-planner-v2-checks`.
