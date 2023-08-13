---
weight: 1
bookToc: false
draft: false
title: "PTA Item Build"
---

# PTA Guide (Updated Patch 13.16)
I am going to keep it simple. For more details consult the Simulation Data directly and create your own build.


## Duskblade Build


### Core Items

![](/item/7002.png)![](/item/3153.png)![](/item/3036.png)

This is the core build I try to go for every game. It does well at 1 item (Best for Ult), decently at 2 items but it really spikes hard at 3 items. 

![](/item/3033.png)

You may need mortal reminder instead of LDR. consult the LDR vs MR page to find out when to buy what.

### AD Assasins

![](/item/3026.png)

Unfortunately, our capability to tank through AD assasin damage has been severely gimped because of nerfs to Overheal (less shield), Bloodthirster (No Shield) and Shieldbow (Not Mythic). For this reason, we have to lean into GA which makes us a less tempting target.

I think Shieldbow is not very helpful into the assasins, but this is based on my own playtesting rather than computation so do your own testing. The bloodline, shieldbow and health Stat Mod ideas felt weak when i tried them.

### AP Burst Champions
![](/item/3156.png)![](/item/3091.png)
We have always leaned into Maw against AP burst. Since Maw now scales with AD, its not so good when used with low ad builds like Rageblade

Stacking Wits can be helpful because some Champions can reduce our MR to zero even with Maw. Build wits if necesssary

### Ultimate Damage
![](/item/6676.png)![](/item/6696.png)

Build Collector this to make Ult hit harder, but I do feel that Axiom in addition is usually overkill. 

I think that going all out maximizing ult damage (replace BOTRK with BT, make a 3rd lethality legendary) alone is usually bad, a hybrid build with good ult and Sustained damage is probably better most of the time.

### Sustained Damage / DPS (Pick 3 Items)

![](/item/6672.png)![](/item/3091.png)![](/item/6676.png)![](/item/3115.png)![](/item/3087.png)

For dps Champions, maximizing time to kill against effective HP against sustained damage is usually the correct choice. 

For bruisers we need to kill them in the small window where they are CCed by our team. This means maximizing dps in a full glass cannon build.

Into tanks, we just want as much DPS as possible, as well as sufficient defenses to survive their damage. Kraken is particularly good into targets that take > 3 hits to kill, otherwise Kraken passive is wasted.

Wits End is good into thornmail, since thornmail users do not buy enough mpen to counter wits end and base resistances.

Nashors tooth is the oddball item, but the simulation does say its a good 6th item pickup.



## Runes: PTA - Cut Down - Gathering Storm
The main damage runs to consider for ultimate damage are Cut Down, Gathering Storm and First Strike.

While First Strike and Gathering storm can have stronger ult damage into squishies, into tanky champions Cut Down + Gathering Storm is stronger into tanks! On top of this, PTA has the strongest non-ultimate damage potential. Therefore, since I run into tanky enemy champions almost every game, these are my default runes

![](/Styles/Precision/PressTheAttack/PressTheAttack.png)
![](/Styles/Precision/Overheal.png)
![](/Styles/Precision/LegendAlacrity/LegendAlacrity.png)
![](/Styles/Precision/CutDown/CutDown.png)
![](/Styles/Sorcery/AbsoluteFocus/AbsoluteFocus.png)
![](/Styles/Sorcery/GatheringStorm/GatheringStorm.png)
![](/StatMods/StatModsAdaptiveForceIcon.png)
![](/StatMods/StatModsAdaptiveForceIcon.png)
![](/StatMods/StatModsHealthScalingIcon.png)
<!-- ![](/StatMods/StatModsAttackSpeedIcon.png) -->

- Use Manaflow Band over Absolute Focus if you cannot deal with mana control. Personally I get triggered every time an enemy walks away with 1HP when I run Manaflow Band.
- Use Coup de Grace if no enemies have 10% more HP than MF.
- You can use whatever Stat Mods you want (attack speed, adaptive force, armor, health). 
	- Scaling health is better late game rune, because into lethality stacking champions, the armor shard does nothing. Early game, the armor Stat Mod is better.
	- adaptive force is better for poke (Q2) and ult damage.


## Supports
The support makes or breaks botlane. This build **must** be played with a suitable supports.

### Suitable Supports:
- Hook Supports: Blitzcrank, Thresh, Nautilus, Pyke
	- MF has trouble dashing into an engage far away. Hook supports solve this problem by bringing the fight to us. 
- Poke + Engage Supports: Ashe, Lux
	- long stuns / roots that go through minions. The CC sets up MF's ultimate. 
- AOE Engage Supports: Ammumu, Neeko, Galio, Rell
	- Survive lane and get 5 man ults

### Unsuitable Supports: use comet or different adc.
- No on demand engage:
	- Soraka, Brand, Veigar,
- MF cannot take advantage of these delayed engage champions well.
	- Yuumi, Senna, Karma


## Early Game itemization
![](/item/1055.png)![](/item/2003.png)

These are the default starting items, the health on Dorans is very valuable for early game all-in situations.

![](/item/1036.png)![](/item/2003.png)![](/item/2003.png)![](/item/2003.png)

The alternate starting items into poke lanes. 3 Pots buys us more time in lane to rush out Vamp Scepter and Refillable on first back

![](/item/1053.png)![](/item/1083.png)![](/item/1001.png)

I aim to build this every game, you have to learn when to pick each one up based on experience.

## Deeper dive into the build 
I used data from Simulation Data/All to settle on duskblade as the mythic of choice. This item does well on the TK_ULT pareto curve into non-tanks, yet it is one of the best mythics into tanks (outside of Rageblade, which has poor ult damage and build path)

Playtesting has also supported the idea that duskblade is probably the best mythic for MF the majority of the time 

### 1st item
At 1 item, we want to be able to duel the enemy ADC in a laning phase situation. Looking at the Duskblade/Jinx data, we can see that the 3 candidate items are 

- Kraken (strongest all-in)
- Ravenous Hydra (Middle Ground)
- Duskblade (strongest Ult) 

If we look at the 2 to 6 item data, we can see that Ravenous Hydra falls off the pareto curve later in the game. For this reason we can strike Hydra off.

Kraken unfortunately has an absolutely abysmal build path for MF, because it now builds out of recurve bow instead of Pickaxe.

Therefore, since we are going for a duskblade build anyway, Duskblade seems to be the best choice for our first item.

### 2nd Item 
The problem with the second item is that we are sitting on a fair number of items:
1) Duskblade
2) Boots1
3) Scepter 
4) Dorans 
5) Cull (With Stacks)
6) Refillable

Of these items, we only want to sell Refillable and cull when completed. This means an item like Collector, which features in the 2 item data can be difficult to build towards since it has 3 components.

If we look at the 3 item ASol / graves / Jax data, we can see that the Duskblade - BOTRK - Last Whisper idea is strong. It is also natural to build BOTRK because we are already sitting on one component (Scepter) so the 2 item powerspike will be hit earlier than with other choices

Duskblade - Collector - Last Whisper


## Discussion on other Mythics

From the simulation data it is clear that there are only three competive mythics. 

Rageblade has the best dps into tanky champions, primarily because it amplifies BOTRK damage. we are talking killing a late game sion in just 2.5s compared to 3.36s without it. However, it also has many problems...
- Ultimate damage is poor, because Rageblade prevents Ult from critting. We can improve ult damage but this can be somewhat addressed by shoring up ultimate damage with Collector and Axiom Arc 
- 