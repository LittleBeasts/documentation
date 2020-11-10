The Item class will hold all the information an item needs. 
There will two general categories: One for consumable items (e.g. health potions or cages to catch beasts) and the other for item that can be used multiple times (like weapons for example).

The effects of item can be diverse so it will be difficult to plan everything that will be needed in order to create items that have all the information we will need in them.

An item will have the following variables:

```Java
String name

String spriteName

boolean consumable

boolean equipped

boolean unique

int amount

int amountOfUses (durability)

int[] bonusStats [healthPoints, speed, stamina, attack, defense, critBonus]
```
