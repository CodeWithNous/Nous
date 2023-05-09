<sub>Authored by the Nous team</sub>

Usage: `RUN (path/filename.nu | [<flag(s)>])`

The RUN function can be used to execute a script file stored in a Nous interpreter. In addition to a file to run, various flags for running those files can optionally be specified. Flags and their effects are as follows.

---

`async`: Runs the specified file in the background without pausing the execution of the current script. Typically this means the execution of the specified script will be slowed down to complete at an externally defined end-point rather than being executing as fast as the Nous interpreter can process.

`unaware`: Runs the specified script, but prevents the Nous interpreter from knowing that they're running the script; this typically means they won't notice the effects of the script either. It is recommended to only use this flag for scripts whose effects are apparent even without the Nous interpreter being aware of them, such as scripts that change MIND aspects/qualities or contain the `ACT` or `SPEAK` functions.

---

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
RUN (Programs/bimbofy.nu [unaware])
EXIT
```

The above code will create a script to lower intelligence and increase libido, and then run the script without the Nous interpreter's knowledge.