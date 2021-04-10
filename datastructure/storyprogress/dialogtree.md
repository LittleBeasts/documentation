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

I'm going to use propose another Datastructure for Dialogs, which I think is easier to use:

```JSON

{
  "DialogTree": {
    "Day 1": {
      "Heading": "Day 1",
      "Szene 1": {
        "Heading": "At Home",
        "Dialog 1": [
          {
            "Speaker": "<name>",
            "Text": "Hey sweety, did you also have a strange dream?"
          },
          {
            "Speaker": "Nike",
            "Text": "Meow",
          },
          {
            "Speaker": "<name>",
            "Text": "Something is not right, I should talk to the Professor."
          },
          {
            "Speaker": "Nike",
            "Text": "Meow?",
          },
          {
            "Speaker": "<name>",
            "Text": "Let's got to his office!"
          },
        ],
        "Trigger": "Nike"
      },
      "Tutorial":{
        "...":"..."
      }
    }
  },
  "Greetings": {
    "K": ["Der Klimawandel ist eine Lüge!.. ähhh Ich meine MEOW?"],
    "Prof W.":{
      "Standard": ["Hmmm... Ah yes.. No... Oh Hi <name> I didn't saw you!", "YES IT WORKS!"],
      "Tips": {
        "Day 1": {
          "Szene 1": "Go to Prof W"
        }
      }
    } 
  }
}

```