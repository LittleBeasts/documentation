To properly create savegame files there needs to be a structure to save the game state and with it the story progress.

For the story progress a  JSON file will save how far the progress is with each story element.

```JSON
{
  "mainplot":0,
  "dunwich":{
    "plot1":0,
    "plot2":0
  },
  "etc":0
}
```

The story progrss will be saved as an integer which will be incremented, when there is story progress. The JSON is divided into the different plots, which then can be updated in parallel. When the story has forks the integer can be set to a specific value instead of just incrementing it. This allows for complex storylines but there will be a need for a complex story board where the story is plotted out.
