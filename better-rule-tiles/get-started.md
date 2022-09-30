# <!-- {docsify-ignore} -->

# Getting started

To start using the tool first you need to create a "Better rule tile container" asset. This asset is the core of the tool. Everything you do will be saved into this container asset, therefore you must create one before you start doing anything else.<br>
To create an asset, right click in the project window, and navigate to: **Create -> 2D -> Tiles -> Better Rule Tile Container**, and click on it.

![Create asset image](./images/create-asset.png)

<br>

# Opening the editor

After you've created a "Better rule tile container" asset, you can open the editor by **double clicking the asset**, or by **pressing open in the inspector** when the asset is selected. 

![Open asset](./images/open-asset.png)

> *Note that you shouldn't edit this asset directly, but only through the editor to avoid errors. Only edit the asset directly for debugging purposes!*

If you have multiple container assets, each asset will open in it's own editor window. If the asset is already open in an editor, opening the asset will bring that editor window in front.<br>
Deleting a container asset will close the editor window editing that asset.

<br>

# The rule tile editor

![Default editor window](./images/editor-window-default.png)

When you open a new file you'll see this window. It has 4 main parts:
- The **grid**,
- The **toolbar** and **editor actions** in the top left corner,
- The **tile drawer** in the botton left corner, and
- The **editor settings** and **export options** in the top right corner.

## The grid

There are 3 different types of grids you can work in: **square**, **isometric** and **hexagonal**, with hexagonal having two different orientations: **pointed topped** and **flat topped**. You can change the grid type in the **export options** dropdown, in the top right corner. You can furthermore customize the grid's scaling in the **other settings** dropdown, which you can find right next to the export options.

![Grids](./images/grids.png)

> *Note, it's best to change the grid type before you start working on anything, to avoid displacement of the grid due to the different coordinate systems.*