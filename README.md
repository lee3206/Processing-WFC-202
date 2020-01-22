# WFC-202

## Processing
Install [Processing](https://processing.org/) and make sure to install the Python package for processing.
Navigate to the Ultima Tiles sketch and open it through processing.

On Windows:
Where it says 
```bash
path = File("C:\Users\You\Navigate\To\Ultima_Tiles\Tiles").listFiles()
```
Enter the file path for your copy of Ultima_Tiles.

Look at the connectors array and note the numbers.
    2
 1 x x 3
   x x
    4
For each tile, the first number is 1, going clockwise around the tile. Each number is a valid connector. So tiles that have a 0 on the left and right sides are valid combinations.

Press play on the processing window to run. It will likely hang for a moment, then start drawing tile by tile. 

Note that there are a great many path tiles and they tend to be non-sensical. One way to improve this behavior would be to reduce the frequency of tiles or add some exclusion rules so that they cannot be right next to one another.
## Unity
All of this work was done using the [WFC for Unity by SelfSame](https://selfsame.itch.io/unitywfc)

Install Unity and import one of the following packages (Simple-Tiled or Overlapping)
All of the Ultima tiles and sprites are available in the Resources folder in Assets.
If you install both the Simple Tiled and Overlapping packages the assets for Simple Tiled are in the Simple Tiled folder and the Overlapping is in the main resources folder.

Map environment prefabs (grass, bridges, rivers, trees, mountains, etc.) are in the top level of the resources folder.
Prefabs of Buildings, dungeons, statues, signs, etc., are in the Decorations subfolder. 
The original PNG images are in the folders "z Original sprites" and "Scenery".

Note that only Prefabs can be added to the tile painter. If you wish to add new images to the scene drag them into the resources folder, then drag them into the scene to create a prefab, then drag the prefab back into resources and delete it from the scene. These may then be added to the tile painter pallete. Additionally, when importing Pixel style artwork into Unity you must select Filter Mode "Point (No Filter)" or they will be compressed and lose the pixel ratios and the ratio of any new image scale must be adjusted to fit inside the tile painter grid without overlap (e.g., a 16x16 pixel image must be adjusted to scale x and y 6.25)

### Simple Tiled
Simple Tiled will produce an image based on the sample tile-set to the left. In order to 

### Overlapping
