<sub>Authored by the Nous team</sub>

Usage: `LINK [GROUP.aspect] AND [GROUP.aspect] | AND [GROUP.aspect]...`

The LINK function can be used to create a connection between the first mentioned aspect and the other(s), causing all changes made to one to apply to the other(s). Aspects of differing data types can be connected with LINK, but any changes made to a connected aspect will not be reflected in connected aspects whose data type would make the change invalid (eg. setting a real number and boolean to 0 are both valid, but setting a real number equal to a string is not.)

Example:
```
LINK [BODY.breast_size] AND [MIND.libido]
PERCEIVE ([BODY.breast_size] ++)
UNLINK [BODY.breast_size] AND [MIND.libido]
EXIT
```

The above code will cause the Nous interpreter to perceive an increase in breast size and a proportionally equal increase to libido.
