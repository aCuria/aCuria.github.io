---
weight: 3
bookToc: false
bookCollapseSection: true
---
# Subsections

{{< section >}}

# Introduction
This is a guide on how to use the raw data. 

I am going to try to explain "how to fish" aka "how to come up with what build to use yourself"

# What do the numbers on the subfolder mean?
"13.15.1" Means patch 13.15. If the third number is 0, it represents PBE data. A '1' usually means the release patch, and above 1 usually means there was some kind of hotfix. I use the same numbers from the riot's data dump for this.

# What is the best build?
There is no true "Best" Build for all games. The "Best" build is a situational one depending on the win condition of that particular game. For example:

## Win Condition: Not dying to the fed assasin = win game 

Use a Build with high Effective HP against Burst. Look at "TK_ADEHP_BURST" (into AP assasins) and "TK_APEHP_BURST" (into AD assasins). 

This data represents the pareto curve for the time taken to kill (TK) against the effective HP against burst. "Against Burst" means we ignore effects from lifesteal, since we cannot lifesteal against instant damage. This data uses pen and rune information from the enemy champion

Note that we may have to stare at TK_ADEHP_BURST data against the tank to get the TK information from the tank with more anti burst oriented items included in the build... then compare that to the TK_ADEHP_BURST from the assasin. This is for fighting against teams with both tanks and assasins 

## Win Condition: Taking down the fed Riven / Insert Bruiser Here = win game 

If the bruiser touches us, we are "supposed" to die. Therefore we need to be able to kill the bruiser in the small time window that our support buys for us through CC effects. The best way to do this is usually to use a glass cannon build that kills in a minimum amount of time, so that the bruiser has the smallest possible window to kill us. Look at the "TKILL" data for this.

Note that movement speed is also sometimes useful to extend the amount of time the bruiser takes to reach us.


## Win Condition: Successfully Duel dps champions = win game 

In the late game, use builds with a fast kill time to effective HP ratio (TK_ADEHP_D_TK)


## Win Condition: Taking down the fed tank = win game 

Use an anti tank build. We dont want to get killed by the tank either, so effective HP against the tank's damage type is important. Wits end type items are very good against thornmail, because tanks dont really build void staff. 

## Win Condition: Surviving Lane = win game 
This happens when facing an enemy ADC who has a strong early game and weak late game. One example would be Draven

Usually some comet build variant is best for this, expecially into immobile champions who do not have a dash to avoid E and comet damage.

That said I really do not like playing comet because it does not scale well. 


# What are the best early game items?
There is no fixed way to go about this, if your games usually end early (1/2/3 items) then maybe you want to hit your powerspike at 2/3 items 

If your games go late then determine what the ultimate endgame build is first (see win conditions), then figure out which items in that build are also strongest at 1/2/3 item.

The most successful builds will be strong early game and scale well enough late game.

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
- Galeforce active damage is accounted for in the computation, but in a real game Galeforce may be on cooldown. Galeforce's active is assumed to be off cooldown, and used for regular damage 
- Guardian Angel is assumed to be off cooldown for the purposes of the 50% base HP restore passive
- Shieldbow's Shield is assumed to be off cooldown
- Maw's Shield is assumed to be off cooldown
- Yoummu's bonus Lethality is assumed to be on cooldown for dps calculations because it only lasts a pitiful 3s. We assume it works for ultimate.

## What items does the algo underestimate?
Utility items. It is very difficult to put a gold value to utility items

For example:
- QSS's CC removal
- Duskblade's untargetable passive
- Edge of Night's spellshield
- Guardian Angel's revive passive (the 4s revive timer utility)
- Tenacity items
- Mana from Manamune and Essence Reaver 
