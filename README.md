Bomberman - JavaFX Game

A classic Bomberman clone developed with Java and JavaFX for an Object-Oriented Programming course.

Features
* Four playable levels of increasing difficulty.
* A point-based scoring system.
* A 180-second time limit for each level.
* Lobby and gameplay scenes managed via FXML.
* Includes a dedicated controller for audio management.

Tech Stack
* Language: Java
* Framework: JavaFX

Getting Started

1.  Prerequisites: JDK 11+ and the JavaFX SDK are required.
2.  Clone: Clone the repository to your local machine.
3.  Configure IDE:
    * Open the project in your IDE (e.g., IntelliJ IDEA).
    * Add the JavaFX SDK as a project library.
    * Set the following VM options in your Run Configuration:
        ```
        --module-path /path/to/your/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml,javafx.media
        ```
4.  Run: Execute the `main` method in `hust.oop.bomberman.BombermanGame`.

Code Overview

* `BombermanGame.java`: The main application entry point that launches the game.
* `GameController.java`: The central controller that manages game state, scenes, points, and the main game loop via an `AnimationTimer`.
* `Level.java`: Manages the logic and rendering for a single game level, including the map and all entities on a `Canvas`.

How to Play
* Objective: Defeat all enemies and find the hidden exit before the timer runs out.
* Controls: Use the arrow keys to move and the spacebar to drop bombs.
