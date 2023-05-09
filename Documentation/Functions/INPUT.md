<sub>Authored by the Nous team, idea courtesy of Twitter@JunieDreamcast</sub>

Usage: `INPUT`

The INPUT function is a special function that, when executed, will pause the current script until the user provides an input to the Nous interpreter. The execution of the script will then resume, with INPUT being treated as a variable containing the programmer's input (as an integer, string, boolean, or any other applicable data type). It is recommended to use this in conjunction with the SPEAK or ACT functions so that the user will know the Nous interpreter is waiting for a response.

Example:
```
SPEAK ("Please enter a new name.")
PERCEIVE ([SPIRIT.name] = INPUT)
EXIT
```

The above code will have the Nous interpreter prompt the user to provide a new name for the Nous interpreter, and then, after the input has been given, change the Nous interpreter's name to the given input.