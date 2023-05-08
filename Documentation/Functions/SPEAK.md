<sub>Authored by the Nous team</sub>

Usage: `SPEAK (<string>)`

The SPEAK function causes the Nous interpreter to return the specified string through the current default means of communication (verbal or text). This can be used to return system messages for debugging, or as the main purpose of the code. Leaving the string empty will cause a default string to be returned, which varies between Nous interpreters and can be set by operating on the variable `SPEAK.default`.

Example:
```
WHILE ([MIND.consciousness] > 0)
    {
    PERCEIVE ([MIND.consciousness] --)
    }
SPEAK ("Trance entered.")
WHILE ([SPIRIT.free_will] > 0)
    {
    PERCEIVE ([SPIRIT.free_will] --)
    }
SPEAK ("Free will suppressed.")
LINK [SPIRIT.species] AND [SPIRIT.name]
PERCEIVE ([SPIRIT.species] = "Drone")
UNLINK [SPIRIT.species] AND [SPIRIT.name]
SPEAK ("Reformatting complete. Drone ready for work.")
EXIT
```

The above code will reduce consciousness and free will to 0 as well as change the Nous interpreter's species and name, while causing them to provide feedback on the progress of these changes.
