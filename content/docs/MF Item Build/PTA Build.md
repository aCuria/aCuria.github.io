---
weight: 2
bookToc: false
draft: false
title: "PTA Build"
---

# PTA Guide (Updated Patch 14.11)
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
![](/StatMods/StatModsAttackSpeedIcon.png) 
![](/StatMods/StatModsAdaptiveForceIcon.png)


![](/StatMods/StatModsHealthPlusIcon.png) this is better into late game assasins

![](/StatMods/StatModsHealthScalingIcon.png) this is better in lane

## Early Game
![](/item/1055.png)

![](/item/1053.png)![](/Styles/Precision/AbsorbLife/AbsorbLife.png) this is extremely important against poke. If there is no poke you can skip scepter and the absorb life rune.


![](/item/1083.png)
![](/item/1001.png) In general I will try to make cull which is just free gold. If rushing Youumu first item, we can choose to skip boots.


{{< tabs "Patches" >}}
{{< tab "14.11" >}} 

The main change is that IE got severely nerfed to the point its no longer a good early game rush item... and Shieldbow got an enormous buff.
- Looking at the AA only dataset, ER / Axiom kills draven the fastest at 1 item, but these items not what we want mid game....  
- For this reason playing for autos early game seems to be dead because we dont have a strong 1st and 2nd item to support it. We really need to play for ult damage and short trades (aa q aa & q2) instead
{{< /tab >}}
{{< /tabs >}}


{{< tabs "PTA" >}}



{{< tab "Default Build" >}} 

# Build Idea 
The idea is to use R to chunk the enemy team first, then follow up with autos. The build which kills a tank the fastest is considered the best.

## Core Items

![](/item/3142.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3031.png)
![](/item/3072.png)

Note that if scepter is in inventory, we may have to make BT before IE.

## Replace boots with one of the below items.

![](/item/6673.png) I suspect this may be the best item to make by default. the idea is to live for 2s longer and get an extra couple of autos off.

![](/item/3032.png) This item is damage optimal into bruisers (even assuming no ult) when considering ult it also achieves optimal kill times. For this reason this is probably the best damage item after the core build...

![](/item/3161.png) This is one of the oddball items that the algo likes, the kill time is top tier for both ult damage and autos only datasets. It even gives ability haste and 300 hp. That said it needs to be "charged up", with stacks. The algo assumes an all in scenario, but this will do less damage in situations where you just need to auto a couple of times.

![](/item/6698.png) ![](/item/6699.png) ![](/item/3508.png) ![](/item/6696.png)These all do about the same (top tier) ult damage, but I think we want more tankiness at this stage fo the game.

![](/item/6695.png) This the best damage option into big shields, for example shieldbow users.

![](/item/3814.png) Does less damage, we make this mainly for the spellshield.

{{< /tab >}}

{{< tab "Anti AP Assassins" >}}
Note that into hybrid threats just make shieldbow because Maw will not help against AD.

![](/item/3142.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3031.png)
![](/item/3072.png)
![](/item/3156.png)

![](/item/3142.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3072.png)
![](/item/3156.png)
![](/item/3814.png)

{{< /tab >}}

{{< tab "Anti AD & Hybrid damage Assassins" >}}

I would default to this 

![](/item/3142.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3031.png)
![](/item/3072.png)
![](/item/6673.png)

Note that GA does a lousy job at making us tankier, it just gives us the revive passive.

![](/item/3142.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3072.png)
![](/item/6673.png)
![](/item/3026.png)

This build actually makes us tankier

![](/item/3142.png)
![](/item/3036.png)
![](/item/6676.png)
![](/item/3072.png)
![](/item/6673.png)
![](/item/2501.png)

{{< /tab >}}

{{< /tabs >}}


# Gameplay
{{< youtube O9lDW4cvHhU >}}



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