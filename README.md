# SpaceHulkWFC
A Spacehulk map generator using wave function collapse to create both a map and a network graph of the map
Inspired by the [Space Hulk](https://en.wikipedia.org/wiki/Space_Hulk) game but intended to be used in a [Wrath & Glory](https://cubicle7games.com/our-games/wrath-glory) campaign.

I was impressed by the generator created by [LordFckHelmchen](https://github.com/LordFckHelmchen) [Wrath & Glory Space Hulk Generator](https://github.com/LordFckHelmchen/wrath-and-glory-space-hulk-generator) but the result didn't really match what I wanted.

The large rooms connected by thin corridors didn't really match the aesthetic I admired from space hulk.
It also didn't create any sort of room listing which I think is essential for planning a game to use the map.

Will be implemented as a SPA using pyiodide so that it can be easily reused.

1. Input
    1. Map size 
        1. x width in tiles
        2. y height in tiles
    2. Tile library
        1. 120 x 120 mm tiles.  Each tile being square and consisting of 40 x 40mm squares
    3. Constraints
        1. Rules for which tiles can be placed against each other tiles
    
2. Output
    1. Map
    2. Network Graph
        1. Each Node to have the x and y coordinates of the tile it refers to
        2. Export as json probably
    3. Base64 encoded hash of the map which can be used to reload the map in the generator so that the map can be extended or edited.
