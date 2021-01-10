## What is Craftia?

You are part of a crew of a space ship exploring the universe. Your ship has discovered and unexplored planet and has positioned itself in a hovering pattern over the planet's surface. You are part of the away team with a mission to explore the planet's surface. Unfortunately the ship is not in great condition. The left engine is having issues and food supplies are running low. The away team will have to make do with what it can find on the planet with a few exceptions. You can pick up a go kit with an elytra for gliding down to the surface, a compass and a lode stone to mark areas of interest and navigate back to them.

The ship's warp system is functional which allows you to warp back to the ship at any time.

## Arriving for the first time

When you join Craftia, you will start in the space ship and your personal spawn (not world spawn) will be set to the space ship. Get your go kit with the following command:

    /kits go

The go kit contains Elytra, a compass and a lode stone.

## Explore the planet surface

Wear elytra on your body so you can glide down to the surface and explore. At any time you can warp back to the space ship with the command:

    /warp ship

It takes 5 seconds for the space ship's warp system to tune in on your coordinates and initiate the warp. You must not be moving or be under attack during this time.

If you find a place of interest that you want to return to, place the lode stone and right-click with your compass. After warping back to the space ship (or going elsewhere on the map), you can now find your way back to this point.

You can get as many go kits as you want. This enables you to mark many places of interest with lode stones and finding them again with your compasses.

## Establishing a base

As you establish a base on the planet surface, it may become important to protect it from other explorers. Explorers have been know to raid other bases. The space ship has a force field protection system that allows each explorer to protect a cuboid area of up to 30,000 blocks. Create a force field protection around your base in the following way:

* Stand at one corner of your base and mark it with `//pos1`
* Move to the opposing corner and mark it with `//pos2`
* Claim the region with `/region claim <name-of-region>`

You may need to build up or dig down to position yourself correctly and fully capture the region you want to protect. See below for more details on regions.

## Warping to your base

The space ship warp system allows each explorer to mark the coordinates of their home base and warp directly to their base from the space ship. When you are standing in your base, mark your coordinates with:

    /sethome

Once this is set, you can now warp to your base from the space ship with the command:

    /warphome

You can only warp to your home coordinates from the space ship.

## Managing your region

To see what's part of your region, you can move around the map and run the command:

    /region info

If this command shows the name of your region and its details, it means you're inside your region. If it shows `__global__` it means you're outside your region. Use this command to see what is inside and outside of your region.




There are many commands available to manage this region.

There are several other ways to mark the area you want to claim. You can use all WorldEdit selection commands, e.g:

    //hpos1  - set first corner to block you are looking at
    //hpos2  - set opposing corner to block you are looking at
    //expand - expand an existing region up, down, east, west, north or south

