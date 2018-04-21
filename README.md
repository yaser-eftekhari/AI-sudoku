# Solve Sudoku with AI

## Synopsis

In this project, we develop a Sudoku-solving agent to solve _diagonal_ Sudoku puzzles. The agent uses three techniques: 1) Constraint propagation, 2) Naked twins strategy, and 3) Search. A diagonal Sudoku puzzle is identical to traditional Sudoku puzzles with the added constraint that the boxes on the two main diagonals of the board must also contain the digits 1-9 in each cell (just like the rows, columns, and 3x3 blocks).


## Quickstart Guide

1. Install and configure the `aind` [Anaconda](https://www.continuum.io/downloads) environment which includes several important packages that are used for the project.

  `conda env create -f aind-universal-v2.yml`

 OS X or Unix/Linux users can activate the aind environment by running the following (Windows users simply run `activate aind`):

    `$ source activate aind`

2. You can run a small set of test cases using the local test suite.

    `(aind)$ python -m unittest -v`

3. You can run the code with visualization (see the last section of the readme for more information)

    `(aind)$ python solution.py`


## Visualization

**Note:** The `pygame` library is required to visualize your solution -- however, the `pygame` module can be troublesome to install and configure. It should be installed by default with the AIND conda environment, but it is not reliable across all operating systems or versions. Please refer to the pygame documentation [here](http://www.pygame.org/download.shtml), or discuss among your peers in the slack group or discussion forum if you need help.

Running `python solution.py` will automatically attempt to visualize your solution, but you must use the provided `assign_value` function (defined in `utils.py`) to track the puzzle solution progress for reconstruction during visualization.
