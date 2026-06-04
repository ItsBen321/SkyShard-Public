# What's in this folder

`Main.json` holds the latest patch and a `DataFiles` map for the exported game-info files.

`catalog_data.JSON` describes the export schema, file names, and current item counts.

## Data files

- `unit_data.JSON`: all unit resources.
- `enchantment_data.JSON`: all enchantment resources.
- `encounter_data.JSON`: all encounter resources.
- `hero_data.JSON`: all hero resources.
- `quest_data.JSON`: hero quest data referenced by heroes.
- `game_mode_data.JSON`: ranked, unrated, solo, challenge, and tutorial mode resources.
- `tip_data.JSON`: library/gameplay tips.

## Resource file structure

Most data files use the same structure:

- One big array containing every resource in that category.
- Every resource contains an array of its properties.
- Every property is a dictionary with:
  - `var`: the variable name, for example `Name`.
  - `value`: the exported value.
  - `var_type`: the Godot/GDScript type name.
  - `hint`: enum/range/resource hint metadata when Godot exposes it.
