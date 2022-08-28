# A quick n' dirty, unofficial guide to adding your own Better Combat compat. Not recommended.
Seriously, if you encounter issues, don't go to Daedelus! This guide is unofficial.

Note: It's generally recommended the mod maker does it themselves, and not players, as they know the ins-and-outs of every weapon, to help ensure mod stability. These are, by all means, experimental settings. Here be dragons!

# Method 1:
Go to your Better Combat config, go to ```fallback_compatability.json```, and add the "regex" of the weapon to where it should be. You should be able to figure it out with context clues.
The "regex" is more like the end of a weapon name. So if you wanted to add, say, all Excavators to a certain preset, you'd just simply put in excavators.

So, basically, you'd see the regex that has ```"mace|hammer|flail",```, and you'd just do this: ```"mace|hammer|flail|excavator",```


# Method 2:
1. Get a data-pack loading mod such as kubejs or OpenLoader for simplicity. Paxi for Forge also works if you're already using Yung's stuff.
2. Get the weapon tag from the mod you wanna implement. Can be done by getting its NBT data by pressing F3+H to enable NBT tooltips.
3. Go through the usual step of making your average datapack, look it up if you don't know how to do that.

3a. In the end (this is assuming you're using OpenLoader), it should be ```data\(YourDataPackName)\data\(the same mod name that its data folder uses)\weapon_attributes\(Your_Weapon_Here).json```

3b. In other words, ```data\LittleTimmysBCCompat\data\BestestSwordEva\weapon_attributes\The_OP_Sword.json```

4. Simply use a [preset.](https://github.com/ZsoltMolnarrr/BetterCombat/blob/1.19.X/README.md#using-a-preset)

5. ???
6. Profit!


# Protips:
If a weapon has an ability used by right clicking that doesn't allow off-hand items to be used such as shields, making it two-handed always helps. You can check what presets are two-handed by clicking on them in the github and looking for the flag that shows it. 

If something like a spear, etc. is practically gutting through your body while you're swinging it, consider changing it to one-hand. This is mainly to do with the mod's weapon itself not having much range, and you'll have to discuss with the modder about that.

If a weapon just looks weird when you're swinging it, it could be due to its own custom weapon animations in its own mod.

The attack speed attribute is retrieved from Vanilla Minecraft attributes.
To change the speed of a weapon, you have two options:
A) If it is a mod weapon, change the code of the mod to have a different speed
B) Assign new attack speed attribute to the weapon via NBT

Seriously, if you encounter any issues, just ask the mod developer to add Better Combat support instead!

If there's a compat available for future versions but not, say, 1.18.2, at least as of right now you can just grab the weapon attributes from the latest .jar and throw 'em in your own datapack. Keep in mind that this may cause stability issues as Better Combat gets more advanced.

And, once you're sure everything works, make sure to make a Pull Request on the mod maker's github and add 'em in so they can be in the main mod as god intended.
