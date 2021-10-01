# Overview

This is a compatibility patch between two other mods: [Animated Holosphere Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2592592503) and [Animated Silicoid Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2579736379).  Unless you are using both of those mods together, you do not need this mod.

If you are using [Silfae's Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2596417938) (the mod, not collection), you do **not** need this patch.

# Changes

Combines to Pop strata files from Holosphere and Silicoids Revisited in order for both mods to have their custom Pop upkeep applied correctly.

## Compatibility

This mod overwrites all of the default `pop_category` (Pop strata) files.  It is not compatible with other mods that want to alter Pop strata (other than the two mods it is explicitly intended to patch).  It's likely to break any time Stellaris makes changes to the underlying Pop strata.  These files are completely overwritten:

* `common/pop_categories/00_social_classes.txt`
* `common/pop_categories/01_gestalt_drones.txt`
* `common/pop_categories/02_other_categories.txt`

Built for Stellaris version 3.1.2 "Lem."  Not compatible with achievements.

### Dependencies

In order for this mod to function, you **must** install these mods and load them before this one:

* [Holosphere Rising](https://steamcommunity.com/sharedfiles/filedetails/?id=868965217) by Silfae
* [Animated Silicoid Portraits](https://steamcommunity.com/sharedfiles/filedetails/?id=1160316076) by Silfae
* [Silfae's city sets updated](https://steamcommunity.com/sharedfiles/filedetails/?id=2247427791) by Nozeminer
* [Animated Holosphere Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2592592503) by me
* [Animated Silicoid Portraits: Revisited](https://steamcommunity.com/sharedfiles/filedetails/?id=2579736379) by me
* [Full Military Service for Battle Thralls](https://steamcommunity.com/sharedfiles/filedetails/?id=2496357447) by me

### When to Install

This mod should be added before the game has started.  If you remove it from a game in progress, Pops may have incorrect or missing upkeep costs.

## Changelog

* 1.0.0 Initial version
* 2.0.0 Update for Stellaris version 3.1 "Lem"
* 2.0.1 Verify compatibility with Stellaris 3.1.2 - no code changes

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/revisited_holosphere_silicoid_compatibility)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property.  That will ensure the game can see the files, and also that CWTools will parse them.  Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.