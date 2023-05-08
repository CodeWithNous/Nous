<sub>Authored by the Nous team</sub>

USAGE: `RELEASE [GROUP.aspect]`

The RELEASE function will cause the specified aspect (or all aspects if none is specified) to no longer be affected by Nous code until otherwise specified. This is a very important safety function that should be run as soon as the control of Nous code is no longer desired, as the changes would otherwise remain in place indefinitely. AND can be used to execute RELEASE on multiple aspects at once without affecting all aspects.

EXAMPLE:
```
WHILE ([MIND.affected] = true)
    {
    IF ([MIND.comfort] = 0)
        {
        RELEASE
	}
    }
EXIT
```

The above code is a basic safety net that will run an infinite loop in the background that continuously checks if the Nous interpreter is comfortable, and if their comfort reaches 0, automatically undoes any and all effects. **Note that a failsafe like this is NOT infallible and should only ever be used in conjunction with basic consent practices rather than in place of them.**
