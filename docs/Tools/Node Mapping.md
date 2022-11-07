I built a node-based mapping library for Unity, using the xNode plugin for the graph tooling.  I build a lot of grid-based games and was hoping to create a Shader-Graph-like solution for generating tile maps.  This tool is open sourced  [here](https://github.com/KPDwyer/rlbits-mapping).   I kept a [fairly active Twitter thread](https://twitter.com/_KPDwyer/status/1204466766530957314) while working on this project as well.

## Needs
When generating maps in a code-driven way, you often need to layer and combine noise patterns in a variety of ways, testing and tweaking as you go.  This iterative process can be slow when changing code every test - or time consuming and unwieldy to expose all of the appropriate elements to the inspector.  Compounding this is that rather than a singular result, you are often building something robust that can be generated in a multitude of ways, so each iteration needs to be tested with some set of changing parameters: often `seed`, but also `map_size` and other elements.

## Solution
The Node Graph workflow lends itself well to these needs: you can preview your map generator at multiple steps in the generation, as well as across multiple seeds.  Live Preview can be made to react to scrubbing of value, and pieces of the genreator can be detached from others to isolate elements that need fixing.

## Present & Future
The tool is open sourced [here](https://github.com/KPDwyer/rlbits-mapping).  I intend to rebuild it in Godot 4, as a `GraphEdit` and `Noise` refactor are slated to be delivered.

|                                                         |                                                                                                                                                                                     |
| ------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![[nodemap_noisecell.gif]]                              | Another strngeth of this tool is combining procedural methods from different domains: like experiementing with cellular automation applied to the ouput of traditional perlin noise |
| ![[nodemap_shapetweaks.gif]]                            | This clip shows what it looks liek to tweak how a Minimum Spanning Tree is connected, but also how the tool stores and renders that data.                                           |
| ![[nodemap_scrubmaze.gif]]                              | Quick gif that shows how scrubbing the `seed` param allows you to view many outputs of a graph                                                                                      |
| ![[cap_nodes.png]] ![[cap_scene.jpg]] ![[cap_play.jpg]] | I wrote a couple of different consumers for the output, including a 3d terrain plugin.                                                                                                                                                                                    |
