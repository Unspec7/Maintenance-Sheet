# Maintenance-Sheet-README

## Getting Started / Intro

First: File > Make a Copy

**BRIGHT YELLOW** means safe to user edit, and actually need to be user edited. This is where the vast majority of your data goes.

The orange "Production Date" cell autopopulates, but is safe to manually update if you know your vehicle's actual production date. If you don't know, leave it alone.

## Summary

**Summary** table mirrors its information from **Intervals**, and is currently set up to handle ~125 individual maintenance options. If you wish to add more, you must add more rows in BOTH tables. If you wish to remove certain maintenance elements, do NOT touch Summary. Instead, delete the entry in ***Intervals*** and it'll auto-remove from the Summary table

**Schedule** table is a visual representation of what items are where relative to where your mileage is. Big yellow bar is your current mileage rounded UP to the nearest 5000 miles. Green blocks are when items are due based on mileage - if they're time based only items, then you'll just need to use your eyeballs (helpful to filter Status by "Due Now").

Overall, the only field in Summary that you should be regularly touching is *Current Mileage*

### What if an item has not been maintained yet?

If an item in the maintenance tracker has no log entry, then the sheet makes the assumption that the item is original from the factory. This means that it'll assume the mileage is 0, and date is the production date/model year. Basically, don't worry about it, everything will be fine.

## Log

This is where almost all of your effort will be. All maintenance logs go here, and are used for the maintenance tracker. *Date, Mileage, Type,* and *Service* are mandatory, and is how the sheet finds the correct entries to use for tracking.

## Intervals

This is where you enter the intervals for all the maintenance items you wish to track, and where you add items if not already present. Feel free to add more Types, but the conditional formatting for the pretty colors will be up to you to set up for the new type. 

- All time based intervals are based on years. If you need months, you'll need to do decimals (e.g. 6mo = 0.5y). I have not tested super low month count options, bugs might occur. 
- If time or mileage is not applicable for one of that item's intervals, "***N/A***" must be used for the interval that is not applicable. If you use blank instead of "N/A", it will break the tracking for that type of interval. Sorry.
- If you wish to add an item, it is easiest to just copy paste an entire existing row into a blank one, and then just update the Type, Service, and Intervals manually. Make sure to include the table with all the X's in the copy paste as well!
- If you wish to remove an item, clear the entire row. Deleting the row works but removes an entire row from the sheet as a whole, and is overkill. Just clearing that row is enough.

The table to the right of the numbers autopopulated, don't worry about editing it.

## Helpers

Helpers tab is where the dropdown menu's in **Log** gets their information, do not touch if you don't know what you're doing

## VIN Decoding

VIN decoding tab only works for BMW's. The sheet will work fine for all other brands, but the VIN decoding tab will be non-functional/broken.

### There's a bug!

Feel free to report here. I may or may not fix it. We'll see.

## Credit 

[u/flanmorrison](https://www.reddit.com/user/flanmorrison/) for the original sheet, reddit post [HERE](https://www.reddit.com/r/BMW/comments/1080p9q/i_made_a_bmw_maintenance_tracker_on_google_sheets/).
