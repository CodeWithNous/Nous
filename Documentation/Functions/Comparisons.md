<sub>Authored by the Nous team</sub>

Nous has a variety of functions that can be used to perform comparisons. These are useful for many things in practice, as neither the programmer nor Nous interpreter can account for variables consistently. Comparisons allow for code to check for the desired conditions to be met before executing code, or inversely execute code until a desired condition is met. Each comparison function is followed by an expression, and then by code; the conditions for running the code vary from comparison to comparison. Below is a complete list of comparison functions and how they are used.

---

`IF (<expression>) {<code>}`: The most basic comparison function. Runs the specified code only if the expression returns True.

`WHILE (<expression>) {<code>}`: A simple loop that will repeatedly run the code until the expression returns false. This is useful for ensuring that code needing specific conditions to be met in order to function will be able to run.

`ELSE {<code>}`: Must placed after a comparison function. Its code will run if the comparison before it returned False. Can also be followed by a comparison to perform an additional check before executing its code (ex. `ELSE IF (...)`)

---

In addition to the basic comparison functions, the logic functions AND, OR, and XOR can be added to check multiple expressions at a time. AND requires all expressions to return True, OR requires one or more expressions to return True, and XOR requires exactly one expression and no others to return True.

Example:
```
LINK [MIND.speed] AND [MIND.intelligence]
WHILE ([MIND.speed] > 0) AND ([MIND.intelligence] > 0)
    {
    PERCEIVE ([MIND.speed] --)
    }
UNLINK [MIND.speed] AND [MIND.intelligence]
EXIT
```

The above code will decrease the Nous interpreter's intelligence as well as the speed of their thoughts until either aspect reaches 0.
