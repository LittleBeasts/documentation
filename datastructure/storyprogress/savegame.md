# Savegame Datastructure

The state of the game will be saved as an XML file in which the necessary information will be reported to ensure that the game can be continued from the last spawn point of the player.

Attributes that need to be reported: 
* LitiPlayer
	* name
	* level
	* skills
* littleBeastTeam
	* name of each monster
	* beast stats
	* skills
	* level
* last spawnpoint / current screen
* player inventory
	* item
	* amount
	* equiped
* story progression
* dialogue progression
* chests opened? (not able to loot same chest multiple times)
* potential settings (music/volume, NSFW mode...)