# Artificial Intelligence Nanodegree
## Diagonal Sudoku Solver

## Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: We first find the boxes with two digits. Then we find the peers of these boxes with the same values, leading to pairs of twin. For each twin pair, we find the set of shared peers. For each set, we remove the digits of the twin pair boxes in the digits of each box in the set. In short, this technique reduces the search space for some boxes in the sudoku.

## Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: In addition to the elimination technique and only-choice technique, we employ the naked-twins technique to reduce the search space for each box. All three techniques are applied repetitively on the sudoku until no changes can be made, then we use the search technique to further reduce the search space. Also, besides the normal units, we also need to add in the two diagonal units to the unit list.

### Install

This project requires **Python 3**.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).
