# King Of The Grid

*A Z80 Sandbox Competition Game* in which developers can write
bots to compete on the most efficient algorithm to be King Of The Grid!

<div align="center">

https://github.com/user-attachments/assets/2881a106-d6ee-4869-8e0b-37a01a3257bd

  Example of a single competition.
</div>

# Game Rules

* See [rules.cpp](https://github.com/kingofthegrid/king-of-the-grid/blob/master/src/rules.cpp) for exact rules (how often, what values etc).
* World size: 32x32 cells
* Two bots (or programs) spawn in top-left and bottom-right corners
* Each bot has a set of energy. See [rules.cpp](https://github.com/kingofthegrid/king-of-the-grid/blob/master/src/rules.cpp) for exact values.
* Bots run on Z80 CPU. See CPUs section.
* Walls (obstacles) are generated before each game starts, such as it is guaranteed there is a path between two bots.
* Food (static) and prey (moves) are spawned periodically.
* Food and Walls are not spawned evenly: random noise is applied using [FastNoiseLite](https://github.com/Auburn/FastNoiseLite) on rules described on [seasons.cpp](src/seasons.cpp)
* Both can move around, eat, scan environment and clone themselves. See [bot_api.h](https://github.com/kingofthegrid/king-of-the-grid/blob/master/bot-api/bot_api.h)
* Bot that survives the longest, wins.
* If both bots survive for too long, it's a draw.

# Live demo

See [kingofthegrid.com](https://kingofthegrid.com/run.html).

# Online IDE to participate

Write your own bot in [an online IDE](https://kingofthegrid.com/ide/)!

# Source code

Source code for the project is located [here](https://github.com/kingofthegrid/king-of-the-grid/).

# How to participate

1. Write your bot in [an online in-browser IDE](https://kingofthegrid.com/ide/) (no downloading needed) or using [this instruction](https://github.com/kingofthegrid/king-of-the-grid?tab=readme-ov-file#how-to-write-your-bot).
2. Open a PR to [bots repository](https://github.com/kingofthegrid/bots) that adds your bot, that adds a file `bots/<your-username>.bin`.
3. After PR is merged, CI/CD will run your bot against other and post results on [kingofthegrid.com](https://kingofthegrid.com).

# Before you submit

Test your bot against others using either [kingofthegrid.com/run.html](https://kingofthegrid.com/run.html) to see how it performs in your browser. You can do this by uploading your bot on one side and select existing bot in another side.

See [examples](https://github.com/kingofthegrid/king-of-the-grid/tree/master/examples) to see how to write your bot. 


