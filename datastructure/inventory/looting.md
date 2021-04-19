Looting will be defined through a Loot table (a Json file) which holds every item and the corresponding informations.

The Loottable could look something like this:

```JSON
{   
    "itemTable": {
        "#rarity": {
            "label": "string: labels the items cotained in this object, e.g: SPECIAL, RARE,...",
            "probability": "general propability for all items inside category",
        }
    },
    "containerTable": {
        "#container": {
            "numberOfitems": "Max amount of items which can be found",
            "propabilitys": [
                "int: propability that the container has x items"                
            ],
            "item":"defined drop (can be ommited)",
            "rarity":"defined rarity (can be ommited)"
        }
    }
}
```
The looting algorithm would generate several different random numbers, to determine what items can be found inside the container the player is currently looking at:
1. How many items can be found
2. Category
3. Item 

The Category and Item gets rerolled for the number of items which can be found inside the container.
