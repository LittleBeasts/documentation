```JSON

{
  "dialogTree": {
    "day1": {
      "heading": "Day 1",
      "scene1": {
        "heading": "At Home",
        "dialog1": [
          {
            "speaker": "$name",
            "text": "Hey sweety, did you also have a strange dream?"
          },
          {
            "speaker": "Nike",
            "text": "Meow",
          },
          {
            "speaker": "$name",
            "text": "Something is not right, I should talk to the Professor."
          },
          {
            "speaker": "Nike",
            "text": "Meow?",
          },
          {
            "speaker": "$name",
            "text": "Let's got to his office!"
          },
        ],
        "trigger":{
          "Nike": "dialog1"
        }
      },
      "tutorial":{
        "...":"..."
      }
    }
  },
  "default": {
    "K": {
      "greetings": ["Der Klimawandel ist eine Lüge!.. ähhh Ich meine MEOW?"],
      "tips": {
        "day1": {
          "scene1": "Go to Prof W"
        }
      }
    },
    "ProfW":{
      "greetings": ["Hmmm... Ah yes.. No... Oh Hi <name> I didn't saw you!", "YES IT WORKS!"],
      "tips": {
        "day1": {
          "scene1": "Go to Prof W"
        }
      }
    } 
  }
}

```