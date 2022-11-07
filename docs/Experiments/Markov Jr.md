Inspired by [mxgmn](https://github.com/mxgmn/MarkovJunior), I implemented a simple set of rules of Markov Jr in Godot.  Markov Jr needs some boilerplate work to make nodes operate in any nonlinear way (hiearchies, subgraphs, etc). I opted out of doing this work unless I could complete the work to make `inference` work, which allows user to enforce constraints on a sequence to varying effects.  I never go that far, but my implementation was enough to generate mazes and flood fills.

It is my hope to revisit Markov Jr as part of the Godot port of my [[Node Mapping]] project.

