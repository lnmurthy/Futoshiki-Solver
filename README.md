# Futoshiki Solver

## Project Details:

- Course: Artificial Intelligence, NYU

## Project Description:

Welcome to our Futoshiki Solver project! Here, we implement the Backtracking Algorithm for Constraint Satisfaction Problems (CSPs) to solve 5 × 5 Futoshiki puzzles. 

### Puzzle Rules:

- The game board consists of 5 × 5 cells. Some cells already have numbers (1 to 5) assigned to them, while others are empty.
- Inequality signs (< or >) are placed horizontally or vertically between some adjacent cells.
- The goal is to find assignments (1 to 5) for the empty cells such that:
    - The inequality relationships between adjacent cells are satisfied.
    - Each digit appears only once in every row and column.

### Algorithm Details:

We implement the Backtracking Algorithm for CSPs to solve the puzzle. We employ the following strategies:
- In the `SELECT-UNASSIGNED-VARIABLE` function:
    - We use the minimum remaining value heuristic.
    - In case of a tie, we use the degree heuristic as a tiebreaker.
    - If multiple variables remain after applying the degree heuristic, we arbitrarily choose one.
- We do not implement the least constraining value heuristic in the `ORDER-DOMAIN-VALUES` function; instead, we simply order the domain values in increasing order (from 1 to 5).
- We do not implement the `INFERENCE` function in the Backtracking Algorithm.

### Input and Output:

- The program reads values from an input text file representing the initial game board.
- The format of the input file includes:
    - Initial cell values (each row contains five integers, ranging from 0 to 5; 0 indicates a blank cell).
    - Horizontal and vertical inequalities (each row contains five integers, with 0 indicating no inequality).
- The program produces an output text file containing the solution.
- The format of the output file includes:
    - Five rows of integers, each containing five integers ranging from 1 to 5, separated by blanks.

## Team:

- Team Members: [Leisha Murthy, Andrew Asseily]

## Languages:

- Python
