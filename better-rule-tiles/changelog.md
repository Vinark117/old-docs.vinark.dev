# <!-- {docsify-ignore} -->
# Changelog

## Version 1.4 (To be released)

- Added a new "Universal sprite settings" window
- Separated the "sprite drawer" toolbar button and added a new button to open the "Universal sprite settings"
- Added an "Enable universal sprite settings" option to the export menu, this option is enabled by default on newly created assets, and disabled on already created assets
- Improved UI for better readability and separation between sections of the window.
- Renamed "tile variations" and "variation of" options to make them less confusing.
- Added a confirmation window when deleting a tile.
- Fixed error which caused the game to not build

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

# Planned features

- Prompts to help users navigate the tool
- More samples with tilemaps and scenes
- Replace tool to replace all output sprites of a tile
- Replace hide sprites option with tile highlighting instead
- Add an option to treat parent tiles as a separate tile, but still transfer their rules over
- Add a button to the tile settings to export that tile as either a custom tile or a default rule tile
- Add a confirmation screen for deleting a tile
- Universal sprite settings, for setting random or animated sprites that apply to all rules which use the specific sprite
- Option to set the animation start frame to a random frame, so the animation wouldn't be in sync with every tile. This would be determined based on a seed.
- Gridcell configuration picker tool
- An option to bump up the priority of the rule
- A tool that creates "preset blocks". You'd create these preset blocks by selecting an area and clicking on a create block button. In a preset block, every tile checks for every other tile in the block. It'd besically act like if you'd select every tile in the selected area and set the selected area as the area to check the neighbors.
- Ability to add tags to tiles and add variations based on those tags