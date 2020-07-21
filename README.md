# tile-world
a tile based world with sorta smart collision ig

a maze built with tiles. theres an array full of 1s and 0s (1 = tile, 0 = air)
the 1s get converted into tile objects, the 0s are left over
(idk if this is the right way to go about doing this)

in a big world, drawing all the individual tiles (whilst having to deal with 0s)
will really take a toll on the performance, which is why i want to find a way
to rid the map array of 0s, and to speed up drawing the tiles
however since the collision counts on indexes i can't really find a way to do that

since i can access any tile with an index, the player can get neighbouring
indexes and only check collision with those tiles, instead of checking
every single tile

the world is a top down maze that the player can navigate through
player is controlled by WASD keys
