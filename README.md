# Maintenance-Sheet-README

**BRIGHT YELLOW** means safe to user edit, and actually need to be user edited. This is where the vast majority of your data goes.

The orange "Production Date" cell autopopulates, but is safe to manually update if you know your vehicle's actual production date. If you don't know, leave it alone.

## Summary

**Summary** table mirrors its information from **Intervals**, and is currently set up to handle ~125 individual maintenance options. If you wish to add more, you must add more rows in BOTH tables. If you wish to remove certain maintenance elements, do NOT touch Summary. Instead, delete the entry in ***Intervals*** and it'll auto-remove from the Summary table

Overall, the only field in Summary that you should be regularly touching is *Current Mileage*

### What if an item has not been maintained yet?

If an item in the maintenance tracker has no log entry, then the sheet makes the assumption that the item is original from the factory. This means that it'll assume the mileage is 0, and date is the production date/model year. Basically, don't worry about it, everything will be fine.

## Log

This is where almost all of your effort will be. All maintenance logs go here, and are used for the maintenance tracker. *Date, Mileage, Type,* and *Service* are mandatory, and is how the sheet finds the correct entries to use for tracking.

## Helpers

Helpers tab is where the dropdown menu's in **Log** gets their information, do not touch if you don't know what you're doing

## VIN Decoding

VIN decoding tab only works for BMW's. The sheet will work fine for all other brands, but the VIN decoding tab will be non-functional/broken.

### There's a bug!

Feel free to report here. I may or may not fix it. We'll see.
