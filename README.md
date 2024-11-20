# **Dungeon Escape: A Turn-Based Grid Adventure**

## **Overview**
Dungeon Escape is a thrilling turn-based game that combines strategy, survival, and unpredictability. Players navigate through a dynamic dungeon grid, avoiding a relentless monster while chasing a treasure that may disappear and reappear at any moment. The game features multiple levels of increasing difficulty, where the grid size doubles as you progress, adding new challenges to the gameplay.

## **Key Features**

### 1. **Dynamic Grid Dungeon**
- A dungeon is represented as a grid filled with obstacles, treasures, and an ever-moving monster.
- Obstacles randomly shift after a certain number of moves, ensuring that each turn feels fresh and unpredictable.

### 2. **Player Movement**
- Use simple commands (`u`, `d`, `l`, `r`) to move up, down, left, or right on the grid.
- Strategy is crucial to avoid the monster while working your way toward the treasure.

### 3. **Treasure Logic**
- The treasure doesn't stay in one place for long! It disappears and reappears unpredictably after a set number of turns, keeping players on edge.

### 4. **AI-Controlled Monster**
- The monster actively chases the player or treasure using one of three algorithms, based on the difficulty level:
  - **Level 1:** Random movements based on reinforcement learning.
  - **Level 2:** A* Pathfinding for smarter pursuit.
  - **Level 3:** BFS (Breadth-First Search) for optimized tracking.
- The monster poses a constant threat, and getting caught ends the game.

### 5. **Increasing Difficulty**
- As you progress through levels, the grid size doubles, creating more complex environments to navigate.
- Treasure and monster logic become more challenging as the dungeon evolves.

### 6. **Randomized Obstacles**
- Walls are placed randomly, ensuring that each game feels unique.
- Even as walls shift, paths to the treasure and escape from the monster are always ensured.

### 7. **Winning and Losing Conditions**
- **Win:** Reach the treasure before the monster to proceed to the next level.
- **Lose:** Get caught by the monster or make an invalid move into a blocked cell.

### 8. **Replayability**
- Procedural dungeon generation, random obstacle placement, and dynamic treasure behavior make each playthrough unique.

## **How to Play**
1. Choose the dungeon size and start the game at Level 1.
2. Use keyboard commands to navigate through the dungeon.
3. Avoid the monster and obstacles while aiming to reach the treasure.
4. Survive treasure disappearance phases and adapt to dungeon shifts.
5. Progress through levels to complete the game!

## **Target Audience**
Dungeon Escape appeals to fans of roguelike, strategy, and survival games. It is designed for players who enjoy dynamic challenges, puzzle-solving, and adaptive AI opponents.

## **Technical Highlights**
- Built using Python with the NumPy library for grid-based dungeon representation.
- AI features reinforcement learning, A* Pathfinding, and BFS algorithms.
- Fully customizable, with adjustable grid size and complexity for a tailored experience.
