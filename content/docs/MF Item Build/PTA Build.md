---
weight: 2
bookToc: false
draft: false
title: "PTA Build"
---

# PTA Guide (Updated Patch 14.19)
I am going to keep it simple. For more details consult the Simulation Data directly and create your own build.

Note: nothing really changed between 14.13-14.16

# Idea
The idea behind using PTA, is that 

- There are enemy team comps where MF gets jumped every teamfight and FS becomes useless. This means assasin comps

- Sometimes, a successful ult is insufficient to clean up. This is the case against tanks.

The builds here are generated assuming we ult the enemy for its full duration, and then use autos to finish them off. The builds that can do this the fastest are considered the best. This is a departure from the previous idea of just using autos and ignoring ult damage.

## Runes
![](/Styles/Precision/PressTheAttack/PressTheAttack.png)
![](/Styles/Precision/PresenceOfMind/PresenceOfMind.png)
![](/Styles/Precision/LegendAlacrity/LegendAlacrity.png)
![](/Styles/Precision/CutDown/CutDown.png)
![](/Styles/Sorcery/AbsoluteFocus/AbsoluteFocus.png)
![](/Styles/Sorcery/GatheringStorm/GatheringStorm.png)
![](/StatMods/StatModsAdaptiveForceIcon.png)
![](/StatMods/StatModsAdaptiveForceIcon.png)

![](/StatMods/StatModsHealthPlusIcon.png) this is better at L6+

![](/StatMods/StatModsHealthScalingIcon.png) this is better early game

## Early Game
![](/item/1055.png)

![](/item/1053.png) this is extremely important against poke. If there is no poke you can skip scepter and the absorb life rune.

![](/item/1083.png)
![](/item/1001.png) In general I will try to make cull over a long sword early game if I have 450g.


{{< tabs "Patches" >}}

{{< tab "14.19" >}} 
Massive changes to almost all items 
{{< /tab >}}

{{< tab "14.17" >}} 
Cut Down nerf: 
- Damage Threshold: Above 50% Maximum Health ⇒ Above 60% Maximum Health

Absorb Life nerf: 
- Level 1-5: 1-5 (based on level) ⇒ 1-2 (based on level)
{{< /tab >}}

{{< tab "14.16" >}} 
Blade of the Ruined King
- Attack Damage: 55 ⇒ 50
- Attack Speed: 30% ⇒ 25%
- On-Hit Damage: 9% (melee) / 6% (ranged) ⇒ 10% (melee) / 6% (ranged)
- I cant believe they made it even worse. Its tremendously weaker than previous seasons.
{{< /tab >}}

{{< tab "14.15" >}} 
Kraken Slayer
- Move Speed: 7% ⇒ 5%
- Bring it Down: 140-310 ⇒ 80% effectiveness for ranged champions (112-248)
- Wasnt good enough to build previously, and its even worse now.

Lord Domniks Regards
- Armor Penetration: 40% ⇒ 35%
- This is pretty painful, but LDR/MR is still the most powerful item in the game for MF.

Mortal Reminder
- Attack Damage: 40 ⇒ 35
- Grevious wounds is much more powerful than LDR's +10ad against almost any kind of healing.

Berserker’s Greaves
- Attack Speed: 35% ⇒ 30%
- Even less reason to build it now.

Wit’s End
- Fray: 15-80 ⇒ 40-80
- We dont really build this now, but it was situationally good in previous seasons. 

Dark Harvest
- Cooldown: 40 ⇒ 35
- On-takedown reset timer: 1.5s ⇒ 1s
- Probably doesnt matter. DH cant proc multiple times per ult, and without the stealth passive on Duskblade Mythic the DH playstyle is dead

Fleet Footwork
- Heal: 8-110 (linear) (+10% Bonus AD) (+5% AP) ⇒ 5-120 (following stat progression multiplier) (+10% Bonus AD) (+5% AP)
- Not relevant for MF.

Death’s Dance
- Armor: 40 ⇒ 50
- I dont think this makes it good enough to buy. Stacking HP/Shields (Shieldbow) is more effective because with only 1 armor item, lethality stacking assasins still reduce our armor value to 0

{{< /tab >}}

{{< tab "14.14" >}} 
Absorb Life 
- Healing: 2-20 (linear scaling) ⇒ 1-23 (following base stat progression) ( Note: This is a nerf levels 1-12 and a buff levels 13-18.)
- This is a nerf. Late game we can heal fine with BT, we only benefit from this rune before making the scepter component.
{{< /tab >}}


{{< tab "14.13" >}} 

MF got a buff, 
- you can absolutely feel its easier to last hit under tower thanks to the +3 base AD. 
- The "Strut Damage Lock-out" and "initial bonus" move speed buff is nice but its difficult to gauge how much of an impact this has, because we can W active to get the full max move speed immediately.
- The +5 to max bonus move speed is actually noticable, its possible to chase down champs more easily now.

overall we can last hit slightly easier with the +3 AD, and we can chase better because the initial bonus move speed was substantially increased.

Miss Fortune
- Base Attack Damage: 52 ⇒ 55
- Strut Damage Lock-out: 5 seconds ⇒ 4 seconds
- Strut Upgraded Move speed delay: 5 seconds ⇒ 3 seconds
- Strut Max bonus move speed: 55/65/75/85/95 ⇒ 60/70/80/90/100
- Strut Initial Bonus move speed: 25 ⇒ 30/35/40/45/50

Dark Harvest
- Damage: 20-80 (+5 per Soul) ⇒ 20 (+9 per Soul) (bonus ratios unchanged)
- Cooldown: 45 ⇒ 40

Electrocute
- Damage: 30-220 ⇒ 50-190 (bonus ratios unchanged)
- Cooldown: 25-20 (based on level) ⇒ 20

{{< /tab >}}

{{< tab "14.11" >}} 

The main change is that IE got severely nerfed to the point its no longer a good early game rush item... and Shieldbow got an enormous buff.
- Looking at the AA only dataset, ER / Axiom kills draven the fastest at 1 item, but these items not what we want mid game....  
- For this reason playing for autos early game seems to be dead because we dont have a strong 1st and 2nd item to support it. We really need to play for ult damage and short trades (aa q aa & q2) instead
{{< /tab >}}
{{< /tabs >}}


{{< tabs "PTA" >}}



{{< tab "Default (3-6 item spike into squishies)" >}} 

# Build Idea 
The build idea here is to optimize for 2 parameters:
- If someone jumps on us, we want to blow them up in the least possible time
- I also want good ult damage, so even if rageblade/kraken/BOTRK does kill someone faster in an all-in, I avoid them because they greatly impact ult damage.

Early game we want to take trades with aa>q>aa or Q2 and back off to heal back using lifesteal. Late game, we wait for our team to CC and then press R to get a couple of kills.


## 1: Make Core Items

![](/item/1001.png)
![](/item/1053.png)
![](/item/3031.png)
![](/item/6676.png)

- Boots: make it when you have an extra 300g
- Scepter: rush it if you need sustain against a poke lane, otherwise it can be delayed indefinitely because it weakens your all-in if you are not in a poke lane

## 2: Choose 1 (Prefer LDR)
![](/item/3036.png)![](/item/3033.png)

## 3: Choose 1 (Prefer BT)
![](/item/3072.png)![](/item/3153.png)![](/item/3139.png)

## 4: Choose 1
![](/item/3032.png)
![](/item/3156.png)
![](/item/3026.png)
![](/item/3814.png)
![](/item/6673.png)

## 4: sell boots for this
![](/item/3142.png)


## Notes
Note that following the build exactly is difficult because of high item component costs. We may have bought some longswords before getting BFS for instance. Collector can be built before IE to absorb some longswords.


{{< /tab >}}

{{< tab "1/2 Item spikes vs ADC" >}}

## 1 Item 

![](/item/3508.png) 3.81s (100-0 kill time)

![](/item/6672.png) 4.18s

![](/item/6676.png) 4.23s

![](/item/3031.png) 4.23s (Q2 is stronger with this though)

## 2 Items

![](/item/6676.png)![](/item/6672.png) 2.46s squishy kill time

![](/item/3031.png)![](/item/3036.png) 2.82s (Scales better)

{{< /tab >}}


{{< tab "Anti Tank" >}}

### 2 Items:

![](/item/3124.png)![](/item/3153.png) 6.16s  (100-0 kill time)

![](/item/3031.png)![](/item/3036.png) 7.09s (better ult damage)

### 3 Items:

![](/item/3124.png)![](/item/3153.png)![](/item/3036.png) 4.62s

![](/item/3031.png)![](/item/3036.png)![](/item/6676.png) 5.64s (better ult damage)

### 4 Items:

![](/item/3124.png)![](/item/3153.png)![](/item/3036.png)![](/item/6672.png) 4.35s

![](/item/3124.png)![](/item/3153.png)![](/item/3036.png)![](/item/3031.png) 4.55s

![](/item/3031.png)![](/item/3036.png)![](/item/6676.png)![](/item/3032.png) 4.74s (better ult damage)

### 5 items:

![](/item/3124.png)![](/item/3153.png)![](/item/3036.png)![](/item/3031.png)![](/item/6676.png) 4.09s

![](/item/3031.png)![](/item/3036.png)![](/item/6676.png)![](/item/3032.png)![](/item/3153.png) 4.3s (better ult damage)

### 6 Items:

![](/item/3124.png)![](/item/3153.png)![](/item/3036.png)![](/item/3031.png)![](/item/6676.png)![](/item/3142.png) 3.38s

![](/item/3031.png)![](/item/3036.png)![](/item/6676.png)![](/item/3032.png)![](/item/3153.png)![](/item/3142.png) 3.4s (better ult damage)

{{< /tab >}}


{{< /tabs >}}


# Gameplay
{{< youtube FPMdMDvjbe4 >}}
{{< youtube 8lLjWkrSz0E >}}



# Support Champions
The support makes or breaks botlane. This build **must** be played with a suitable supports.

## Suitable Supports:
- Hook Supports: Blitzcrank, Thresh, Nautilus, Pyke
	- MF has trouble dashing into an engage far away. Hook supports solve this problem by bringing the fight to us. 
- Poke + Engage Supports: Ashe, Lux
	- long stuns / roots that go through minions. The CC sets up MF's ultimate. 
- AOE Engage Supports: Ammumu, Neeko, Galio, Rell
	- Survive lane and get 5 man ults

## Unsuitable Supports: use comet or different adc.
- No on demand engage:
	- Soraka, Brand, Veigar,
- MF cannot take advantage of these "delayed CC" champions well.
	- Yuumi, Senna, Karma 