
 # 🧪 Maze Escape – Save the Scientist

## 🧭 Introduction
A scientist is trapped inside a high-tech research facility after an AI lockdown triggered by a security breach. The facility is structured as a complex grid-based maze filled with traps, high-security doors, and unpredictable hazards. Your mission is to guide the scientist safely to an exit using the **A\* Search Algorithm**.

---

## 🏗️ Environment Representation

The research facility is modeled as a **15 x 15 grid**. Each cell in the grid can represent:

- 🟩 **Empty Cell** – A free space; the scientist can move here (Cost: `1`)
- 🟥 **Wall** – Impassable obstacle
- ⚠️ **Trap Zone** – Hazardous area with **randomized movement cost** between `10-20`
- 🏁 **Exit** – The goal destination
- 🔒 **Lock** – A dead-end door that permanently locks if entered

Each cell connects to its four adjacent neighbors (**up**, **down**, **left**, **right**) unless blocked. The **starting position** of the scientist is predefined at the beginning of the task.

---

## 🧠 Search Algorithm – A\*

### Implementation Features:

- **Algorithm**: A\* Search
- **Heuristics**: 
  - Customizable
  - Suggested: `Manhattan Distance` or `Euclidean Distance`
- **Cost Handling**:
  - Normal Cell: `1`
  - Trap Zone: `Random (10–20)`
  - Dynamic cost updates during traversal
- **Replanning**: If the environment changes mid-path (e.g., a trap appears or a lock is triggered), A\* is recalculated from the current position.

---

## 🔄 Dynamic Maze Handling

Upon the **first successful escape**:
- Slightly **modify** the maze (walls, traps, and locks are randomized)
- Assign a **new random start** and **new random exit**
- Repeat the escape **three times** total, adapting to new layouts each time

This allows testing of the algorithm's adaptability and robustness.

---

## 🧍‍♂️ Path Execution

Once a path is found:
- The scientist follows it **step-by-step**
- If unexpected environmental changes occur, the algorithm **recalculates** the path from the current position

---

## 📊 Performance Evaluation

For each of the three escape tasks, the following metrics will be recorded:

- ✅ **Optimal Path** – The computed path from start to exit
- 🧮 **Total Steps Taken**
- 💰 **Total Path Cost**
- ⏱️ **Time Complexity**
- 💾 **Space Complexity**

---

## 📦 Project Deliverables

1. **Source Code**:
    - Maze generation and modification
    - A\* Search Algorithm with heuristic
    - Simulation of movement with replanning

2. **Performance Report**:
    - Detailed evaluation across all three dynamic mazes

---

## 🛠️ Technologies & Tools (Optional Section)

- Language: _e.g., Python 3.10_
- Libraries: _e.g., NumPy, Matplotlib (for visualization)_
- Runtime Environment: _e.g., Jupyter Notebook or Terminal_

---

## 🚀 OUTPUT

![image](https://github.com/user-attachments/assets/b75690be-8df2-46af-8972-f553d9cb6b22)


