<sub>Authored by the Nous team</sub>

Usage: `UNLINK [GROUP.aspect] AND [GROUP.aspect] | AND [GROUP.aspect]...`

The UNLINK function can be used to dissolve an existing connection made with LINK/INVLINK, allowing changes to be made to a specified aspect without also affecting the other. It is recommended to include UNLINK at the end of a block of code that works with the LINK or INVLINK functions, unless the programmer intends to make external changes to the connected aspects.

Example:
```
LINK [MIND.intelligence] AND [BODY.height]
WHILE [MIND.intelligence] > 0
    {
    PERCEIVE ([BODY.height] --)
    }
UNLINK [MIND.intelligence] AND [BODY.height]
EXIT
```

The above code will create a LINK between the Nous interpreter's intelligence and height, then cause a perceived decrease in both until intelligence reaches 0, after which the loop will be exited and the LINK will be dissolved.