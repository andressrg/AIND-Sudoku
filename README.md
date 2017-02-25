# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A:
The main idea of constraint propagation is to reduce the search space of our problem.

Naked twins are 2 boxes with the same 2 possible values on a given unit.

In this unit we are able to remove both possible values of the twins from their peers.

With this reduction we have a smaller space of possibilities and can get closer to a solution.

Its important to note that this space reduction via constraint propagation must be faster than just doing the search anyway.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A:
As the previous answer the main idea of constraint propagation is to reduce the search space of the problem.

Here we have three strategies that use constraint propagation to solve diagonals sudoku: elimination, only choice and naked twins. We use this constraint propagation techniques the same way as with normal sudokus but with a small difference: we use the diagonals of the sudoku as another unit to consider in our strategies. This means we have 4 kinds of units now: rows, columns, squares and diagonals. But other than that the idea of constraint propagation is the same: use different rules that we know are true in order to reduce the search space of the problem and solve it faster than only doing plain search.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
