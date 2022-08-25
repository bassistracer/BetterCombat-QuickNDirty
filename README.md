# BetterCombat-QuickNDirty
A quick n' dirty, unofficial guide to adding your own Better Combat compat. Not recommended.

Note: It's generally recommended the mod maker does it themselves, as it helps prevent things like. Y'know. Spoilers. Or what-have-you. Seriously, ask them to make a compat before trying this to keep stability, as they know the ins-and-outs of every weapon.

1. Get a data-pack loading mod such as kubejs or OpenLoader for simplicity.
2. Get the weapon tag from the mod you wanna implement. Can be done by getting its NBT data by pressing F3+H to enable NBT tooltips.
3. Go through the usual step of making your average datapack, look it up if you don't know how to do that.

3a. In the end (this is assuming you're using OpenLoader), it should be data\(YourDataPackName)\data\(the same mod name that its data folder uses)\weapon_attributes\(Your_Weapon_Here).json

3b. In other words, data\LittleTimmysBCCompat\data\BestestSwordEva\weapon_attributes\The_OP_Sword.json

4. Simply use a [preset.](https://github.com/ZsoltMolnarrr/BetterCombat/blob/1.19.X/README.md#using-a-preset)

5. ???
6. Profit!


Protip:
If a weapon has an ability used by right clicking that doesn't allow off-hand items to be used such as shields, making it two-handed always helps. You can check what presets are two-handed by clicking on them in the github and looking for the flag that shows it. 

If something like a spear, etc. is practically gutting through your body while you're swinging it, consider changing it to one-hand. This is mainly to do with the mod's weapon itself not having much range, and you'll have to discuss with the modder about that.

If there's a compat available for future versions but not, say, 1.18.2, at least as of right now you can just grab the weapon attributes from the latest .jar and throw 'em in your own datapack. Keep in mind that this may cause stability issues as Better Combat gets more advanced.

And, once you're sure everything works, make sure to make a Pull Request on the mod maker's github and add 'em in so they can be in the main mod as god intended.
