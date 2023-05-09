<sub>Authored by the Nous team</sub>

Usage: `EXPORT [any] <AS [String|DEFAULT]>`

The `EXPORT` command can be used to export a variable or function from one Nous script to be `IMPORT`ed into another. Exports can either be named, or assumed to be the default export for the file.

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
EXPORT BIMBOFY AS DEFAULT
EXIT
```

The above code will define "BIMBOFY" a script to lower intelligence and increase libido, and then export it for other scripts to use.