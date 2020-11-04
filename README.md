# documentation
This is the documentation for the littleBeasts game

# Plan
 - Oberfläche im Spiel: 
  * Kampfoberfläche: 
    * Attacke wählen → Ergebnis: Gewonnen oder nicht.
    * ~~Lebensleiste~~ (1LP → Getroffen heißt verloren)
- Events, die Damage machen, Monster kreieren, 
- Monster kann attacke wählen
- Player kann attacke wählen
- Monster bekommt Schaden (Anzeige nicht notwendig → 2-3 Treffer höchstens)
- Fangen geht: Attacke fangen → gefangen oder nicht.

- Über Server laufen lassen: Aktion auswählen, Ergebnis sehen, Rest im Client dargestellt und verwaltet. Frage ob es ein Monster gibt entscheidet der Client.
- JSON als Serialisierung als 1. Schritt, 1. Byte der Nachricht gibt die Version (um die Serialisierung ändern zu können).

