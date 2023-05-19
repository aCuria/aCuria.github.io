---
weight: 2
bookToc: false
---


# This entire page is work in progress due to the massive changes in 13.10.
I am going to try to explain "how to fish" aka "how to come up with what build to use yourself"

# What is the best build?
There is no true "Best" Build for all games. The "Best" build is a situational one depending on the win condition of that particular game. For example:

## Win Condition: Not dying to the fed assasin = win game 

Build high Effective HP against Burst. Bloodline tends to be somewhat better at this metric
- [PTA Alacrity Rengar TK_ADEHP_BURST]({{< ref "RawData/PTA Alacrity/Rengar TK_ADEHP_BURST" >}})
- [PTA Alacrity Vex TK_APEHP_BURST]({{< ref "RawData/PTA Alacrity/Vex TK_APEHP_BURST" >}})
- [PTA Bloodline Rengar TK_ADEHP_BURST]({{< ref "RawData/PTA Bloodline/Rengar TK_ADEHP_BURST" >}})
- [PTA Bloodline Vex TK_APEHP_BURST]({{< ref "RawData/PTA Bloodline/Vex TK_APEHP_BURST" >}})

## Win Condition: Taking down the fed Riven / Insert Bruiser Here = win game 

If the bruiser touches us, we are supposed to die. Therefore use a glass cannon build that kills in a minimum amount of time, so that the bruiser has the smallest possible window to kill us.
Preferably we are able to 100-0 the Bruiser within the CC duration of our support

- [PTA Alacrity Riven TKILL]({{< ref "RawData/PTA Alacrity/Riven TKILL" >}})
- [PTA Bloodline Riven TKILL]({{< ref "RawData/PTA Bloodline/Riven TKILL" >}})

## Win Condition: Successfully Duel dps champions = win game 

In the late game, use builds with a fast kill time to effective HP ratio 
- [PTA Alacrity Jinx TK_ADEHP_D_TK]({{< ref "RawData/PTA Alacrity/Jinx TK_ADEHP_D_TK" >}})
- [PTA Alacrity Draven TK_ADEHP_D_TK]({{< ref "RawData/PTA Alacrity/Draven TK_ADEHP_D_TK" >}})
- [PTA Alacrity AurelionSol TK_APEHP_D_TK]({{< ref "RawData/PTA Alacrity/AurelionSol TK_APEHP_D_TK" >}})
- [PTA Bloodline Jinx TK_ADEHP_D_TK]({{< ref "RawData/PTA Bloodline/Jinx TK_ADEHP_D_TK" >}})
- [PTA Bloodline Draven TK_ADEHP_D_TK]({{< ref "RawData/PTA Bloodline/Draven TK_ADEHP_D_TK" >}})
- [PTA Bloodline AurelionSol TK_APEHP_D_TK]({{< ref "RawData/PTA Bloodline/AurelionSol TK_APEHP_D_TK" >}})

## Win Condition: Taking down the fed tank = win game 

Use an anti tank build. We dont want to get killed by the tank either, so effective HP against the tank's damage type is important
- [PTA Alacrity Chogath TK_APEHP]({{< ref "RawData/PTA Alacrity/Chogath TK_APEHP" >}})
- [PTA Bloodline Chogath TK_APEHP]({{< ref "RawData/PTA Bloodline/Chogath TK_APEHP" >}})

## Win Condition: Surviving Lane = win game 
This happens when facing an enemy ADC who has a strong early game and weak late game. One example would be Draven

Usually some variant comet build is best for this, expecially into immobile champions who do not have a dash to avoid E and comet damage.

- [Comet Draven TK_ULT]({{< ref "RawData/Comet CutDown/Draven TK_ULT" >}})

That said I really do not like playing comet because it does not scale well. 

I would skew towards builds with more ultimate damage, because ultimate damage is not affected by running comet runes 


# What are the best early game items?
Personally I would determine what my desired endgame build is first (see win conditions), then figure out which items in that build are also strong into the enemy ADC at 1 item.

- [PTA Alacrity Jinx TK_ULT]({{< ref "RawData/PTA Alacrity/Jinx TK_ULT" >}})
- [PTA Alacrity Draven TK_ULT]({{< ref "RawData/PTA Alacrity/Draven TK_ULT" >}})
- [PTA Bloodline Jinx TK_ULT]({{< ref "RawData/PTA Bloodline/Jinx TK_ULT" >}})
- [PTA Bloodline Draven TK_ULT]({{< ref "RawData/PTA Bloodline/Draven TK_ULT" >}})



# Q & A

## Why are there extra item components in the raw data?
I am trying to normalize the gold cost of different builds by "buying" additional item components with "extra gold". This has the side effect of giving a value to free item slots and rune choices 

Every item build is credited with:
- +900g (Vamp Scepter): If a build already has lifesteal, the 900g can be spent on ad components 
- +300g (Boots1): If a build already another source of movement speed, the 300g can be spent on ad components  
- +180g If Dorans Blade has been "sold", 180g is credited 

## How to read the raw data?

- **tk**: Time taken for Miss Fortune to kill this particular from full HP
- **ult**: Ultimate Damage done by Miss Fortune into this particular champion, starting from full HP
- **aaqaa**: Damage dealt after the second auto (aa + q + aa). If this value is blank, it may mean that the champion was killed with aa + q, in which case I did not record the aa + q + aa damage.
- **AdHp**: Miss Fortune's Effective HP against AD damage against the enemy champion. This is affected by how much armor pen the enemy champion is assumed to have bought in his build
- **AdHp/Tk**: Effective HP against AD damage divided by Time taken to kill. I am trying to express the idea that the longer we take to kill an enemy champion, the more damage we can expect to take from that enemy champion.
- **AdB**: Effective HP against AD *burst* damage. This does not account for healing, since we cannot heal through damage that kills us instantly
- **g**: Cost of the build in Gold

## What items does the algo overestimate?
Items with long cooldown active abilities. 

For example:
- Galeforce active damage is accounted for in the computation, but in a real game Galeforce may be on cooldown!
- Guardian Angel is assumed to be off cooldown for the purposes of the 50% base HP restore passive
- Shieldbow's Shield is assumed to be off cooldown
- Maw's Shield is assumed to be off cooldown
- Yoummu's bonus Lethality is assumed to fully charged (this is a more reasonable assumption given how fast it charges)

## What items does the algo underestimate?
Utility items. It is very difficult to put a gold value to utility items

For example:
- QSS's CC removal
- Duskblade's untargetable passive
- Edge of Night's spellshield
- Guardian Angel's revive passive (the 4s revive timer utility)
- Tenacity items
