# Sudoku-Puzzle
A web-based game based on the concepts of **recursion and backtracking** , that allows the player to **generate** as well as **solve** the given 9x9 sudoku puzzle


## Description
**_Sudoku_** is one of the most popular puzzle games of all time. The objective of Sudoku is to fill a 9x9 grid with digits from 1 to 9 such that each column, row, and box *(or called 'subgrid', 'region', 'block')* contain every number in the set {1, ... , 9} exactly once.

This web application features generating and solving standard 9x9 Sudoku puzzles using the **backtracking algorihtm** for the same.

<p>
    <img src="https://user-images.githubusercontent.com/95221972/181872637-34fa141d-6f4c-416f-91cf-e6f1806b3634.png" width=500>
</p>

## Working of the Algorithm 
The sudoku is essentially a constraint satisfaction problem. Each empty cell has a set of potential numbers that can be filled in while maintaining the consistency with respect to the Sudoku rules i.e., each cell can be filled with 1 to 9 and no numbers should repeat in a row or column or same block/sector.

1. Pick an empty cell
2. Fill with one of the potential numbers that doesn't break the consistency
3. Find another empty cell and repeat step 2. If there are no potential numbers, backtrack to the previous cell that was filled and choose another potential number
4. Repeat steps 1 to 3 until all the cells are filled

Finding the next cell to fill requires a heuristic. The cell with the least number of potential numbers is chosen everytime. This reduces the number of backtracks significantly.

### **<a href="https://bhagatananya05.github.io/Sudoku-Puzzle/">Demo</a>**

![](https://user-images.githubusercontent.com/95221972/181872541-a3d3062c-2a43-4cdd-a8dc-fbd139412196.gif) 



