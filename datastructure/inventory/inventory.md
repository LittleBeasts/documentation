Inventor is a class which holds all item a player has. 
```Java

Item armorShoulder;
Item armorShoes;
Item armorLegs;
Item armorChest;
Item armorHead;
Item weapon;

Slot[] slots = [ //Slot list to save inventory Items
    slot(){ // Each slot can hold 1 Item but several amounts of the specified item
        Item item,
        int amount
    }
]

```
