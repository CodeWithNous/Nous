<sub>Authored by the Nous team</sub>

Usage: `IMPORT <[Array[String]]> FROM [String]`

The IMPORT command can be used to import variables or functions from Nous scripts with valid `EXPORT`s. If no array of imports is given, it will try to import the script's default export.

Example:
```
IMPORT FROM "Programs/bimbofy.nu"
BIMBOFY
EXIT
```

The above code will import an exported function from the file "Programs/bimbofy.nu", run an imported function, and exit.