#  <!-- {docsify-ignore} -->

# Better rule tiles for Unity

This package was made to make the hassle of creating rule tiles for your Unity game better, easier and more intuitive than the regular rule tiles, while also adding more features which would not be availible unless you code it yourself.

It's main features include:
- Draw in all the tile placement possibilities into a single grid, no need to set rules by hand.
- Edit multiple tiles on one grid, and save them into a single asset for better file organization.
- Includes more rules than the default rule tile, which enables different tiles to interact with eachother on the tilemap.
- Automatically orders the rules for you, so one rule will not override the rest accidentally.
- Adding extended neighbors to a tile takes significally less time.
- Easily create sloped and other variations of a tile.
- Quickly create new tiles if you've already set one up prior.
- Supports square, isometric and hexagonal grids as well.

Try out the demo or buy the packgage on [itch.io](https://vinarkgames.itch.io/better-rule-tiles-for-unity).
<!--or the [Unity Asset Store]()-->

Get Started with the tool on the [get started](./better-rule-tiles/get-started)<!--(https://docs.vinark.dev/#/./better-rule-tiles/get-started)--> page.

# Development


Found a bug? You can report it [here](https://itch.io/t/2381185/bug-reports).<br>
Do you have an idea you feel like should be added to the tool? You can post it [here](https://itch.io/t/2381181/feature-request).<br>
Get involved in the development of this and other projects on my [discord server](https://discord.gg/DKpbVKk).<br>
Find tutorials about the package, and other useful and interesting content on my [youtube channel](https://www.youtube.com/channel/UCo-V8qAlHZWFRkUDCtc0cyQ).<br>

# Frequently asked questions

**Q: My sprites get displayed as missing textures.**<br>
A: Select your image file, and in the inspector under advanced settings enable `Read/Write`, after that close the editor and reopen it again to see the changes get applied. [Read more.](./better-rule-tiles/tile-creation?id=adding-sprites-to-the-grid)

**Q: My sprites are stretched on the grid.**<br>
A: Select your image file, and in the inspector change the `mesh type` from tight to `full rect`, this will make sure blank spaces are not left out from the image. After that close the editor and reopen it again to see the changes get applied.

**Q: My tiles are blank when I place them into the tile palette.**<br>
A: You have to set the `default sprite` option in the tile. If no rules match (which are pretty likely in the tile palette) than the default sprite is shown, if that's empty it shows nothing. [Read more.](./better-rule-tiles/tile-creation?id=rule-tile-options)