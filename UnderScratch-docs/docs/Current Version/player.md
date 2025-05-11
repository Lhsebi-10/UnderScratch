---
title: Player
sidebar_position: 1
---
:::note[Stub]
This Page may be incomplete in some Areas.
:::
:::warning[WIP]
This Feature is incomplete.
:::

In Underscratch, the Player is the name given to the "SOUL" Object / Sprite.  
The SOUL Object mainly controls the Players movement, both in the enemy's turn and (partially) in the players turn.  
Furthermore, it handles the blue souls gravity and the appearance of each soul mode.  
It currently also handles most of the code for detcting if conact with a specific bullet has been made, however this will be changed soon, possibly in [a2.0.0].  
Another thing that the SOUL object currently controls is the debug menu and debug options, for more information on that please read [LINK].

## Starting atributes

The SOUL object also holds a small script with the starting paramters.  
These are as follows:
- player_atk:  
    The Players Attack value.
    :::info[notice]
    The damadge formula is different to the one used in Undertale (and possibly Deltarune)!  
    The Atk is not squared like in Undertale, so if you land a critical hit with 25 atk you will deal 25 damage!
    :::  

- player_speed:
    :::warning[caution]
    as of a1.0.0 this variable is not functional, this will be fixed soon!
    :::  
    How fast the Soul moves during an attack.

- soul_mode:  
    The soul mode that is active when the fight starts.

- soul_blue_max-jumps:  
    The maximum ammount of Jumps you can perform in the blue soul mode before having to land again.

- soul_yellow_direction:  
    The starting direction of the yellow Soul.

An Image of the script:

![Starting Parameters](/img/starting-parameters.png)

## Yellow Soul Bullet controller
:::danger[DNE (Do not edit)]
This is simply an explanation of an Object or Function, it is not to be edited!
:::
This is a separate Object in Underscratch, however it is used for the Soul, specifically the yellow mode (no shit).  
It is used as the Bullets in said mode, and it also adjust its rotation and trajectory based on the Souls orientation in the yellow mode (wasd). 

## Soul Damadge controller

This, too is a separate Object, it is used to set the damadge of certain attacks for the Player.  
Simply adjust the variable coresponding with the type of attack you want to change the damadge of (i.e.: normal bullet damadge -> soul_normal_dmg).  
Please only edit this part of the code, as editing the other 2 scripts could break things.  
The following is an image of said Code:

![The "script" for changing the dmadge ammount](/img/Soul-damadge-controller.png)