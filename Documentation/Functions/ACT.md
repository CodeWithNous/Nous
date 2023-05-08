<sub>Authored by the Nous team</sub>

Usage: `ACT (<string>)`

The ACT function, when executed, prompts the Nous interpreter to perform the described action. As the string used is a written description, it is important to use language that is clear and simple as well as tailored to the intended Nous interpreter to be as easily understood as possible.

Example:
```
WHILE ([SPIRIT.loyalty] < 100)
    {
    PERCEIVE ([SPIRIT.loyalty] ++)
    }
ACT ("Salute the user")
EXIT
```

The above code will increase the Nous interpreter's loyalty, and when it's reached its maximum value, cause them to salute.
