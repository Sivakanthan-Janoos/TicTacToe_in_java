# Tic Tac Toe (Java)

A classic Tic Tac Toe game built in Java with an interactive GUI and object-oriented design.

## About
This repository contains a Java implementation of Tic Tac Toe that showcases a GUI-based interactive game and an object-oriented approach to game logic. The project is suitable as a beginner-to-intermediate programming exercise, a demo app for learning GUI basics, or a foundation for adding features like AI opponents, network play, or persistence.

## Demo
![image alt](https://github.com/Sivakanthan-Janoos/TicTacToe_in_java/blob/fa791468c1b7fec97794a06320c1856bc24f524e/TicTacToe.png)

## Features
- Interactive graphical board (click a cell to play)
- Two-player local gameplay (Player X and Player O)
- Win/draw detection and end-of-game notification
- Option to restart the game
- Clean, object-oriented code suitable for study and extension

## Requirements
- Java 8 or newer (Java 11 or 17 recommended)
- A Java IDE (IntelliJ IDEA, Eclipse, NetBeans) or JDK with command-line tools
- (Optional) Maven or Gradle if you add a build file

## Installation & Run

Clone the repository:
```bash
git clone https://github.com/Sivakanthan-Janoos/TicTacToe_in_java.git
cd TicTacToe_in_java
```

### Option A - Run in your IDE (recommended)
1. Open the project in IntelliJ IDEA, Eclipse, or NetBeans.
2. Locate the class with the `public static void main(String[] args)` method (often named `Main`, `TicTacToe`, or `TicTacToeApp`).
3. Run the main class. The GUI window should appear and the game is playable.

If you prefer, update this README with the exact main class name so users can run it directly.

### Option B - Build and run from source (javac/java)
If the project uses no build tool and is plain `.java` files, compile and run using javac/java:

1. Compile (example — adapt paths to match your project structure):
```bash
# compile all .java files under src/
javac -d out $(find src -name "*.java")
```

2. Run (replace `your.package.MainClass` with the actual main class full name):
```bash
java -cp out your.package.MainClass
```

### Option C - Build with Maven or Gradle (if available)
If you add a Maven `pom.xml` or Gradle `build.gradle`:

Maven:
```bash
mvn package
java -jar target/tictactoe-<version>.jar
```

Gradle:
```bash
./gradlew build
java -jar build/libs/tictactoe-<version>.jar
```

(Replace `<version>` and jar name based on your build configuration.)

## How to play
- Two players take turns placing their mark (X or O) on a 3x3 grid.
- Click a cell to place your mark.
- The first player to place three of their marks in a horizontal, vertical, or diagonal row wins.
- If all cells are filled without a winning row, the game is declared a draw.
- Use the "New Game" or "Restart" control (if present) to play again.

## Architecture & Design
This project follows an object-oriented approach. Typical components you will find or can model:
- Game model (represents board state, win/draw logic)
- Player abstraction (human, and optionally AI)
- Game controller (turn management, validation)
- GUI/view (renders board, handles input/events)

Suggested classes (names may vary):
- GameBoard (board representation, move validation, win detection)
- GameController (game loop, current player handling)
- TicTacToeUI (Swing/JavaFX GUI that displays the board and handles clicks)
- Player (possibly HumanPlayer, AIPlayer)

If you want, I can open the repository and produce a class-by-class summary based on the actual files.

## Extending the project
Ideas for improvements:
- Add a single-player mode with AI (minimax, heuristics)
- Allow different board sizes (4x4, 5x5) and win lengths
- Add keyboard controls, animations, and sound effects
- Add persistent scorekeeping or player profiles
- Add unit tests for game logic using JUnit
- Add packaging (executable JAR) and a build pipeline (GitHub Actions)

## Troubleshooting
- GUI doesn't appear: ensure you are running the correct `main` class and Java version is compatible.
- Compilation errors: check package declarations and classpath. If you used `javac` directly, ensure `-d` output directory and classpath are correct.
- If you want, paste compilation errors here and I will help debug them.

## Contributing
Contributions are welcome! A suggested contribution flow:
1. Fork the repository
2. Create a feature branch: `git checkout -b feat/awesome-feature`
3. Make changes and commit with clear messages
4. Push: `git push origin feat/awesome-feature`
5. Open a pull request describing the change

Please include tests for logic changes and update the README (screenshots, instructions, or badges) when you add major features.

Consider adding a CONTRIBUTING.md and CODE_OF_CONDUCT.md for larger projects.

## Acknowledgements
- Classic Tic Tac Toe rules and many public examples of GUI implementations.
- Any resources, tutorials, or libraries you used — list them here.
