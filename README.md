# Dungeon Game README

Welcome to the Dungeon Game! This is an exciting and challenging game where you navigate through a dungeon filled with monsters, obstacles, and treasures. The goal is to reach the treasure before the monsters catch you, all while avoiding obstacles and managing your limited moves.

## Table of Contents
- [Introduction](#introduction)
- [Game Setup](#game-setup)
- [Gameplay Instructions](#gameplay-instructions)
- [Game Logic](#game-logic)
- [Monsters and Obstacles](#monsters-and-obstacles)
- [Pathfinding Algorithms](#pathfinding-algorithms)
- [Level System](#level-system)
- [Functionality Breakdown](#functionality-breakdown)
- [Running the Game on Google Colab](#running-the-game-on-google-colab)

---

## Introduction

The Dungeon Game takes you through multiple levels of increasing difficulty. Each level features:
- A player who must navigate the dungeon,
- Monsters that try to catch the player,
- Obstacles that make the journey tricky,
- A treasure that the player must reach before the monsters do.

Your movement is limited by a number of moves per level, and you must avoid monsters while navigating through the dungeon's obstacles.

---

## Game Setup

The dungeon is a grid-based layout where different elements are placed, including:
- **Player**: Your character represented by an emoji (`🧑`, `👩`, `👨`, etc.).
- **Monsters**: Various monsters (`👹`, `😈`, `🧟`, etc.) that are randomly placed and try to capture you. their number increase with level.
- **Obstacles**: Items such as fire (`🔥`), stones (`🪨`), and other barriers that make navigation difficult.
- **Treasure**: Valuable items like diamonds (`💎`) and trophies (`🏆`) placed in the dungeon, which you need to collect to win.

---

## Gameplay Instructions

1. **Movement**:
   - Use the following keys to move: 
     - `u` for up, 
     - `d` for down,
     - `l` for left, 
     - `r` for right.
   - You need to avoid monsters and obstacles while navigating the dungeon.

2. **Objective**:
   - Your objective is to reach the treasure (`3`) before the monsters catch you (`4`).
   - You must also avoid obstacles (`1`), and if you encounter one, you can't move through it.

3. **Game Over**:
   - If a monster reaches you or if you run out of moves, you lose.
   - If you reach the treasure, you win the level and progress to the next one.

---

## Game Logic

1. **Grid Creation**:
   - The dungeon is initialized with obstacles, monsters, and a treasure.
   - The player always starts in the top-left corner of the grid, and the treasure starts in the bottom-right corner.

2. **Pathfinding**:
   - The monsters use different pathfinding algorithms to move toward the player or treasure:
     - **BFS (Level 1)**: Monsters use Breadth-First Search to find the shortest path.
     - **A* (Level 2)**: Monsters use the A* algorithm, which is more efficient and optimized.
     - **Reinforcement Learning (Level 3)**: Monsters learn optimal movement strategies.

3. **Movement**:
   - Players move by entering commands (`u`, `d`, `l`, `r`).
   - The monsters move every turn based on their pathfinding algorithms, pursuing the player or treasure.

4. **Level Progression**:
   - The game has multiple levels, each with increasing difficulty.
   - At each level, the grid size increases, and the monsters' movement strategies improve.

---

## Monsters and Obstacles

- **Monsters**: The game features different monsters that move toward the player or treasure. These monsters use different algorithms (BFS, A*, and reinforcement learning) to find the shortest path to their target.
  
- **Obstacles**: Obstacles like fire (`🔥`), stones (`🪨`), and traps (`🛑`) are scattered throughout the grid. Players must navigate around these to avoid getting stuck.

- **Treasure**: The treasure is placed in a reachable location on the grid, and players must reach it before the monsters do.

---

## Pathfinding Algorithms

- **BFS (Breadth-First Search)**: Used in Level 1. It guarantees the shortest path but does not consider optimal routes or obstacles.
  
- **A***: Used in Level 2. A* uses both distance and heuristic to find the shortest and most efficient path to the target.

- **Reinforcement Learning**: Used in Level 3 and higher. The monster learns from its experiences, optimizing its movement strategies using a Q-table.

---

## Level System

- **Level 1**: Simple grid with basic BFS pathfinding for monsters.
- **Level 2**: Grid size increases, and monsters use A* pathfinding.
- **Level 3**: More complex grid with reinforcement learning for monsters' movement.

---

## Running the Game on Google Colab

To play the Dungeon Game, follow these steps:

1. open the Dungeon Game notebook in Google Colab.
2. Run the notebook cells sequentially to play the game directly in your browser.

No setup is required other than running the cells, and you can start playing right away!

Thank you for playing! We hope you enjoy your dungeon adventure! 😄🎮
