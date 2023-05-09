<sub>Authored by the Nous team</sub>

Usage: `CHAIN (path/filename.nu)`

The CHAIN function is a combination of the RUN and EXIT functions. It executes the designated script, and then immediately ceases the execution of the current script.

Example:
```
IF ([SPIRIT.favourite_colour] = "red") {
    CHAIN (./redscript.nu)
}

IF ([SPIRIT.favourite_colour] = "blue") {
    CHAIN (./bluescript.nu)
}

SPEAK ("Neither of those are my favourite colour.")
EXIT
```

The above code checks for the Nous interpreter's favourite colour. If it is red, it chains the script "redscript.nu"; the same applies for blue and "bluescript.nu". 

If the Nous interpreter's favourite colour is not one of those two, they will say so and then the script will cease.