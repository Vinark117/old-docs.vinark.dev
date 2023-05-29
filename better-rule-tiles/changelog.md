# <!-- {docsify-ignore} -->
# Changelog

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

- Rename tile variations to make things clearer for the user
- Prompts to help users navigate the tool
- More samples with tilemaps and scenes
- Replace tool to replace all output sprites of a tile
- Replace hide sprites option with tile highlighting instead
- Add an option to treat parent tiles as a separate tile, but still transfer their rules over