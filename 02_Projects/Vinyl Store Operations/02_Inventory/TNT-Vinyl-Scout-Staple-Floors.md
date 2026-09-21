---
title: Vinyl Scout house-staple floors
updated: 2026-09-21
status: draft for Tam + Tre
owner: Tam (lock), Tre (confirm), Groove (encode in Scout later)
source: Scout Trending/Reorder 2026-09-21 + TNT ops (Dark Side / Meddle checks)
---

# House-staple floors (draft)

**Rule:** These titles should not sit at 1 copy. When on-hand drops below the floor, Scout should flag reorder and suggest qty to **get back to the floor** — not mirror peak-sold (no more “Reorder: 11”).

**Default floors**
- Most staples: **floor 2** (reorder when 1 or 0)
- Absolute movers / gift magnets: **floor 3** (reorder when 2 or below)
- Sub Pop always-back when OOS stays as-is for the rest of Sub Pop; floors below override for named titles

Accessories / stickers / sleeves: **exclude** from staple floors and from Trending noise.

## Proposed list (15)

| # | Title | Floor | Why | Confidence |
| --- | --- | --- | --- | --- |
| 1 | Pink Floyd — The Dark Side of the Moon | **2** | Scout peak 11; Tam already wanted 2 on shelf | High — lock |
| 2 | Pink Floyd — Meddle | **2** | Same lane; recent stock check | High — lock |
| 3 | Fleetwood Mac — Rumours | **3** | Scout peak 11; classic gift / millennial staple | High |
| 4 | Tame Impala — Currents | **2** | Scout peak 10; modern-chill fit | High |
| 5 | Queen — Greatest Hits | **2** | Scout peak 14; always sells | High |
| 6 | Smashing Pumpkins — Siamese Dream | **2** | Scout out / peak 8 | High |
| 7 | Nirvana — Nevermind | **2** | Sub Pop + Seattle; Scout calendar ORDER on Sept 24 (stock 0) | High |
| 8 | Miles Davis — Kind of Blue | **2** | Jazz staple on Trending; chill-tastemaker | High |
| 9 | Bob Marley — Legend | **2** | On Trending; gift / first-timer | Medium |
| 10 | Jeff Buckley — Grace | **2** | On Trending; tastemaker | Medium |
| 11 | Alice in Chains — Dirt | **2** | Scout peak 11; Seattle metal/grunge | Medium — ask Tre |
| 12 | Alice in Chains — Jar of Flies | **2** | On Trending with Dirt | Medium — ask Tre |
| 13 | Fleet Foxes — Fleet Foxes | **2** | Sub Pop / WA; Scout Sub Pop Watch | High |
| 14 | Pearl Jam — Ten | **2** | Seattle staple (studio Ten; Live Ten is first-carry separate) | High |
| 15 | The Postal Service — Give Up | **2** | Sub Pop Watch; local indie staple | Medium — ask Tre |

## Not on this list (on purpose)

- Discovery / color variants / IEX — stay qty 1, no floor
- First-carries never in RAIN — stay off Scout reorder; Tre adds by hand
- Cold-inventory sitters (peak sold 0) — markdown / move, not floors

## How Scout should behave once encoded

1. If title is on this list and `on_hand < floor` → appear in Reorder Queue with reason `Staple floor`.
2. Suggested qty = `floor - on_hand` (usually 1), optionally +1 if peak sold is very high — **cap at 2** unless Tam raises it.
3. Mark Ordered still clears the row for the week.

## Next

- Tam/Tre: check, cut, or bump floors.
- Then encode in Vinyl Scout (repo) or keep as a printed override until then.
