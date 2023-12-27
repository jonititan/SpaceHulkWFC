# SpaceHulkWFC
A Spacehulk map generator using wave function collapse to create both a map and a network graph of the map

Will be implemented as a SPA using pyiodide so that it can be easily reused.

Input
  Map size 
    x width in tiles
    y height in tiles
  Tile library
    120 x 120 mm tiles.  Each tile being square and consisting of 40 x 40mm squares
  Constraints
    Rules for which tiles can be placed against each other tiles
    
Output
  Map
  Network Graph
    Each Node to have the x and y coordinates of the tile it refers to
    Export as json probably
  Base64 encoded hash of the map which can be used to reload the map in the generator so that the map can be extended or edited.
