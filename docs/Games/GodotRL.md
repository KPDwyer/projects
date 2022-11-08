GodotRL (not the final name) is a Roguelike I'm slowly chipping away at as I learn Godot.  I challenge myself to write large systems and keep them working together harmoniously, as well as make the design accessible.  Some [tweets are available here](https://twitter.com/_KPDwyer/status/1438324255092056064) for now.  

## Completed Features
- A threaded implementation of [Dijkstra Maps](http://www.roguebasin.com/index.php/Dijkstra_Maps_Visualized), which may need to be ported to GDScript 2.0 or C# in the future.
- Radial FoV by way of [Bresenham's algorithm](https://en.wikipedia.org/wiki/Bresenham%27s_line_algorithm), performed in octants
- A Command Queue action system with full interrupt, divert and undo support.
- Deterministic map generation with serializable settings, for consistent reproduction of a level across plays (handy for repro cases)
- Several move abilities, including `in range`, `explicit points` and `explicit paths`
- A thoughtful energy system where abilities energy costs determine how long until the next turn.
- A Turn order bar that accurately shows the turn order and a preview of how each abilities energy cost affects turn order.
- Entities mix and match 2 aspects from a pool to determine appearance and abilities
- Auto Explore mode, where the player auto explores teh map until it is fully explored or something interesting happens

## Upcoming
- A token system to act as a foundational mechanic for combat
- Undo support for the logger
- Peek view for inspecting anything you'd wish
- ...and more!

[here's a recent clip](assets/turn_order.mp4)
