# Chay Khoi DEADLINE (Escape the DEADLINE)

![Game Demo](images/2026-05-23%2017-44-01%20(online-video-cutter.com).gif)

A 2D top-down arcade space shooter game built in Java using the Swing and AWT frameworks. In this game, players pilot a spacecraft to navigate through space, destroy incoming hazards, collect vital supplies, and survive as long as possible to achieve the highest score.

## Game Concept

The game is themed around escaping "DEADLINE," represented as challenging and hostile entities in space. The player must use reflexes and strategic movement to dodge homing missiles, avoid explosive stars, shoot down incoming meteorites, and replenish resources such as ammunition and health before getting overwhelmed.

## Game Controls

- Move Up: W or UP Arrow
- Move Down: S or DOWN Arrow
- Move Left: A or LEFT Arrow
- Move Right: D or RIGHT Arrow
- Shoot: SPACE
- Restart (on Game Over screen): R

## Requirements

- Java Development Kit (JDK) 11 or higher.
- Java Swing and AWT library support (packaged natively with standard JDKs).

## Running the Game

1. Clone or download the repository to your local machine.
2. Open the project folder in your preferred IDE (e.g., IntelliJ IDEA, Eclipse, NetBeans) or terminal.
3. Locate the entry point file at:
   src/main/Main.java
4. Compile and run Main.java to start the game frame.


## Key Features

- Fluid Controls and Rotation: The player plane rotates dynamically to face the direction of movement (supporting 8-directional movement) and features multi-frame sprite animations to simulate propulsion.
- Diverse Hazards:
  - Meteorites: Spawn dynamically and fly linearly across the screen. Can be shot down for points.
  - Homing Rockets: Track the player's position continuously in real-time. Can be blown up or guided into colliding with meteorites.
  - Exploding Stars: Dangerous celestial bombs that enter a countdown state for 3 seconds before detonating, creating a massive expanding shockwave that deals heavy, multi-tick damage to the player and obliterates nearby entities.
- Resource Items:
  - HP Packs: Restores the spacecraft's health points (HP).
  - Ammo Crates: Adds ammunition to allow continuous weapon firing.
  - Decay Mechanic: Uncollected items naturally decay and disappear after 10 seconds.
- High Score Persistence: Automatically tracks your performance and saves the all-time high score locally in a "highscore.dat" data file.
- Rich Sound Effects and Playlists: Employs a robust SoundManager to handle continuous background music (BGM), collision sound effects (SFX), and randomized fun commentary tracks.
- Clean Object-Oriented Architecture: Fully utilizes core OOP concepts including inheritance, polymorphism, and encapsulation. All game entities inherit from a base Entity class and override drawing, update, and resource-loading behaviors.
