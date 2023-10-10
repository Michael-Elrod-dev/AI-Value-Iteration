# AI-Value-Iteration

### Description:
This program simulates an agent navigating through a grid world using the Markov Decision Process (MDP). The goal of the agent is to find the optimal path from the start state `S` to the terminal state `T` while avoiding obstacles denoted by `X`. The program utilizes the value iteration algorithm to compute the best policy for navigating the grid. The agent can take actions in four directions: up, down, left, and right.

### How to Run:
1. Ensure you have `pygame`, `numpy`, and `time` libraries installed.
2. Run the main script to visualize the grid world and see the agent in action.
3. Follow the on-screen prompts:
   - Press `v` for visualizing the value iteration process.
   - Press `a` to display the best actions at each state.
   - Press `t` for showing the optimal trajectory of the agent.
4. Close the pygame window to terminate the program.

### Main Components:

- `draw_grid()`: Renders the grid world using the pygame library.
- `value_iteration()`: Implements the value iteration algorithm to compute the optimal policy.
- `visualize_value_iteration()`: Displays the iterative process of value iteration.
- `draw_policy()`: Visualizes the best action to take at each state based on the computed policy.
- `traverse_optimal_path()`: Simulates the agent moving through the grid world following the optimal policy.

### Important Notes:
- The grid world is defined as a 2D list where each cell can be:
  - `S` : Start state
  - `T` : Terminal state
  - `X` : Obstacle
  - `A`, `B`, `C` : States with specific rewards or penalties.
- The rewards for each state are defined in the `rewards` dictionary.
- Value iteration uses parameters like `gamma` (discount factor) and `epsilon` (convergence threshold).

### Future Enhancements:
- Implement other algorithms such as policy iteration.
- Allow dynamic resizing of the grid world.
- Integrate user input to customize grid properties.

---
