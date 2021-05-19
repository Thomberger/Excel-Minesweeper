# Excel Minesweeper

This project implement a minesweeper game in excel with vba macros.

 <img src="/GIT Images/InGame.jpg" width="49%" ><img src="/GIT Images/Finished.jpg" width="49%" >

## How to Play
To play a game you should download the file and allow excel macros.
Then :
* Go into the "Reglage" sheet
* At the top left change the settings
 * You can change game size and bomb percentage
 * click "Nouvelle Partie" to start a new game
* Play using
  * "Go" or "Ctrl-z" to discover tile
  * "Ca doit etre une bombe !" or "Ctrl-x" to place a bomb-flag

## Cheating
The value of each cell is written in the formula bar therefore you should disable it to correctly play the game: (view/formula bar)
<br><img src="/GIT Images/Formulabar.jpg" width="70%" >

In the "reglage" sheet there is a "cheat section" allowing you to do one these actions:
 * Find all tile containing zeroes
 * Find all tiles that are not bombs
 * Find all tiles that are bombs
 * Discover all tiles


## Solver
In the "Game" sheet there is a button "solve it !". This button try to solve the minesweeper WITHOUT checking the value of the tile. At each iteration the solver do:
* search for tile containing a bomb (by deduction) and mark them as bombs
* search for tiles containing no bomb (by deduction) and discover them
* If there is no more deduction possible (at start for example) try to discover a random tiles

As it is possible no deduction can be made at some steps of a minesweeper game, the solver can lose if it lacks a bit of luck ! <br>The solver looks like that :

<img src="/GIT Images/solver.gif" width="100%" >

## Licence

This software is distributed under the MIT license. Enjoy!
