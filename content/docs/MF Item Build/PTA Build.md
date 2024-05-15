---
weight: 2
bookToc: false
draft: false
title: "PTA Build 14.10"
---

# PTA Guide (Updated Patch 14.10)
I am going to keep it simple. For more details consult the Simulation Data directly and create your own build.

# Idea
The idea behind using PTA, is that 

- There are enemy team comps where MF gets jumped every teamfight and FS becomes useless. This means assasin comps

- Sometimes, a successful ult is insufficient to clean up. This is the case against tanks.

The builds here are generated assuming we ult the enemy for its full duration, and then use autos to finish them off. The builds that can do this the fastest are considered the best. This is a departure from the previous idea of just using autos and ignoring ult damage.

## Runes
![](/Styles/Precision/PressTheAttack/PressTheAttack.png)
![](/Styles/Precision/AbsorbLife/AbsorbLife.png)
![](/Styles/Precision/LegendAlacrity/LegendAlacrity.png)
![](/Styles/Precision/CutDown/CutDown.png)
![](/Styles/Sorcery/AbsoluteFocus/AbsoluteFocus.png)
![](/Styles/Sorcery/GatheringStorm/GatheringStorm.png)
![](/StatMods/StatModsAttackSpeedIcon.png) and some combination of 
![](/StatMods/StatModsAdaptiveForceIcon.png)![](/StatMods/StatModsHealthPlusIcon.png)![](/StatMods/StatModsHealthScalingIcon.png)

## Early Game
![](/item/1055.png) > 
![](/item/1083.png)
![](/item/1001.png)


{{< tabs "PTA" >}}



{{< tab "Anti Tank (E+R into AA's)" >}} 

# Anti Tank Build (E+R into AA's)
The idea is to use R to chunk the enemy team first, then follow up with autos. The build which kills a tank the fastest is considered the best.

## Maximize damage potential

![](/item/3031.png)
![](/item/1001.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3072.png)
![](/item/3142.png)

## Force early Yoummus 

![](/item/3142.png)
![](/item/1001.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3031.png)
![](/item/3072.png)

## Force early BT 

![](/item/3072.png)
![](/item/1001.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3031.png)
![](/item/3142.png)

## Replace boots with one of the below items.

![](/item/3095.png)
![](/item/3508.png)

![](/item/6695.png) only into shields

![](/item/6673.png)
![](/item/3161.png) these 2 items trade damage for durability
{{< /tab >}}




{{< tab "Anti Tank Build (AAs only, no R)" >}} 

# Anti Tank Build (AA's)
The idea is to use AA > Q > AA > AA... to kill the enemy tank. The build that kills the fastest is considered the best.

## Maximize damage potential (Kills in 2.37s)

![](/item/3508.png)
![](/item/1001.png)
![](/item/6672.png)
![](/item/3036.png)
![](/item/3031.png)
![](/item/6676.png)
![](/item/3142.png)

## Assuming BT is in the build (Kills in 2.69s)
![](/item/3508.png)
![](/item/1001.png)
![](/item/3036.png)
![](/item/3072.png)
![](/item/3031.png)
![](/item/6676.png)
![](/item/3142.png)

{{< /tab >}}


{{< tab "Anti AD Assasins and Hybrid Burst damage build" >}} 

# Anti AD Assasins and Hybrid Burst damage build 
The idea is to be as tanky as possible against burst damage, while still having enough damage to kill the assasin.

If we can survive the assasin's burst damage, then we should win the 1v1 because our sustained damage is better.

The algo assumes assumes ult is NOT used, and generates a pareto curve of "time to kill" against "effective HP against burst damage".

Builds on the resultant pareto curve with good ult ult damage are prioritized.

Use exhaust and scaling health runes ![](/StatMods/StatModsHealthPlusIcon.png)![](/StatMods/StatModsHealthPlusIcon.png) 
You can consider bloodline for the health, but I feel we lose too much early game power without alacrity, and it takes forever to stack bloodline.

![](/item/6673.png)
![](/item/1001.png)
![](/item/3036.png)
![](/item/3072.png)
![](/item/3142.png)
![](/item/3814.png)
![](/item/3748.png)

{{< /tab >}}


{{< tab "Anti AP Assasin" >}} 

# Anti AP Assasin Build
The idea is to be as tanky as possible against burst damage, while still having enough damage to kill the assasin.

If we can survive the assasin's burst damage, then we should win the 1v1 because our sustained damage is better.

The algo assumes assumes ult is NOT used, and generates a pareto curve of "time to kill" against "effective HP against burst damage".

Builds on the resultant pareto curve with good ult ult damage are prioritized.

Use exhaust and scaling health runes ![](/StatMods/StatModsHealthPlusIcon.png)![](/StatMods/StatModsHealthPlusIcon.png) 
You can consider bloodline for the health, but I feel we lose too much early game power without alacrity, and it takes forever to stack bloodline.

![](/item/3072.png)
![](/item/1001.png)
![](/item/3036.png)
![](/item/3814.png)
![](/item/6676.png)
![](/item/3156.png)
![](/item/3142.png)

{{< /tab >}}

{{< tab "Anti DPS" >}} 

# Anti DPS (for example, the enemy ADC)
WIP - idk what the meta builds for the enemy adcs are yet.

{{< /tab >}}


{{< /tabs >}}





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