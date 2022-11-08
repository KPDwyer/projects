beholdin' is a coffee break twin stick shooter; a daily challenge score chaser that rewards the risky and creative players.  You can [find it on itch](https://kpdwyer.itch.io/beholdin).  I finished the game around 2018 after about 1.5 years of commutes.  Call it 10 hours a week, about 70 weeks to be generous, that's 700 hours.  Its rough around the edges, but I **love** it and will probably dedicate some time to making it more robust in the future.  I kept a [devlog](https://kpdwyer.itch.io/beholdin/devlog) alongside releases that some parties might find interesting.  Oddly enough, the best visual story of the game's development is probably this [moment on Twitter](https://twitter.com/i/events/1037127521270157312) (for now).

## Features
- a single procedurally generated level every day.
- a unique level skin (biome?) for each day of the week.
- a unique combination of enemies & mechanics for each day of the week.
- in each room, every wave triggered increases your multiplier, each hit you take decreases it.
- player-paced risk vs reward: break each crystal one at a time to deal with each wave in isolation, or break 'em all at once and hope you can handle it for max score.  
- leaderboards, for bragging rights.
- Reflective walls, gravity wells, shields, lasers, bombs & turrets: all the classics make an appearance.

## Technical Notes
- Lasers are ray-marched so they could be reflected by reflectors, but also get their trajectory bent by gravity wells (push & pull)
- all of the gameplay art was made in-unity with custom tools to make meshes out of polygons.
- each vertex of the art meshes stores a UV lookup value into a gradient palette that you can swap as you please (try hitting space while you're playing the game!)
- the game was made almost entirely on my train commute to and from work.  GameSparks & Playfab integration required some evening work.
- each audio track was made in Gadget on my iPad.  elements of the songs are ducked in and out based on whether a room has unbroken crystals, active combat, if a room has a boss, and more.