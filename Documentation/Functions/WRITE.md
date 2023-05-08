<sub>Authored by the Nous team</sub>

Usage: `WRITE (path/filename.nu) {}`

The WRITE function can be used to create a .nu file in the specified directory of the Nous interpreter. All file paths are relative to the working directory, and leaving the path blank will create the file in the working directory.

Example:
```
WRITE (Programs/intdrain.nu)
    {
    WHILE ([MIND.intelligence] > 0)
        {
        PERCEIVE ([MIND.intelligence] --)
        }
    EXIT
    }
EXIT
```

The above code will create the file "intdrain.nu" in the Nous interpreter's "Programs" folder, which, when run, will gradually cause a decrease in intelligence until it can no longer be decreased.
