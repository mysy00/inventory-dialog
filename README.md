# Inventory Dialog with item stacking

![sampctl](https://shields.southcla.ws/badge/sampctl-inventory--dialog-2f2f2f.svg?style=for-the-badge)

A fork of an extension for ScavengeSurvive/inventory that uses SA:MP dialog menus for
player interaction with their inventory items.
If you want more control, it's recommended to use the upstream project.
I keep this fork for my server where inventory items of the same type don't have any differences.

Key changes:
- Items of the same type are stacking.
- When you select an item, the options are: Use, Information, Drop.

## Installation

Simply install to your project:

```bash
sampctl package install ScavengeSurvive/inventory-dialog
```

Include in your code and begin using the library:

```pawn
#include <inventory-dialog>
```

## Usage

Documentation is in the source code.

## Testing

To run tests:

```bash
sampctl package run
```

And connect to `localhost:7777` and try it out. H opens the inventory, Y adds an
item, F picks up. `/lockinv` prevents the inventory from being opened by
returning 1 on `OnPlayerOpenInventory`.
