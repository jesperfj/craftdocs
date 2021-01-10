## What is Craftia?

Your space ship has discovered an unexplored planet and has positioned itself in a hovering pattern over the planet's surface. You are part of the away team with a mission to explore the planet's surface. Unfortunately the ship is not in great condition. The left engine is having issues and food supplies are running low. The away team will have to make do with what it can find on the planet. You can pick up a go kit with an elytra for gliding down to the surface, a compass and a lode stone to mark areas of interest and navigate back to them.

The ship's warp system is functional which allows you to warp back to the ship at any time.

## Arriving for the first time

When you join Craftia, you will start in the space ship and your personal spawn (not world spawn) will be set to the space ship. Get your go kit with the following command:

    /kits go

The go kit contains Elytra, a compass and a lode stone.

## Explore the planet surface

Wear elytra on your body so you can glide down to the surface and explore. At any time you can warp back to the space ship with the command:

    /warp ship

It takes 5 seconds for the space ship's warp system to tune in on your coordinates and initiate the warp. You must not be moving or be under attack during this time.

If you find a place of interest that you want to return to, place the lode stone and right-click with your compass. After warping back to the space ship (or going elsewhere on the map), your compass will guide you back to this point.

You can get as many go kits as you want. This enables you to mark many places of interest with lode stones and finding them again with your compasses.

## Establish a base

As you establish a base on the planet surface, it may become important to protect it from other explorers. Explorers have been know to raid other bases. The space ship has a force field protection system that allows each explorer to protect a cuboid area of up to 30,000 blocks. Create a force field protection around your base in the following way:

* Stand at one corner of your base and mark it with `//pos1`
* Move to the opposing corner and mark it with `//pos2`
* Claim the region with `/region claim <name-of-region>`

You may need to build up or dig down to position yourself correctly. See below for more details on regions. You can only have one region. If you change your mind and want to establish a base somewhere else, you need to delete the region you created and create a new one in another place. Delete your region with:

    /region delete <name-of-your-region>

## Warping to your base

The space ship warp system allows each explorer to mark the coordinates of their home base and warp directly to their base from the space ship. When you are standing in your base, mark your coordinates with:

    /sethome

Once this is set, you can now warp to your base from the space ship with the command:

    /warphome

You can only warp to your base from the space ship. If you are somewhere else on the planet surface and want to go to your base, first warp to the ship and then warp to your base from there.

## Managing your region

To see what's part of your region, you can move around the map and run the command:

    /region info

If this command shows the name of your region and its details, it means you're inside your region. If it fails or showes something else e.g. `__global__` then you're outside your region. Use this command to see what is inside and outside of your region.

To change the shape of your region, start by selecting your region:

    /region select <name-of-your-region>

Now you can change the shape of the region using any of the [WorldEdit selection commands](https://worldedit.enginehub.org/en/latest/usage/regions/selections/). For example, you can expand the region in one direction with the `//expand` command:

    //expand 4 west

to expand your region 4 blocks westwards or

    //expand vert 10

to expand your region 10 blocks upwards or 

    //expand vert -10

to expand downwards 10 blocks (you can use any other number). You can use `//contract` in a similar way. Once you have modified your selected area, it's important that you now actually redefine your region:

    /region redefine <name-of-your-region>

This is the command that actually sets the new dimensions of the region so don't forget it.

### Add members to your region

When you claim a region, you are the region's owner and nobody else can break or place blocks in the region. If you want another explorer to share access to your region you can add them as a member:

    /region addmember <name-of-your-region> <name-of-user>

You can remove them with 

    /region removemember <name-of-your-region> <name-of-user>

### Restrict Chest Access in your region

When you claim your region, only you and its members can open and close doors and break blocks. This means you can easily protect your base and prevent others from accessing chests by keeping them behind closed doors.

But if you forgot to close the door, then a stranger can walk in and open your chests. You can protect you chests with the following command:

    /region flag <name-of-your-region> -g nonmembers chest-access deny
