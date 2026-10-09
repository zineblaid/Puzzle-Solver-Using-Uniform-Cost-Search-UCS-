# 8-Puzzle Solver Using Uniform Cost Search (UCS)

##  Project Overview

This project implements the **Uniform Cost Search (UCS)** algorithm in Python to solve the 8-puzzle problem.

The 8-puzzle consists of a 3×3 grid containing eight numbered tiles and one empty cell, represented by `0`. The objective is to transform the initial state into the goal state while minimizing the total movement cost.

Unlike algorithms that minimize the number of moves, UCS finds the solution with the lowest cumulative cost when all action costs are non-negative.

##  Objectives

- Understand the Uniform Cost Search algorithm.
- Represent puzzle configurations as states.
- Generate valid successor states.
- Manage states using a priority queue.
- Calculate the cumulative cost of each path.
- Find the minimum-cost path from the initial state to the goal state.

##  Initial and Goal States

**Initial State:**

```text
2  8  3
1  6  4
7  0  5
```

**Goal State:**

```text
1  2  3
8  0  4
7  6  5
```

The empty cell (`0`) moves up, down, left, or right, depending on its position in the grid.

##  Movement Costs

Each movement has a specific cost:

| Action | Cost |
|---|---:|
| UP | 9 |
| DOWN | 2 |
| LEFT | 4 |
| RIGHT | 3 |

The total path cost is calculated by adding the costs of all movements.

##  Algorithm

The UCS algorithm follows these steps:

1. Initialize the priority queue with the initial state and a cost of zero.
2. Extract the state with the lowest cumulative cost.
3. Check whether the state is the goal state.
4. Generate all valid successor states.
5. Calculate the new cumulative cost for each successor.
6. Update the best known cost and parent information when a cheaper path is found.
7. Repeat until the goal state is reached or no states remain to explore.
8. Reconstruct the solution path and display the actions and total cost.

##  Technologies Used

- **Programming Language:** Python
- **Library:** `heapq` for priority queue management
- **Concepts:** Artificial Intelligence, State-Space Search, Uniform Cost Search, Path Cost Optimization

##  How to Run

### Requirements

- Python 3.x

The `heapq` module is included in the Python standard library, so no additional package installation is required.

### Execution

1. Clone this repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/8-puzzle-ucs.git
   ```

2. Navigate to the project directory:

   ```bash
   cd 8-puzzle-ucs
   ```

3. Run the Python program:

   ```bash
   python main.py
   ```

##  Output

The program displays:

- The sequence of actions required to reach the goal.
- The cost associated with each action.
- The total cost of the solution path.

##  Key Concepts Learned

- Uniform Cost Search (UCS)
- Priority queues
- State-space representation
- Successor generation
- Parent tracking and path reconstruction
- Cumulative path cost
- Optimal search strategies

##  Author


OULED LAID ZINEB
Software Engineering Student

## 📄 License

This project is available for educational and learning purposes.
