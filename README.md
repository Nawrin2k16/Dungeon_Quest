Here's the merged and refined `README.md` file for your Dungeon-Quest game:

---

# Dungeon-Quest: A Turn-Based Grid Adventure

## Overview
**Dungeon Quest** is an interactive, grid-based survival game where strategy, adventure, and AI-driven challenges collide. The player must navigate through a dynamic dungeon to reach the treasure while avoiding pursuing monsters. With each level, the difficulty escalates: grid sizes double, new obstacles appear, and the number of monsters increases, requiring increasingly sophisticated tactics.

## Features
1. **Grid-Based Gameplay:**
   - The dungeon is represented as a grid, with cells that may contain obstacles, the player, monsters, or treasures.
   - Players move up (`u`), down (`d`), left (`l`), or right (`r`) to navigate the dungeon and avoid obstacles.

2. **Dynamic Environment:**
   - Obstacles shift periodically, altering the dungeon layout and forcing players to adapt their strategy.
   - Treasure disappears after a set number of moves and reappears at random locations, creating a time-pressure element.

3. **Levels & Progression:**
   - Players progress through levels by reaching the treasure.
   - Each level increases the grid size (doubling with each level) and adds new monsters, making it more difficult to survive.
   - As the levels advance, more monsters are introduced, requiring players to use even more advanced strategies to avoid them.

4. **Challenging Monster AI:**
   - Monsters use pathfinding algorithms such as BFS, A*, or reinforcement learning to track the player or treasure.
   - The AI adapts as levels progress, becoming smarter and harder to evade.
   - Multiple monsters appear as the levels increase, working together to corner the player and prevent them from reaching the treasure.

5. **Game Over Conditions:**
   - The player is caught by a monster, or they fail to reach the treasure in time.
   - The monster reaches the treasure before the player does.

6. **Treasure Mechanics:**
   - The treasure disappears after a set number of moves, forcing the player to wait for it to reappear at a new random location.
   - When the treasure reappears, it spawns in a random, empty cell, adding an extra layer of challenge.

## Technical Highlights
- **Algorithms:** The game utilizes BFS, A*, and reinforcement learning to guide the monsters' movements, adapting to player behavior.
- **Randomized Obstacles:** Dynamic, randomized obstacles make each gameplay session unique, increasing replayability.
- **Scalable Difficulty:** The game's difficulty scales as the player progresses, with increasing grid sizes, more monsters, and smarter AI.

## How to Play
1. Upon starting, enter the dungeon size and begin navigating using the keyboard (`u`, `d`, `l`, `r` for up, down, left, and right).
2. Your goal is to avoid monsters, survive shifting obstacles, and reach the treasure.
3. If you successfully reach the treasure, you progress to the next level. Each new level has a larger grid and more monsters.
4. The game ends if you are caught by a monster or if the monster reaches the treasure before you do.

## Requirements
- Python 3.x
- NumPy (for grid representation and calculations)

## Installation & Running
1. Clone the repository:
   ```bash
   git clone https://github.com/Nawrin2k16/Dungeon_Quest.git
   cd dungeon-quest
   ```

2. Install the required dependencies:
   ```bash
   pip install numpy
   ```

3. Run the game:
   ```bash
   python dungeon_escape.py
   ```

## Future Improvements
- Implement a graphical interface using libraries like `pygame`.
- Add multiple difficulty modes to cater to a wide range of players.
- Introduce new AI behaviors and power-ups for the player.
- Develop a multiplayer mode for cooperative or competitive gameplay.

---

Enjoy the challenge of **Dungeon Quest**, where strategy and wit determine your survival!
