Usage: USER ([GROUP.aspect | /quality])

The USER function is a special function that returns an aspect/quality based on the user who executed the code on the Nous interpreter. Note that the Nous interpreter's perception of the user is inherently limited, so this function should only be used for aspects/qualities that the user knows the Nous interpreter is aware of or could gauge accurately enough. What aspects/qualities meet that criteria will vary between different Nous interpreters.

EXAMPLE:
```
PERCEIVE ([SPIRIT.gender] = USER ([SPIRIT.gender]))
EXIT
```

The above code will change the gender of the Nous operater to match the user's gender.