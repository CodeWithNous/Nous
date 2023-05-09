<sub>Authored by the Nous team</sub>

Usage: `DEFINE [String] AS ([any])`

The DEFINE command can be used to create a variable or function within a Nous script.

Example:
```
DEFINE "BIMBOFY" AS ({
    INVLINK [MIND.intelligence] AND [MIND.libido]
    WHILE ([MIND.intelligence] > 0)
        {
        PERCEIVE ([MIND.intelligence] --)
        }
    UNLINK [MIND.intelligence] AND [MIND.libido]
})
EXPORT BIMBOFY
EXIT
```

The above code will define "BIMBOFY" a script to lower intelligence and increase libido, and then export it for other scripts to use.