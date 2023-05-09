<sub>Authored by the Nous team</sub>

Usage: `EXIT | (<file>)`

The EXIT function is used to stop the execution of a script. It must be present at the end point of a file in order to ensure the Nous interpreter stops running the script when intended. It can also be used to stop a script prematurely. Additionally, if a script is running as a background process via the `RUN` function's `async` flag, a file path can be specified to stop the execution of the specified script.

Example:
```
WHILE ([MIND.intelligence] > 0)
    {
    PERCEIVE ([MIND.intelligence] --)
    }
IF ([MIND.libido] = 100)
    {
    EXIT
    }
ELSE
    {
    WHILE ([MIND.libido] < 100)
        {
        PERCEIVE ([MIND.libido] ++)
        }
    }
EXIT
```

The above code will lower the Nous interpreter's intelligence to 0, and then abort if libido is already at 100, otherwise it will also raise libido to 100.
