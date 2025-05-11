---
title: Enemies
sidebar_position: 3
---
:::note[Stub]
This Page may be incomplete in some Areas.
:::
:::warning[WIP]
This Feature is incomplete.
:::

## Enemy Object
In Underscratch, the "enemy1" object is used for the enemy of the fight.  
inside of the object, there you can change the costume, and the enemies stats, these are saved in a list and are as follows:

### Enemy Stats:
- Name: used for the name in the Menu's
- Hp and MaxHp: self explanatory, they can be different values
- atk: this currently has no use, tho it will later be used for the check act, it does not affect the damadge of the bullets, that is handled through another variable
- def: the enemies defense, gets subtracted from the attack value of the player (after they have landed the hit)
- act2 - 6: currently unused, these will be used for the acts that the player will be able to perform, regardless, here is the structure of each act block:
    - line 1: name of the act
    - line 2-4: the text that displays when the act is performed, leaving one empty skips it
    - line 5: how much it "satisfies" the enemy (i.e.: the mercy bar in deltarune), percentage based

thats pretty much it lol.