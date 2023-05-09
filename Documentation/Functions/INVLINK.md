<sub>Authored by the Nous team</sub>

Usage: `INVLINK [GROUP.aspect] AND [GROUP.aspect] | AND [GROUP.aspect]...`

The INVLINK function is similar to the LINK function; however, the connections created with INVLINK cause an inverse change to be applied to linked aspects after a change is applied to one. Like LINK, INVLINK can connect different data types, but will only reflect changes if it would be valid to do so. Additionally, INVLINK connections will function identically to LINK connections when using the `=` operator. Note that when using INVLINK with three or more aspects, only the first aspect will be inverted, so to speak; so a change to aspect 2 will apply an equal change to aspect 3 but an inverse change to aspect 1, and so on.

Example:
```
INVLINK [MIND.intelligence] AND [BODY.breasts/size] AND [MIND.libido]
WHILE ([MIND.intelligence] > 0)
    {
    PERCEIVE ([MIND.intelligence] --)
    }
UNLINK [MIND.intelligence] AND [BODY.breasts/size] AND [MIND.libido]
EXIT
```

The above code will cause the Nous interpreter to perceive their breast size and libido as increasing, while their intelligence is inversely perceived as decreasing.
