# <!-- {docsify-ignore} -->

# Introducing the tool <!-- {docsify-ignore} -->

[![The Solution to ALL of Your Rule Tile Problems!](./images/youtube-thumbnail.png)](https://www.youtube.com/channel/UCo-V8qAlHZWFRkUDCtc0cyQ)

## Chapter 01: "Intro"

We've all been there. Spending numerous hours clicking tiny boxes so we can save some time later down on the line. If you've ever used rule tiles in Unity you know how time consuming and tedious can it be just to convert a single tileset into a rule tile. And sometimes it doesn't even have all the features you'd need for your game, so you just end up spending even more time working around those problems. Well... don't you worry, because I have the perfect solution for it!

## Chapter 02: "The tool"

I call it **"Better rule tiles"**, it's a package that adds a tilemap style editor that lets you create rule tiles in it. Using this tool you can create rule tiles significantly faster than doing it the regular way, and there are also a number of features which are not present in the default editor. For example this tool lets you create interactions between tiles, and adds more default rules to choose from.

## Chapter 03: "Installing the package"

But let's start by installing the package to your project. To get the package head to the project's itch page where you can download the package. There are two versions, the full version is paid, but there's a demo so you can try out the package and decide whether it's worth it for you or not.

After you've dowloaded the package, you need to add it to your project. It comes in a zip file so first you need to unpack it, after that you can place the unpacked folder in either the **"assets"**, or the **"packages"** folder of your project. To get to these folders right click in your project window and click on **"Show in explorer"**, I recommend adding it to the packages so it doesn't take up space next to your assets. To add the package just copy the unpacked "BetterRuleTiles" folder to your desired location, and you're good to go.

## Chapter 04: "Creating the asset"

To open the editor you first have to create a **"Better rule tile container"** asset. You can find this in the create asset menu by navigating to **"Create/2D/Tiles/"**. This asset is the heart of the editor, this stores all the data of the editor, and after you're done and generated the tiles, they'll also be stored in this asset. You can open the editor by double clicking on this asset, or by clicking the open button in the editor. You can create as many containers as you want and they'll each have their own editor, so you can edit multiple tilemaps simultaniously.

## Chapter 05: "Adding the sprites"

To get started with creating rule tiles in the editor you first need to import the sprites. To import sprites you just simply drag and drop them into the editor. If you have a sliced tilemap, it will import all sprites. You can also add the sprites one by one if you need to.

If the images appear as missing textures in the editor, you have to check the **read and write enable option** in the images' import settings, after that you have to close the editor and reopen it again and your textures will appear.

## Chapter 06: "Creating tiles"

There's only one more thing you need before making the rule tiles, you need to create one first. In the bottom left corner of your screen you can see a tile drawer, in there, click the **add tile** button to create a new tile. This is basically the same thing as creating a rule tile in the inspector. You can add as many tiles as you want, and can edit these tiles all on the same grid, but let's just focus on one tile right now.

When selecting this tile you'll see an inspector window appearing in the bottom right corner. Here you can change the name of the tile, the preview image, the color and the shape of the preview image, the default tile options you'd see when editing a regular rule tile, and some other settings specific to this tool which we'll come back to later.

Let's rename our tile and change the default settings of it. I'll rename the tile to "Obstacle", change the color to a grayish color that better represents the tiles, and I'll set the default sprite to the sprite which has no neighbors. Click on apply changes to apply the changes you've made to the tile.

Everything is set up for this tile, so we can start making the rules now.

## Chapter 07: "Making the rules"

Select the brush tool from the top-left corner of the screen, with this you can start creating a rule. The process is similar to how the default rule tile works, you draw the tiles where the tile, and it's neighboring tiles supposed to be, and place the **"Not same"** tile where an X would be. You can than use the picker tool to pick your desired sprite and place it in it's place with the brush tool. The sprites and the tiles are on two separate layers, if a sprite is on top of a tile, that tile will use that sprite and it's surrounding tiles to create a rule. You can check if there's a tile under your sprite by toggling the eye icon in the top-right corner.

If we go to the export options and click on the export button right now, you'll see that only this sprite is present in the tile, and it's rules match the neighbors in the editor. You can also see that the settings we applied to the tile itself got applied to the exported tile, like the name and the default sprite.

## Chapter 08: "Making more rules"

But this tool is not to just do the same thing as in the default inspector, here you can draw real scenarios to the grid and specify the rules of that, so it's way easier te create and manage all of the different rules. So let's just do that.

I'm gonna start by creating a 1 by 1, 2 by 2 and a 3 by 3 square. than export the rule tile so we can check out the changes. As you can see all the 10 different tiles got added to the rule tile with their respective rules. 

We can also check this tile in the scene too. So let's create a tile palette and add the tile onto it. Now if we draw with this tile you can see that if we create a block it will have the correct rules. Of course if we create other shapes whis won't really work so we need to add some more rules.

This is also a good time to mention that even thougt you can place every tile right next to each other, sometimes you have to separate them so it covers more scenarios. In this example you can see that even though we already specified the edge pieces that should go there, it still uses the default sprite. This is because we only specified a scenario where all 3 tiles around it are empty, which in this case is not true, so we have to create a scenario which would be used for every edge piece. We can take the 3 by 3 square to separate it to edges and corners. I used the select tool along with the copy and paste functions to create a duplicate of the 3 by 3 square. After that I used the eraser tool to remove the sprites and the brush tool along with the delete tile to delete the tiles. You can also delete the 2 by 2 square because these tiles are already in the 3 by 3 configuration. Now if you check the tiles, the edge pieces are properly displayed.

## Chapter 09: "Making a complete tileset"

Using these techniques you can create a complete tileset. There's a sample rule tile included with the full package, so if you're having trouble figuring out the rules, or just want to save some time you can use this template to create your rule tile. Copy-pasting does not work across different editors unfortunately, but it should be fairly easy to copy the layout from one editor to another. Or if you want to create a new tile based on this you can just duplicate the asset and edit it directly, I'll do the latter because it'll save some time.

And with that We have a fully working rule tile with every possible scenario, done under 10 minutes.

## Chapter 10: "Variations"

So far we only covered how we can speed up the creation of rule tiles, but this tool is capable of doing way more than just that.

Let's say you want to add slopes to your tileset, but because slopes are basically just corner pieces in disguise you can't just add them to the same rule tile, so you create a different rule tile, but this rule tile doesn't connect to the non sloped variants, so it's completely useless... Well, there's a solution for that.

I've set up the a feeeew rules for slopes. I know this looks a bit intimidating but the layout doesn't matter right now, you can have as many or as little slopes as you want, and the process will be the same. So... I've created four new tiles, one for each corner, and set up the rules that are only specific to the slopes. If we try this out right now you'll see that it doesn't really work as you'd want it to. 

If you just draw with it regularly only the slope parts will show up, all the other tiles will display the default tile. This is quite obvious why it doesn't work, there are no rules set up for any of these scenarios, but you surely don't want to recreate the base tilemap four more times just so you can have slopes. Well, you don't have to. If you select the tile and look into the tile inspector window, you'll see an option called "Unique tile", this is set to true by default, but if you change it to false a dropdown will appear where you can select another tile. If this toggle is set to false this selected tile will be used to fill any missing rules in the tile. So if we select the "obstacle", it will add the missing rules from the obstacle tile to this tile.

Let's change all the slopes to use the "obstacle" tile as a base, than generate the tiles.

Now if you draw with these slopes again, you'll see that the sprites that were previously defaulted, now will display the proper sprite, based on the "obstacle" rule tile. 

You can use the tile now as it is, but most likely you want to use it together with the other variants. Luckily there's an option for that too. For this you have to look at the **"Add variations"** option in the tile inspector. The tile you're editing will connect to any other tile you add here, you just simply select the tile from the dropdown and click the add button to add it. I want all 5 tiles to connect to each other, so I'll add all of them on all of the tiles.

If you generate these tiles one more time, and try them out, you'll see that now they're all connecting to each other, so you can add those slopes anywhere you want.

## Chapter 11: "Extended rules"

There's one more feature I want to show before moving to another tileset. You were probably wondering for some time now if you could add randomized or animated tiles, or even extend the range where the tile checks for neighbors. Well... These are all possible with this tool. If you go to the top-left corner of your screen, you can see an icon with a mouse and a cog. That's the grid cell inspector tool. After selecting the tool and clicking a tile on the grid, the inspector window will show the properties of that specific grid cell. Here you can change the settings of the tiling rule the same way you could in a regular rule tile, with the only difference that this grid only specifies where to check, and not what to check for, so it's way faster to add a larger number of places.

If you have some tiles on the grid with modified properties, there's an option in the top-right corner to highlight them, so you can find them easier.

## Chapter 12: "Other tile shapes"

I've showed everything I can with these tilemaps, but what if you want to work with isometric or hexagonal tiles? Well, the tool supports all grid types you'd want to work with. At the export options in the top-right corner there's the grid type option which is set to square by default. Changing this will change the grid shape. It's better to do this before starting to work on your tilemaps, because the hexagonal tilemaps for example use a different coordinate system, so changing between these two grid types can mess with the placement of the tiles.

You can also change the size of the grids in the dropdown next to the export options, or add an offset if your tiles are not aligned properly, along with a few other editor settings.

## Chapter 13: "The end"

I have lots of tips and trick that I could show you regarding this tool, but it would be quite a long video, so I'll wrap it up here. If you need more detailed description of this tool, there's a documentation I've written where you can find descriptions of every setting and option there is in the tool. You can also join my discord server if you need any help. Both links are in the description of this video, along with the page for the tool itself. I hope you liked this tutorial, and especially the tool I created. 

That's it for this video. Bye.