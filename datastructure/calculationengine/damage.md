# Properties of a Damage

**Attackers**: two different figures involved in the attack

**attack**: [see description](https://github.com/LittleBeasts/documentation/wiki/Attacks) 

**Damage amount**: first the damage amount is set to the base damage amount, given by the attack.

**Strength**: attacker-related property (can be gained from object references of the attackers), increases the damage amount.

**Resistence**:  attacker-related property (can be gained from object references of the attackers), decreases the damage amount.

**Accuracy**: attack-related property, high accuracy increases the damage amount.

**Critical Chance**: attack-related property, gets multiplied with a random number. If result is above a certain threshold, damage amount increases heavily.


After damage amount has been calculated, the health points of the attacked figur get decreased by the value of damage amount.
