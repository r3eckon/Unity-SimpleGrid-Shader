# Unity-SimpleGrid-Shader
Simple procedural grid shader with GUI customizable parameters

# Usage

Drag and drop both Shader and Material files in your project. The Material can then be edited and also dropped on a gameobject mesh inside Unity. 

To edit the grid material, the following GUI options are available.

![Available Material Parameters](https://i.imgur.com/rzwV2OR.png)

Line Color, Cell Color and Selected Color all represent their respective grid components. Colors use Alpha Cutoff for full transparency by setting the alpha channel to 0.

Grid Size is the amount of cells in the grid. You must make a simple edit to the shader itself to go above 100.

Line Size is the size of lines making up the grid. 

Select Cell enables or disables the cell "Selected" by the parameters Selected Cell X and Y. It only colors a certain cell using a different color, but the base code to "Select" cells in the grid can be used in more complex ways.

The parameters shown above create the following grid.

![Example Grid](https://i.imgur.com/Vaeo80i.png)

# More information

There is no aspect ratio based scaling by default, to keep cells squared keep the plane mesh square ( or implement your own aspect ratio scaling )

The selected cell can also be chosen by editing the material using the SetFloat value, to potentially make the material interactive. ( See official unity docs to learn more )

The shader, when applied to new materials, can be found under "PDTShaders/TestGrid".
