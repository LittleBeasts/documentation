The dialog tree will be stored as a JSON file and will then be presented to the player. When a dialog option is chosen it is saved in the state of the NPC.

```JSON
{
  "dialogtree": {
    "character": {
      "npcname": "Harald",
      "dialog": {
        "firstTree": {
          "greeting": "Hello, I'm Harald, what do you want?",
          "options": {
            "option1": {
              "option": "Why are you here?",
              "answer": "What is it your business, beat it!"
            },
            "option2": {}
          }
        },
        "secondTree": ""
      }
    }
  }
}
```

The logic for the dialog needs to be done in JAVA. 

