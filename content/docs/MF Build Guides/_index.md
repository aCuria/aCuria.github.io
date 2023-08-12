---
weight: 2
bookCollapseSection: false
bookToc: false
title: "MF Builds"
---

# Miss Fortune Builds
This section contains the builds I currently think are the best. 

Unlike most other guides, I attempt to derive the "best" build entirely algorithmically using event based simulation. 

{{< section >}}


## How it works
The algorithm works by looping over every combination of items, with the time complexity being O(N6) for 6 items, O(N5) for 5 items, and so on. A rejection function is used to remove invalid combinations such as multiple mythics. Additional rules, such as requiring a grevious wounds item, can also be applied. To optimize the algorithm, AP items are removed for MF computation. Enemy build orders and runes are manually entered based on data from lolalytics or personal games.

The computation of damage is the complicated part of the algorithm and is done using an event queue. The queue checks which events (auto attacks, skills, items) are currently off cooldown and executes them, then moving the clock forward to the next event until a predetermined amount of time has passed. Tank champions require longer time intervals of 6-8 seconds compared to 4 seconds for other champions. This approach is called event-based simulation.

After computing the damage and other statistics for every item combination, the results for damage, time to kill, and effective HP are stored. The challenge at this point is to make sense of the data since there is so much of it. One approach is to use multiple 2-variable Pareto curves to cull the data down, but there may be more efficient methods available. 

## Engine Updates
- 13.8: Generating item printout is now threaded on a per-sort type basis instead of per-result basis
- 13.8: N item build now attempts references N-1 item build for item order search
- 13.8: Updated HP shard to 15-140 HP from 15-90... cant believe I missed this one, seems OP
- 13.8: Started tracking the (effective_HP / tk) metric, which I think could give a better indication as to what build to go for against dps champions. That is, the faster that we can kill, the less defence we need to block incomming damage. This seems to favor bloodthirster late game.
- 13.7: For builds which costing less than the most expensive build, I previously added 1 ad per 35g under 6 items. Now, I instead add BFS / Pickaxe / LS item components, stopping when the build hits 6 components. This has the effect of giving value to slot efficency.
- 13.7: I no longer consider Collector's execute damage when computing ult damage, as this somewhat skewed results favoring collector.
- 13.7: If a build does not have more lifesteal than dorans blade, the Vamp Scepter component is forced. This means Bloodline allows for Vamp Scepter to be skipped, which frees one slot
- 13.7: Lifeline and Stoneplate shields are now triggered at the 30% threshold, as opposed to a pre-process step. This theoretically should make BOTRK weaker, but it only affected item power levels into tanks
- 13.7: For the purposes of BOTRK, enemy healing is now applied linearly as the enemy takes damage.
- 13.6: Berzerkers Greaves is added to the item rotation instead of being a forced item. If no out-of-combat movement speed items (Yoummus, Zeal item, Lethality Mythics...) are purchased, 300g boots1 are forced, consuming one slot. This is effectively a discount on movement speed items.
- 13.6: total distance traveled towards an enemy target in combat is computed. This includes temporary effects, such as BOTRK active
