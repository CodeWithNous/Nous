<sub>Authored by the Nous team</sub>

Usage: `... NOTE <text>`

The NOTE function allows you to put notes in your text that will not be seen by the program while it is running. This is useful for reminding yourself what lines of code do, as well as for informing others what things do if you share code.

Example:
```
NOTE The below code will create a LINK between the Nous interpreter's intelligence and height, 
NOTE then cause a perceived decrease in both until intelligence reaches 0, 
NOTE after which the loop will be exited and the LINK will be dissolved.
LINK [MIND.intelligence] AND [BODY.height] NOTE link intelligence and height
WHILE ([MIND.intelligence] > 0)
    {
    PERCEIVE ([BODY.height] --) NOTE perceive decrease
    }
UNLINK [MIND.intelligence] AND [BODY.height] NOTE unlink when done
EXIT NOTE stop running the script
```
