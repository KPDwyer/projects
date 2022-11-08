Inspired by [mxgmn](https://github.com/mxgmn/MarkovJunior), I implemented a simple set of rules of Markov Jr in Godot.  Markov Jr needs some boilerplate work to make nodes operate in any nonlinear way (hiearchies, subgraphs, etc). I opted out of doing this work unless I could complete the work to make `inference` work, which allows user to enforce constraints on a sequence to varying effects.  I never go that far, but my implementation was enough to generate mazes and flood fills.

It is my hope to revisit Markov Jr as part of the Godot port of my [[Node Mapping]] project.

| ![[mkjr_floodrules.png]] | A flood fill is a very simple markovjr ruleset w/ 2 rules.  see the [video here](assets/mkjr_flood.mp4).                              |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| ![[mkjr_mazerules.png]]  | With only 3 rules and no code changes, you can implement the entirety of a backtrack maze algorithm.  [video here](assets/mkjr_maze.mp4). |

