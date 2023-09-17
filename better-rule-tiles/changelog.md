# <!-- {docsify-ignore} -->
# Changelog

## Version 1.4.1

- Fixed sprite output transform when using universal sprite settings
- Readded sprite output transform option when using preset blocks
- Moving and pasting over something will now override what's already there

## Version 1.4.0

- Added a new "Universal sprite settings" window, here you can change the output parameters of a sprite, so if you place that sprite down multiple times it'll always have the same output.
- Separated the "sprite drawer" toolbar button and added a new button to open the "Universal sprite settings"
- Added an "Enable universal sprite settings" option to the export menu, this option is enabled by default on newly created assets, and disabled on already existing assets
- Improved UI for better readability and separation between sections of the window.
- Renamed "tile variations" and "variation of" options to make them less confusing.
- Added a confirmation window when deleting a tile.
- Fixed error which caused the game to not build
- Textures will be marked readable automatically if they're not already, it's not required to set it manually anymore
- Added a new "preset block" feature. Draw part of a scene in the editor and mark it as a preset block to make sure it'll look as you wanted it to. To remove the preset block, use the tile inspector tool on a tile inside the preset block.
- Added more tooltips
- Added samples each with their own tilemaps and scenes for the following features:
    - simplify rules feature
    - creating rules
    - preset blocks
    - connections between tiles
    - universal sprite settings and sprite options
    - variations
    - custom properties
- Toolbar now better adapts to the width of the editor window

## Version 1.3.3

- Fixed bug: Tiles randomly disappear from the grid and the tile drawer.
- Fixed bug: Editor crashes when entering or exiting play mode.
- Added a "Close window" button to the container asset, in case you can't close the window in any other way.

## Version 1.3.1 & Version 1.3.2

- Changed the way the editor handles arrays.

## Version 1.3.0

- Added a new sprite output type: Pattern.
- Other backend changes.

## Version 1.2.0

- Tested and verified compatibility with Unity 2019.
- Changed how locked cells are displayed.
- Added options to customize how locked cells are displayed.
- Added a sprite drawer.
- Added options to customize the new sprite drawer.
- Import all sprites with a single button press.
- Fixed a build error related to the Functions class.

## Version 1.1.0

- Changed toolbar button placement code to be more dynamic.
- Added the ability to lock and unlock a selection, so it can't be edited accidentally.
- Added a warning message if the default sprite was not assigned.

## Version 1.0.1

- Added support for differently sliced isometric tiles, previously it only supported square sliced sprites.
- Updated package dependencies to reflect the minimum supported versions of packages and unity version.
- The tool now supports Unity 2020.

## Version 1.0.0

Initial release


<!-- {docsify-ignore} 

# Possible upcoming features
- Replace hide sprites option with tile highlighting instead
- Add an option to treat parent tiles as a separate tile, but still transfer their rules over
- Add a button to the tile settings to export that tile as either a custom tile or a default rule tile
- Add a confirmation screen for deleting a tile
- Option to set the animation start frame to a random frame, so the animation wouldn't be in sync with every tile. This would be determined based on a seed.
- Gridcell configuration picker tool
- An option to bump up the priority of the rule
- Ability to add tags to tiles and add variations based on those tags

-->