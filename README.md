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
Install Unity and import one of the following packages (Simple-Tiled or Overlapping) 

### Simple Tiled
Simple Tiled will produce an image based on the sample tile-set to the left. In order to 

### Overlapping
