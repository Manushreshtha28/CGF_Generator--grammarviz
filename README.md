# Grammarviz — CFG Derivation Engine

**Grammarviz** (internally powered by the **CFGviz** engine) is a high-fidelity, interactive educational tool for visualizing Context-Free Grammar (CFG) derivations and parse trees. Designed with a "Blueprint Brutalist" aesthetic, it serves as a comprehensive diagnostic and learning aid for Formal Languages and Automata Theory.

**Live Demo:** [https://cgf-2.vercel.app](https://cgf-2.vercel.app)

---

## 🖋️ Author
**Manu Shreshtha Yadav** ID: 2024UCS1638  
Computer Science & Engineering

---

## 🛠️ Features

### 1. Multi-Mode Derivation Engine
The core engine uses a Breadth-First Search (BFS) approach to determine valid derivation paths for any input string.
* **Leftmost Derivation:** Systematically expands the leftmost non-terminal.
* **Rightmost Derivation:** Systematically expands the rightmost non-terminal.
* **Simultaneous View:** Users can toggle a "Both" mode to compare different derivation structures side-by-side.

### 2. Interactive Parse Tree
Generates dynamic, zoomable SVG parse trees that represent the hierarchy of the derivation.
* **Visual Distinction:** Clearly separates Non-Terminals (Blue) from Terminals (Green).
* **Vector Export:** Supports high-quality SVG export for academic reports.
* **Auto-Layout:** Algorithmic node positioning ensures clarity even for complex grammars.

### 3. Live Playback Animation
Includes a dedicated "Animation Stage" to watch the derivation process unfold step-by-step.
* **Playback Control:** Adjustable speeds including Slow, Normal, and Fast.
* **Step Logic:** Highlights specific production rules as they are applied.
* **Success Indicators:** Features a visual "Accept" effect when a string is successfully derived.

### 4. Grammar Analysis & Statistics
Provides a detailed diagnostic suite for the input grammar:
* **Symbol Extraction:** Automatically identifies the sets of Terminals ($\Sigma$) and Non-Terminals ($N$).
* **Form Detection:** Validates if the grammar follows Chomsky Normal Form (CNF).
* **Redundancy Checks:** Flags unreachable symbols, $\epsilon$-productions, and unit productions.

---

## 🚀 Usage Guide

1.  **Define Grammar:** Enter your start symbol and rules using the `A → BC | d` syntax in the sidebar.
2.  **Input String:** Enter the target string (use `ε` for the empty string).
3.  **Run:** Click **RUN DERIVATION** to compute the results.
4.  **Explore:** Use the tabs to switch between **Derivation Steps**, **Parse Tree**, and **Live Animation**.

---

## 💻 Tech Stack

* **Logic:** Vanilla JavaScript (ES6+) utilizing a custom BFS-based CFG engine (CFGviz).
* **Styling:** CSS3 featuring a graph-paper grid, IBM Plex Mono typography, and a "Blueprint" theme.
* **Visuals:** Dynamic SVG generation for hierarchical trees.
* **Deployment:** Vercel.

---

## 📜 License
This project is developed for educational purposes. Feel free to use and modify the engine for learning Automata Theory.

