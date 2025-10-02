# Minesweeper 💣

Welcome to Minesweeper, a classic implementation of the beloved puzzle game, built entirely in C and designed to run in the **command line**. This project was developed as a mini-project for a first-semester Computer Engineering course.

The game features a colorful, text-based UI, complete with animations for a more engaging user experience.

---
## ✨ Features

* **Classic Minesweeper Gameplay**: Enjoy the timeless logic puzzle right in your terminal.
* **Colorful Terminal UI**: Utilizes ANSI escape codes for a vibrant and clear game board, making numbers and flags easy to distinguish.
* **Smooth Animations**: Features a "typewriter" welcome message and flashing screen effects for wins and losses.
* **Two Game Modes**:
    * **Beginner**: An 8x8 grid with 10 mines.
    * **Intermediate**: A 16x16 grid with 40 mines.
* **Player Profiles**: Enter your name and track your win/loss statistics for the current session.
* **Interactive Menu**: Easily navigate between playing, changing your username, starting as a new player, or exiting the game.

---
## 🛠️ Technologies Used

* **Language**: **C**
* **Standard Libraries**: `stdio.h`, `stdlib.h`, `time.h`, `string.h`

---
## 🚀 Getting Started

To compile and run this game on your local machine, follow these simple steps.

### Prerequisites

You will need a C compiler, such as **GCC** or **MinGW**, installed on your system.

### Compilation & Execution

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  **Navigate to the project directory:**
    ```sh
    cd your-repo-name
    ```
3.  **Compile the source code.** Assuming the file is named `main.c`:
    ```sh
    gcc main.c -o minesweeper
    ```
    > **Note:** The code uses `_sleep()` for animations, which is specific to Windows. If you are on **Linux or macOS**, you may need to replace `_sleep()` with `usleep()` and include `<unistd.h>`. The `system("cls||clear")` command should work on both Windows and Unix-like systems.

4.  **Run the game:**
    * On **Windows**:
        ```sh
        .\minesweeper.exe
        ```
    * On **Linux / macOS**:
        ```sh
        ./minesweeper
        ```

---
## 룰 How to Play

1.  After launching the game, you'll be greeted by the main menu where you can enter your name.
2.  Choose **Play** and select a game mode (8x8 or 16x16).
3.  The game board will be displayed. To make a move, use the format: **`Row Column Action`**.
    * **Row**: The row number of the cell.
    * **Column**: The column number of the cell.
    * **Action**:
        * `L` or `l` to **reveal** (open) a cell.
        * `R` or `r` to place or remove a **flag** on a cell.

4.  **Example**: To reveal the cell at row 2, column 3, you would type:
    ```
    2 3 l
    ```
5.  Find and place flags on all the mines to win the game! Hitting a mine results in a loss.

---
## 👤 Author

This project was created by **ALISHA**.

---
## 📄 License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.