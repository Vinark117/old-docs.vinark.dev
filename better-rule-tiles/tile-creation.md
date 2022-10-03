# <!-- {docsify-ignore} -->

# Creating a tile

To create a tile just head over to the [tile drawer](./better-rule-tiles/get-started?id=the-tile-drawer), and click the **Add Tile** button to create a tile. You can add any number of tiles, there's no limit on how much you can have.<br>
These tiles are basically the equivalent to creating a rule tile asset in the project window. When generating the tiles in the [export options](./better-rule-tiles/get-started?id=the-editor-settings) all of these tiles in the drawer will be converted to rule tiles that you can use in the game, with it's rules automatically set based on what you placed in the **editor grid**.

![Convert Tiles](./images/tiles-convert.png)

# The tile inspector

When selecting one of the tiles that you created in the drawer, an **inspector window** will appear in the bottom right corner of the editor, here you can change certain properties of the tile. Some settings are the same as in a regular rule tile, like the default sprite, collider or gameobject, but some options are more specific to these better rule tiles, and enable you to do things that the default rule tiles cannot.

## Editor options

## Auto texture

## Rule tile options

## Unique tiles and tile variations

## Custom properties

# Setting tile rules

Setting rules is similar to setting them in the default rule tile, but instead of individually clicking each grid cell to cycle between the options, here you can just select the option than draw it on the grid. This way you can create rules way more faster than regular rule tiles. To place the rule ***"this"*** (which in a regular rule tile is the green arrow), you just need to draw the same tile next to one that has a sprite assigned, and if you want the rule ***"not this"*** (the red cross on the regular rule tile), you just draw with the tile **not same**. And to ignore the tile you just don't place anything there.

![Grid To Rules](./images/grid-to-rules.png)

To find out more about the possibilities and get a more detailed explanation on how rules work you can go [here](./better-rule-tiles/rules).