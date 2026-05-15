Bomberman - JavaFX Game

A classic Bomberman-inspired arcade game developed using Java and JavaFX as part of an Object-Oriented Programming (OOP) course project.
The game recreates the nostalgic Bomberman gameplay experience while applying core software engineering and OOP principles such as inheritance, polymorphism, encapsulation, modular design, scene management, and event-driven programming.

The project focuses not only on gameplay mechanics but also on clean architecture, maintainable code structure, and interactive user experience through JavaFX.

Project Overview

This game allows players to control a bomber character through multiple levels filled with enemies, obstacles, destructible walls, hidden exits, and timed challenges.

The player must strategically place bombs to destroy enemies and clear paths while avoiding explosions and enemy collisions.
Each level increases in difficulty, introducing more complex enemy movement, map layouts, and survival challenges.

The project was built with:

Java for core game logic
JavaFX for graphics rendering and UI management
FXML for scene and interface organization
AnimationTimer for the real-time game loop
Object-Oriented Programming principles for scalable architecture
Main Features
Multiple Playable Levels

The game contains four different levels, each designed with:

Unique map layouts
Different enemy placements
Increasing gameplay difficulty
More challenging navigation and timing mechanics

As players progress through levels, enemy density and environmental complexity increase, requiring better movement and bomb placement strategies.

Real-Time Gameplay System

The game runs using a real-time update loop implemented with JavaFX's AnimationTimer.

This loop is responsible for:

Updating entity positions
Rendering game objects
Detecting collisions
Managing explosions
Handling enemy AI movement
Updating the countdown timer
Refreshing score and game state
Score System

A point-based scoring system is included to track player performance.

Players earn points by:

Defeating enemies
Completing levels
Destroying obstacles
Finishing stages efficiently

The scoring system encourages replayability and competitive gameplay.

Countdown Timer

Each level includes a 180-second time limit.

The timer adds pressure and strategic pacing to gameplay:

Players must clear levels before time expires
Efficient bomb placement becomes essential
Slow gameplay can result in failure even without losing lives
Bomb and Explosion Mechanics

The bomb system simulates classic Bomberman gameplay:

Players can place bombs on the map
Bombs explode after a short delay
Explosions spread in multiple directions
Walls and enemies can be destroyed
Players must avoid their own explosions

Explosion range and collision detection are handled dynamically within the game engine.

Enemy AI

Enemies move autonomously around the map and create obstacles for the player.

Enemy behaviors include:

Random movement patterns
Collision interaction
Player damage upon contact
Path blocking and area control

This creates continuous pressure and increases gameplay intensity.

Scene Management with FXML

The project uses JavaFX FXML files to separate:

UI design
Scene structure
Controller logic

Different scenes include:

Lobby/Menu Scene
Gameplay Scene
Game Over Screen
Victory/Completion States

This separation improves maintainability and keeps the architecture organized.

Audio Management System

The project contains a dedicated audio controller responsible for:

Background music
Explosion sound effects
Menu audio
Gameplay feedback sounds

Using a centralized audio management system makes the project more modular and easier to extend.

Technologies Used
Programming Language
Java
Framework & Libraries
JavaFX
JavaFX FXML
JavaFX Media
Programming Concepts Applied
Object-Oriented Programming (OOP)
Inheritance
Polymorphism
Encapsulation
Abstraction
Event-driven Programming
MVC-inspired structure
Project Structure
src/
│
├── hust/oop/bomberman/
│   ├── BombermanGame.java
│   ├── controllers/
│   ├── entities/
│   ├── graphics/
│   ├── levels/
│   ├── audio/
│   ├── utils/
│   └── ...
│
├── resources/
│   ├── fxml/
│   ├── images/
│   ├── sounds/
│   └── maps/
Getting Started
Prerequisites

Before running the project, ensure the following are installed:

JDK 11 or higher
JavaFX SDK
IntelliJ IDEA (recommended)
Installation Guide
1. Clone the Repository
git clone <repository-url>
2. Open Project in IDE

Open the project using:

IntelliJ IDEA
Eclipse
VSCode (with Java extensions)
3. Configure JavaFX SDK

Download and configure the JavaFX SDK:

Add JavaFX as a project library
Ensure the SDK path is correctly linked
4. Configure VM Options

Add the following VM options in your Run Configuration:

--module-path /path/to/your/javafx-sdk/lib --add-modules javafx.controls,javafx.fxml,javafx.media

Replace:

/path/to/your/javafx-sdk/lib

with the actual JavaFX SDK location on your machine.

5. Run the Application

Execute:

hust.oop.bomberman.BombermanGame

The game window should launch successfully.

Gameplay Instructions
Objective

The main goal is to:

Eliminate all enemies
Discover the hidden exit
Complete the level before the timer reaches zero
Controls
Key	Action
Arrow Keys	Move character
Spacebar	Place bomb
Core Classes Overview
BombermanGame.java

The main entry point of the application.

Responsibilities:

Launching JavaFX application
Initializing scenes
Loading resources
Starting the game
GameController.java

Acts as the central game manager.

Responsibilities:

Managing game states
Updating score
Handling level transitions
Running the main game loop
Coordinating rendering and updates

Uses JavaFX AnimationTimer for real-time gameplay execution.

Level.java

Represents and manages a single game level.

Responsibilities:

Loading map data
Rendering map tiles
Managing entities
Handling collisions
Updating gameplay logic
Object-Oriented Design

This project demonstrates multiple important OOP concepts.

Encapsulation

Game entity data and behaviors are wrapped into separate classes.

Inheritance

Different entities inherit from common parent classes, reducing duplicated code.

Example:

Character
Enemy
Bomb
Wall
Polymorphism

Different game entities can override update and render methods for customized behavior.

Modularity

The project separates:

Rendering
Audio
Game logic
Input handling
UI management

This improves maintainability and scalability.

Future Improvements

Potential future features include:

Multiplayer support
Smarter enemy AI
Power-up system
Save/load game functionality
Additional levels
Boss battles
Animated visual effects
Custom map editor
Online leaderboard
Learning Outcomes

Through this project, the development team gained experience in:

JavaFX application development
Real-time game programming
Game loop architecture
Scene management
Collision detection
Event handling
OOP software design
Team collaboration and project organization
Conclusion

This Bomberman project is a complete arcade-style game built with Java and JavaFX, combining classic gameplay mechanics with strong object-oriented software design principles.

The project serves as both:

A functional and enjoyable game
A practical demonstration of Java OOP and JavaFX development skills

It highlights the ability to design modular systems, manage real-time rendering, and implement interactive gameplay mechanics in a desktop application environment.
