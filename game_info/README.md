# What's in this folder

## main
This holds general info about the game. Currently:
- Patch: the latest patch (so you can fetch from the patch_notes folder)

## unit_data
All the current relevant unit data. File structure:
- One big array containing every unit
- Every unit contains an array of its properties (dictionaries)
- Every property holds this current information:
  - "var": the name of the variable (example: "Name")
  - "value": the value of the variable (example: "Cannon")
  - "var_type": the type of the variable (example: "String")
  - "hint": when it expects a special value (mainly for enums/categories)