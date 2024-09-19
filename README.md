# Sudoku Game

This is a graphical Sudoku game built using Java and Swing. The game allows users to play, clear, solve, and restart Sudoku puzzles. Additionally, the game includes functionality to solve individual cells or the entire board.

## Features

- **New Game**: Generates a random Sudoku puzzle from a predefined list.
- **Solve**: Automatically solves the entire Sudoku puzzle.
- **Solve Cell**: Solves only the currently selected cell.
- **Clear**: Clears the entire Sudoku board.
- **Restart**: Restarts the game with the current puzzle.

## Project Structure

- **Main Class**: `Sudoku.java`
  - Contains the main logic for the game, including event handling and board setup.
  - Sudoku solving logic implemented using backtracking algorithm.

## How to Run

1. **Clone the Repository:**

    ```bash
    git clone <repository-url>
    ```

2. **Compile and Run:**

    To compile the project, ensure you have the JDK installed and run the following command:

    ```bash
    javac Sudoku.java
    ```

    After compilation, run the game using:

    ```bash
    java Sudoku
    ```

## Dependencies

- **Java Development Kit (JDK)**: The game requires JDK 8 or above to compile and run.

## Controls

- **Number Input**: Select a cell and type a number (1-9) on your keyboard to fill the cell.
- **Backspace**: Deletes the number in the selected cell.
- **Mouse Click**: Click on a cell to select it.

## GUI Components

- **Buttons**:
    - `New Game`: Starts a new Sudoku puzzle.
    - `Solve`: Solves the entire puzzle.
    - `Solve Cell`: Solves the currently selected cell.
    - `Clear`: Clears the entire board.
    - `Restart`: Restarts the current puzzle.

- **Grid**: A 9x9 grid representing the Sudoku board.

## Logic for Sudoku Solver

The Sudoku solver is implemented using a **backtracking algorithm**. The following methods are used:
- **isNumberInRow()**: Checks if a number is present in a specific row.
- **isNumberInColumn()**: Checks if a number is present in a specific column.
- **isNumberInBox()**: Checks if a number is present in the 3x3 subgrid.
- **solveBoard()**: Recursively tries to solve the Sudoku board by placing numbers and backtracking if an invalid placement is found.

## Future Enhancements

- Timer to track how long it takes to solve the puzzle.
- Add difficulty levels (easy, medium, hard).
- Implement a scoring system.

## Contributing

Feel free to open issues and contribute to the project by submitting pull requests.

## License

This project is open-source and available under the [MIT License](LICENSE).
