Looting will be defined through a Loot table (a Json file) which holds every item and the corresponding informations.

The Loottable could look something like this:

```JSON
{   
    "itemTable": {
        "category": {
            "label": "string: labels the items cotained in this object, e.g: SPECIAL, RARE,...",
            "probability": "general propability for all items inside category",
            "items": [
                {
                    "id": "unique: identifies the item",
                    "name": "Ingame display name",
                    "description": "Describes what the item can do and what it is",
                    "dependencys": ["boolean Array which determines if the conditions for finding the item are fulfilled"],
                    "probability": "int: determines how likely it is to find the item in %",
                    "effects": "unique: What Effects does this item have if it get's used?",
                    "usage": "determines if the item is a consumable, a static item for buffing or a story related item"
                }
            ]
        }
    },
    "containerTable": {
        "#container": {
            "numberOfitems": "Max amount of items which can be found",
            "propabilitys": [
                "int: propability that the container has x items"
            ]
        }
    }
}
```
The looting algorithm would generate several different random numbers, to determine what items can be found inside the container the player is currently looking at:
1. How many items can be found
2. Category
3. Item 

The Category and Item gets rerolled for the number of items which can be found inside the container.
