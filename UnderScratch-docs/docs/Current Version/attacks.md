---
title: Attacks
sidebar_position: 4
---
:::note[Stub]
This Page may be incomplete in some Areas.
:::
:::warning[WIP]
This Feature is incomplete.
:::

## Atacks
Oh boy, this is a long one. 
Attacks in Underscratch are handled in a somewhat uniqe way.  
There is a Manager OBject, that tells the game what attacks to perform, it uses a list.  
Each attack is its own separate object, this is done to give Developers more freedom in how they design their attacks (and bc its easier to do but lets not talk abt that).  

## Attack Manager
This is the Manager Object, it has a script that adds all the attacks you want to have onto a list.  
If you want to add an Attack, add a block to add the name of your attack objects name to the list (called "attack list"), and you should be good to go.  
If the "attack list" list has played the last attack, it will automatically set the index back to 1, repeating the attacks in the given order.
Note that the list of attacks is dependendt on the order in the script, there is no ID system of any sorts.

## Attack Objects
Each Attack is its own Object, inside of the Object, you need the following scripts pasted in (you can copy them form the "bullet" object):
<div style={{ display: 'flex' }}>
  <img src="/img/attacks-mandatory1.png" alt="First Image" style={{ width: '48%', height: '200px', objectFit: 'contain', marginRight: '2%' }} />
  <img src="/img/attacks-mandatory2.png" alt="Second Image" style={{ width: '50%', height: '150px', objectFit: 'contain' }} />
</div>
Then, you simply write the logic for the bullets in a "when i start as a clone" script, furthermore, you can adjust the first script (left) to spawn more clones, maybe have it add to a variable and if said variable is a certain ammount change costumes, you decide!  
Attacks are the most versatile part of Underscratch, you can truly make anything you want!

## Attack Colors
:::danger[caution]
As of version a1.0.0 Blue and Orange attacks are not functional.
:::
Currently, the type a bullet has is fully dependent on its color.  
The Colors are as follows:
- White - Normal attack, deals "bullet_normal_dmg"'s damadge:   <span style={{ backgroundColor: '#ffffff', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span>  #ffffff
- Blue - damadges the player only if they are moving whilst touching it, deals "bullet_blue_dmg"'s damadge: <span style={{ backgroundColor: '#3f51ff', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #3f51ff
- orange - damdges the player only if they arent moving whilst touching it, deals "bullet_orange_dmg"'s damadge:     <span style={{ backgroundColor: '#ffa500', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #ffa500
- Green - Heals the player "bullet_green_heal"'s value:  <span style={{ backgroundColor: '#00ff00', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #00ff00
- Yellow - Destroyable by the Yellow Soul, if touched, deal "soul_yellow_dmg"'s damdge:  <span style={{ backgroundColor: '#ffd600', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #ffd600

