---
title: Attacks and you
sidebar_position: 1
---
:::note[Stub]
This Page may be incomplete in some Areas.
:::

Welcome, in this Tutorial, you will create your very own attack to use in your Fight!

What you'll need:
- the latest version of UnderScratch (as of writing this, a1.0.0)
- Turbowarp, or any other Scratch mod that is compatible with the custom extensions:
    - more comparisons
    - sensing+
    - stretch
    - Box2d physics (by griffpatch)
    - comment blocks
- around 5 minutes of time
- *✨creativity✨*

Open UnderScratch and continue to step 1.

## Step 1: getting the attack framework ready

once in UnderScratch, duplicate the "bullet" object and name it "MyAttack".  
it should now look like this:

![thisissoeasy](/img/bulletsandyou-step1.png)

Now, change the "bullet" text in the following script to "MyAttack:

![bruh](/img/attacksandyou-step1-2.png)

After thats done, move on to Step 2!

## Step 2: writing the attack into the list

Now, we will need to go to the "Attack manager" object, simply click on it.  
Once there, you should see this script:

![urmom](/img/urmom.png)

Attach the block under the script and put in "MyAttack" into the white text field.  
Afterwards, go to step 3!

## Step 3: making your attack

Now its time for the actual fun part!
Place a "when i start as a clone" block and start writing whatever things you want your attack to do.
remember that the attack starts off hidden, so use a "show" block first, furthermore, its position is in the middle of the screen, keep that in mind when planning your attack, however, you can just use a "go to..." block.

After writing the code you want for your attack, add the "broadcast [end enemy attack v]" block to the end of your script, or drag a new one if its missing.  
Heres an example of a finished attack:

![balala](/img/balala.png)

## Step 4: test it out!

Now, start the project, attack the Poseur and see your attack in action!
