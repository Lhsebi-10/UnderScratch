---
title: General Concepts
sidebar_position: 2
---

:::note[Stub]
This Page may be incomplete in some Areas.
:::

### Attacks
- Attacks are handled by the "Attack Manager" Object.  
- Each Attack needs to be one separate Object
- It contains a "On Green Flag clicked" Script that clears the "attack list" array.  
- For attacks to show up, the names of your attack objects need to be added to the "attack list" array when the green flag is clicked. 
- The "attack index" variable is responsible for deciding which attack in the "attack list" array is used next. Editing of the variable is genrally endorsed (i.e.: for Heal attacks or Attacks that generally dotn pregress the fight)
  
For more Information on the Structure of Attacks, read [link].

### Bullet types
:::danger[caution]
As of version a1.0.0 Blue and Orange attacks are not functional.
:::
Currently, the type a bullet has is fully dependent on its color.  
The Colors are as follows:
- White - Normal:   <span style={{ backgroundColor: '#ffffff', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span>  #ffffff
- Blue - [blue stop signs]: <span style={{ backgroundColor: '#3f51ff', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #3f51ff
- orange - Movement:     <span style={{ backgroundColor: '#ffa500', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #ffa500
- Green - Healing:  <span style={{ backgroundColor: '#00ff00', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #00ff00
- Yellow - Destroyable by the Yellow Soul:  <span style={{ backgroundColor: '#ffd600', display: 'inline-block', width: '1em', height: '1em', border: '1px solid #ccc', marginLeft: '0.5em' }}></span> #ffd600

For more Information read [link].


### Turns
- There 2 states for the "turn" variable to be in:
    - player
        - the player is in control, they can go through the menus, fight, act, use an item and spare
    - enemy
        - the enemy is in control, the attack in the "attack list" array that coresponds to the "attack index" is activated.
        