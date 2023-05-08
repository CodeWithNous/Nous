<sub>Authored by the Nous team</sub>

Usage: `RUN (path/filename.nu)`

The RUN command can be used to execute a script file stored in a Nous interpreter.

Example:
```
WRITE (Programs/bimbofy.nu)
    {
    INVLINK [MIND.intelligence] AND [MIND.libido]
    WHILE ([MIND.intelligence] > 0)
        {
        PERCEIVE ([MIND.intelligence] --)
        }
    UNLINK [MIND.intelligence] AND [MIND.libido]
    EXIT
    }
RUN (Programs/bimbofy.nu)
EXIT
```

The above code will create a script to lower intelligence and increase libido, and then run the script.
