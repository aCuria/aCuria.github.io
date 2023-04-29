---
weight: 5
bookToc: false
title: "Multipliers"
---

# Damage Multipliers

## Lethality

The armor value here is the remaining armor after % armor pen.

| Armor | 18   | 36   | 40   | 54   | 79   |
|-------|------|------|------|------|------|
| 74    | 1.12 | 1.26 | 1.3  | 1.45 | 1.74 |
| 125   | 1.09 | 1.19 | 1.22 | 1.32 | 1.54 |
| 150   | 1.08 | 1.17 | 1.19 | 1.28 | 1.46 |
| 200   | 1.06 | 1.14 | 1.15 | 1.22 | 1.36 |
| 250   | 1.05 | 1.11 | 1.13 | 1.18 | 1.29 |
| 300   | 1.05 | 1.1  | 1.11 | 1.16 | 1.25 |
| 350   | 1.04 | 1.09 | 1.1  | 1.14 | 1.21 |
| 400   | 1.04 | 1.08 | 1.09 | 1.12 | 1.19 |

## % Armor Pen 

| Enemy Armor | LDR  | (LDR + BC) |
|-------------|------|------------|
| 100         | 1.18 | 1.34       |
| 150         | 1.22 | 1.44       |
| 200         | 1.25 | 1.52       |
| 250         | 1.27 | 1.57       |
| 300         | 1.29 | 1.62       |
| 350         | 1.3  | 1.66       |
| 400         | 1.32 | 1.69       |


## Navori + Bullet Time Multiplier

| Crit Chance | AD Ratio | Navori Multiplier | Total Ad Ratio | Damage Multiplier (x) |
|-------------|----------|-------------------|----------------|-----------------------|
| 0           | 0.75     | 1                 | 0.75           | 1                     |
| 20          | 0.79     | 1                 | 0.79           | 1.05                  |
| 40          | 0.83     | 1.08              | 0.8964         | 1.2                   |
| 60          | 0.87     | 1.12              | 0.9744         | 1.3                   |
| 80          | 0.91     | 1.16              | 1.0556         | 1.41                  |
| 100         | 0.95     | 1.2               | 1.14           | 1.52                  |

Therefore, Navori and 100% crit is a 1.52x Bullet Time damage increase


## Infinity Edge + Bullet Time Multiplier
| Crit Chance | AD Ratio with IE | Damage Multiplier |
|-------------|------------------|-------------------|
| 0           | 0.75             | 1                 |
| 20          | 0.79             | 1.05              |
| 40          | 0.858            | 1.14              |
| 60          | 0.912            | 1.22              |
| 80          | 0.966            | 1.29              |
| 100         | 1.02             | 1.36              |

Therefore, Navori and 100% crit is a 1.36x Bullet Time damage increase.

## Crit Damage + Basic Attack Multiplier

| Crit Chance | Multiplier | Multiplier (With IE) |
|-------------|------------|----------------------|
| 0           | 1          | 1                    |
| 20          | 1.15       | 1.15                 |
| 40          | 1.3        | 1.44                 |
| 60          | 1.45       | 1.66                 |
| 80          | 1.6        | 1.88                 |
| 100         | 1.75       | 2.1                  |

100% Crit increases basic attack damage by 1.75x, which increases to 2.1x with IE.


## Attack Speed + Basic Attack Multiplier

| Bonus AS (Runes, Items) | Total Bonus As (Items, Runes, L18, Strut) | Attacks per second | Multipier |
|-------------------------|-------------------------------------------|--------------------|-----------|
| 0%                      | 151%                                      | 1.64656            | 1         |
| 25%                     | 176%                                      | 1.81056            | 1.1       |
| 40%                     | 191%                                      | 1.90896            | 1.16      |
| 50%                     | 201%                                      | 1.97456            | 1.2       |
| 75%                     | 226%                                      | 2.13856            | 1.3       |
| 100%                    | 251%                                      | 2.30256            | 1.4       |
| 115%                    | 266%                                      | 2.40096            | 1.46      |
| 130%                    | 281%                                      | 2.49936            | 1.52      |
| 184%                    | 335%                                      | 2.8536             | 1.73      |

Note that 184% requires lethal tempo. Compared to 130% attack speed, lethal tempo is an additional 1.73/1.52 = 13.8% damage increase.

Formula: Attacks per Second = BaseAttackSpeed * (1 + BonusAttackSpeed)

## Giant Slayer
| Enemy HP - MF HP | 250   | 500  | 1000 | 1500 | 2000 | 2500 |
|------------------|-------|------|------|------|------|------|
| Multiplier       | 1.025 | 1.05 | 1.1  | 1.15 | 1.2  | 1.25 |

## Cut Down
| % more HP than MF | 10%  | 25%  | 75%  | 100% |
|-------------------|------|------|------|------|
| Damage Multiplier | 1.05 | 1.07 | 1.12 | 1.15 |



