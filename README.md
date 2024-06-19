# Sudoku Solver

A Java program that solves a 9x9 Sudoku puzzle using a backtracking algorithm.

## Project Description

This project provides a solution to solve a standard 9x9 Sudoku puzzle. The solution uses a backtracking algorithm to fill in the empty cells of the puzzle while ensuring that the Sudoku rules are followed.
This project demonstrates my knowledge of Data Structures and Algorithms, particularly the backtracking technique.

## Sudoku Solver Algorithm

The solver uses a backtracking algorithm:

1. It checks each cell in the 9x9 grid.
2. If a cell is empty (contains 0), it tries all digits from 1 to 9.
3. For each digit, it checks if placing that digit in the current cell is safe by ensuring:
   1. The digit is not repeated in the current row.
   2. The digit is not repeated in the current column.
   3. The digit is not repeated in the current 3x3 subgrid.
4. If a safe digit is found, it is placed in the cell, and the algorithm proceeds to solve the next cell recursively.
5. If no safe digit is found, it backtracks and resets the cell to empty (0).

## Example Sudoku Puzzle

Here is an example of a Sudoku puzzle used in the main method:
                { { 0, 0, 8, 0, 0, 0, 0, 0, 0 },
                { 4, 9, 0, 1, 5, 7, 0, 0, 2 },
                { 0, 0, 3, 0, 0, 4, 1, 9, 0 },
                { 1, 8, 5, 0, 6, 0, 0, 2, 0 },
                { 0, 0, 0, 0, 2, 0, 0, 6, 0 },
                { 9, 6, 0, 4, 0, 5, 3, 0, 0 },
                { 0, 3, 0, 0, 7, 2, 0, 0, 4 },
                { 0, 4, 9, 0, 3, 0, 0, 5, 7 },
                { 8, 2, 7, 0, 0, 9, 0, 1, 3 } }

## Output

If a solution exists, the program will output the solved Sudoku grid. If no solution exists, it will output "Solution does not exist".

## How to Use

1. Clone this repository to your local machine:
   ```sh
   git clone https://github.com/ratnesh1253/SudokuSolver.git
   cd SudokuSolver
2. Compile the `Sudoku.java` file:
   ```sh
   javac Sudoku.java
3. Run the `Sudoku` program:
   ```sh
   java Sudoku

## Contact
For any questions or feedback, please contact [email](mailto:ratneshkshirsagar1253@gmail.com).
