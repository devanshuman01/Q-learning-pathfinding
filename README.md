# Q-Learning Agent vs. BFS Benchmark 🤖

A practical implementation of the fundamental **Reinforcement Learning** concepts discussed in my research paper, *"Game AI Development using Reinforcement Learning"*.

## 📄 Research Context
This project serves as a code demonstration for **Section 2.1.A (Q-Learning)** of the associated research paper published in IJIRT. While the paper reviews advanced architectures like Deep Q-Networks (DQN) and Actor-Critic methods, this repository focuses on benchmarking the foundational **Tabular Q-Learning** algorithm against classical pathfinding (BFS).

* **Paper:** [Game AI Development using Reinforcement Learning (IJIRT)](https://ijirt.org/publishedpaper/IJIRT181050_PAPER.pdf)
* **Focus:** Implementing the value-based, model-free algorithm described in **Table I** of the paper.

## 🧪 The Experiment
As discussed in the paper's section on **"NPC Decision-Making"**, RL agents can learn complex behaviors over time. This project tests that theory by pitting an RL agent against a mathematically perfect **Breadth-First Search (BFS)** solver.

* **Grid World:** A dynamic 6x6 environment representing a simplified game map.
* **The Agent:** Uses the Bellman Equation to update a Q-Table:
  $$Q(s,a) = Q(s,a) + \alpha [R + \gamma \max Q(s',a') - Q(s,a)]$$
* **The Result:** The agent successfully converged to the optimal path (matching BFS steps) after ~300 episodes, demonstrating the "Trial and Error" learning process described in the abstract.

## 🎥 Visualization
![Agent Demo](demo_agent.gif)
*(The Blue Agent learns to navigate around Black Obstacles to reach the Green Goal)*

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Libraries:** NumPy (Math), Matplotlib (Visualization)
* **Algorithm:** Tabular Q-Learning (Model-Free RL)

## 📂 Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/devanshuman01/Q-learning-pathfinding
