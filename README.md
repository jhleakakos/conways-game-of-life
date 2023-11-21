# conways-game-of-life

Small demo of Conway's Game of Life.

There are two outputs:
- Print: gives terminal output for game state
- Draw: gives graphical output through matplotlib for game state

The main logic behind this is the set of rules for when a cell survives, dies, or comes alive.
- If a cell is alive, it will survive if it has two or three neighbors
  - If it has any more or less, then it dies
- If a cell is dead, it will come alive if it has exactly two neighbors

You set a starting state by passing initial live cells as a list of tuples to the ```populate_grid()``` method

Once the game starts, you can see how the initial state plays out by choosing a number of steps to proceed into the
game with the ```make_n_steps()``` method.

## Areas for Improvement
- add animation between game states
- refactor nested for-loops to improve performance
- clean up visual display to make the key changes easier to follow