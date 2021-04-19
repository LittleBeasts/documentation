The Item class will hold all the information an item needs. 
There will two general categories: One for consumable items (e.g. health potions or cages to catch beasts) and the other for item that can be used multiple times (like weapons for example).

The effects of item can be diverse so it will be difficult to plan everything that will be needed in order to create items that have all the information we will need in them.

An item will have the following variables:

```Java
String name

String spriteName

boolean equipped

boolean unique

Enum type {ShoulderArmor, Weapon, Consumable...}

int amount

int amountOfUses (durability)

int[] bonusStats [healthPoints, speed, stamina, attack, defense, critBonus]

String description

Enum effects {UNLIMITED_POWER}
```

Now that we have a basic structure for items, which we can use in game. We need a place to store all the available Items and their attributes. This will be achieved by the following JSON file:

```JSON
{
    "item": {
        "name": "item_name",
        "spriteName": "sprite_name",
        "type": "item_type",
        "uses": 64,
        "bonusStats": ["healthPoints", "speed", "stamina", "attack", "defense", "critBonus"],
        "unique": true,
        "description":"item_description",
        "effects":"item_effect",
        "rarity":"RARE"
    },
    "ring": {
        "name": "golden Ring",
        "spriteName": "sprite_golden_ring",
        "type": "Jewelry",
        "uses": 64,
        "bonusStats": [100, 100, 100, 100, 100, 100],
        "unique": true,
        "description":"Ash nazg durbatulûk, ash nazg gimbatul, ash nazg thrakatulûk, agh burzum-ishi krimpatul. One Ring to rule them all, One ring to find them; One ring to bring them all and in the darkness bind them.",
        "effects":"UNLIMITIED_POWER",
        "rarity":"LEGENDARY"
    }
}
```
Note that some attributes of Items aren't stored in the Itemclass of the Calculation Engine, e.g rarity, because they aren't of effect for the player, once they aquired the item. These Stats will only be used while generating the Players loot. Which is described in [looting.md](https://github.com/LittleBeasts/documentation/blob/master/datastructure/inventory/looting.md)