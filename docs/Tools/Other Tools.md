I'm in the process of moving these articlesto this new format, but for now you can find some of my old tools elsewhere.  Keep in mind some of these tools are as old as 2017 and are here for historical reasons, not because the problem they solve is still a problem.

[Generating Animators](https://kpdwyer.github.io/2019-01-17-Pixel-Animator-Generator) - This is a small Unity tool to generate an Animator & Animations from a folder structure.  Its not a compelte solution, just automating some of the more annoying work. 

[Simple Whitelist RuleTile](https://kpdwyer.github.io/2021-01-03-Whitelist-Ruletile) - Extremely handy for projects using lots of RuleTiles with Unity's Tilemap system.  Often a ruletile should count another type as its own to correctly handle edges with different tiles.  this is a simple implementation to have a rule tile treat another ruletile as itself. 

[RPGMaker Autotile Asset Pipeline in Unity](https://kpdwyer.github.io/2019-04-10-Autotile-Pipeline) - Another handy tool for using tilemaps in Unity, this tool correctly imports RPGMaker's A2 tile assets into Unity's Ruletile system.  The mapping used here is twice the resolution of the actual tile, as RPGMaker actually tiles these at twice the resolution: The tiles that work for a 16x16 world are actually broken into 8x8 to manager all corner combos.  Also handy is that the mapping is defined by a scriptable object, so you can make an autoimporter for a different source layout. 

[Unity Depth Capture for Facebook](https://github.com/KPDwyer/DepthCapture) - Quick tools that captures a screenshot and the depth buffer from Unity, auto formatted to work as a Facebook 3D photo upload. 

[SpriteMaker](https://github.com/KPDwyer/SpriteMaker) - An older tool I built to handle generating smaller UI & Utility sprites directly from inside Unity.  

[PaletteSwapper](https://github.com/KPDwyer/PaletteSwapper) - Another older tool allowing you to manually swap asset palettes right in Unity.

