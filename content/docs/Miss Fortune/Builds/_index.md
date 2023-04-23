---
weight: 1
bookCollapseSection: false
bookToc: false
title: "MF Builds"
---

# Builds Introduction
This section contains the builds I currently think are the best. 

Unlike most other guides, I attempt to derive the "best" build entirely algorithmically using event based simulation. 

# How it works
The algorithm works by looping over every combination of items, with the time complexity being O(N6) for 6 items, O(N5) for 5 items, and so on. A rejection function is used to remove invalid combinations such as multiple mythics. Additional rules, such as requiring a grevious wounds item, can also be applied. To optimize the algorithm, AP items are removed for MF computation. Enemy build orders and runes are manually entered based on data from lolalytics or personal games.

The computation of damage is the complicated part of the algorithm and is done using an event queue. The queue checks which events (auto attacks, skills, items) are currently off cooldown and executes them, then moving the clock forward to the next event until a predetermined amount of time has passed. Tank champions require longer time intervals of 6-8 seconds compared to 4 seconds for other champions. This approach is called event-based simulation.

After computing the damage and other statistics for every item combination, the results for damage, time to kill, and effective HP are stored. The challenge at this point is to make sense of the data since there is so much of it. One approach is to use multiple 2-variable Pareto curves to cull the data down, but there may be more efficient methods available. 

