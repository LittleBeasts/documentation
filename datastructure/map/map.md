## Software
The maps will be managed with the LITIengine utiLITI software. The map has to be created as \*.tmx file in a tile map editor and the used tiles also need to be imported as tileset it a \*.tsx format.
All the editing of tiles will be done in pixel editor like for instance Krita or just plain Paint. Then the map can be created with a tile map editor like tiled. 
The \*.tmx and \*.tsx are XML formats which store the information in plain text. The utiLITI software then exports all resources to a file (convetionally named "game.litidata") which can then be imported to the Java project with ```Resources.load``` and called with their in the utiLITI software created names.  

## Design Guidelines
To guaratee a universal validity to each map and an easy naming scheme to use in JAVA there needs to be a guideline for designing maps. (Generally important for work in *Tiled*)
* The maps have rectangular tiles
* The perspective will always be orthogonal
* Exit/Enter point should be visibly positioned
* *Layer* needs to be bottom to top and back to front
* If a character should be rendered behind a layer use: **RENDERTYPE : OVERLAY**
* Tileset for each regions must be homogeneous
## Technical Guidelines
(Important for work in *utiLITI*)
* *Spawnpoint* needs to be named after the region it leads from
* exit *Area* needs to be named after the region it leads to
* all impassable tiles need to be marked with *Collisionboxes*
## Development Guidelines
(For use in JAVA)
* save last used *Spawnpoint* in *GameLogic* for savegame


