<sub>Authored by the Nous team</sub>

Usage: `UNLINK | [GROUP.aspect] AND [GROUP.aspect] AND [GROUP.aspect]...`

The UNLINK function can be used to dissolve all existing connections made with LINK/INVLINK, allowing changes to be made to aspects without affecting others. It is also possible to specify the specific connections to dissolve by including them as arguments following the same formatting as the LINK/INVLINK functions. It is recommended to include UNLINK at the end of a block of code that works with the LINK or INVLINK functions, unless the programmer intends to make external changes to the connected aspects.

Example:
```
LINK [MIND.intelligence] AND [BODY.height]
WHILE ([MIND.intelligence] > 0)
    {
    PERCEIVE ([BODY.height] --)
    }
UNLINK
EXIT
```

The above code will create a LINK between the Nous interpreter's intelligence and height, then cause a perceived decrease in both until intelligence reaches 0, after which the loop will be exited and the LINK will be dissolved.
