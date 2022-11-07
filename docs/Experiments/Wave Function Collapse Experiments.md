Inspired by [mxgmn](https://github.com/mxgmn/WaveFunctionCollapse) & [Oskar Stålberg](https://twitter.com/OskSta), I spent a bunch of time building out a Unity implementation for WFC using tilemaps.  This was a fun exercising in optimization, and taught me a lot about how procedural generation can still leave room for authored editing: to me, the strength of WFC is allowing both the designer and the algorithm to "collapse" any of the nodes, opening up myriad ways to collaborate with the machine.

Source for WFC is closed.  The code is not documented well enough to be of any use to anyone, but interested parties can reach out if they want to learn more.  As usual, it's worth noting that performance in these clips is often bound by screen capture / streaming, and staggered execution is an intentional choice to make the videos more interesting! 

[Staggered Fill on YouTube](https://www.youtube.com/watch?v=AfUS6-QcaNw) - In this clip, each contiguous island can be clicked on to destroy the island, and then refill via WFC.  each new island is covered based on it's center point's distance to the middle of the square.

|                          |                                                                                                                                                        |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![[wfc_simplegen_small.gif]] | I started off with a simple generator using a basic pipe tileset                                                                                       |
| ![[wfc_shape_thumb.png]] | But ended up making a more complex pipes set with overpasses, endings and other features.  I fell in love with the pictures I could find in the chaos. |
| ![[wfc_kpd_thumb.png]]   | [fullsized asset here](wfc_KPD_full.png).  I began constraining the generation within shapes by selectively allowing regions                             |

Which lead to interactions like the following clips, where the user could select a region manually to trigger rebuilds of the WFC. 

[radial_sample.mp4](assets/radial_sample.mp4)

[gameplay_destruction.mp4](assets/gameplay_destruction.mp4)

