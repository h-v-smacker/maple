# Maple
Maple Tree for Minetest by ExeterDad

This mod adds a maple tree to the minetest game. Originally written for the Hometown server (http://hometownserver.com/) by ExeterDad (https://forum.minetest.net/memberlist.php?mode=viewprofile&u=10544).

## The tree

![Maple Tree](https://github.com/h-v-smacker/maple/blob/master/maple_in_the_wild.jpg)

## Bonemeal

The mod now registers itself with the bonemeal API, and saplings should be recognized automatically.

~~If you are using the bonemeal mod, you can add this to mods.lua to enable maple support:~~

```
if minetest.get_modpath("maple") then
	bonemeal:add_sapling({
		{"maple:maple_sapling", maple.grow_sapling, "soil"},
	})
end
```