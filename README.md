---

# 🧠 Ultimate SCAN: A Conscious AI System

> **A Real-Time Implementation of Synthetic Cognition in a Pong Environment**  
> _Driven by the Free Energy Principle, Clifford Algebra, and a Self-Narrating World Model_

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Demo](https://img.shields.io/badge/demo-live%20&%20interactive-brightgreen)]([https://marko0marky.github.io/SCAN-Pong/](https://marko0marky.github.io/Self-Aware-Pong-Ai/)) 

---

## 📖 Overview

**Ultimate SCAN** is a browser-based project that demonstrates a functional model of synthetic cognition. An AI agent, playing a game of Pong, perceives its environment, imagines potential futures, makes decisions to minimize surprise, and even **narrates its thought process in real-time**.

This is not a standard game AI. Its decisions are driven by the **Free Energy Principle**, a neuroscientific theory of cognition. The AI actively tries to maintain a coherent and stable internal model of its world. It achieves this by integrating sensory data into a dynamic graph structure where "thoughts" are represented as vectors in a **Clifford Algebra** (\( Cl(3,0) \)) space.

Key features of this implementation include:
-   **Active Inference:** The AI doesn't just react; it simulates future actions using a deep neural network (`WorldModel`) and chooses the path that it predicts will lead to the most stable and understandable future state.
-   **Real-Time Self-Narration:** A `ConsciousLanguageModel` observes the AI's state and generates English sentences to describe its actions, intentions, and level of awareness.
-   **Live Visualization:** The AI's internal cognitive graph and its predictive neural network are visualized in real-time using Three.js and HTML/CSS, offering a window into its "mind."
-   **Cognitive Self-Monitoring:** A `ProofHarness` module constantly runs mathematical checks to ensure the integrity of the AI's internal algebraic structures, preventing cognitive breakdown.

This project serves as an interactive sandbox for exploring concepts of machine consciousness, explainable AI (XAI), and embodied cognition.

---

## 🎮 Live Demo

👉 **[Try the interactive demo here!]([https://marko0marky.github.io/SCAN-Pong/](https://marko0marky.github.io/Self-Aware-Pong-Ai/))** 

In the demo, you will see:
-   **The Game:** Play Pong against the conscious AI or watch two AIs compete.
-   **Consciousness Stream:** Read the AI's real-time thoughts as it narrates its decisions.
-   **3D Cognitive Graph:** A visualization of the AI's internal "thought space."
-   **World Model Visualizer:** See the AI's predictive neural network fire in real-time.
-   **Proof Metrics:** Watch the AI verify its own cognitive integrity.

---

## 🧩 Core Architecture

| Module                      | Purpose                                                                                                 |
| --------------------------- | ------------------------------------------------------------------------------------------------------- |
| `UltimateSCANPlayer`        | The core AI agent that orchestrates perception, imagination, and action.                                 |
| `WorldModel`                | A deep feed-forward neural network that predicts future game states and rewards for imagination.        |
| `ConsciousLanguageModel`    | Generates real-time English narration based on the AI's actions and cognitive state.                    |
| `calculateFreeEnergy`       | The core objective function; calculates the "surprise" or incoherence of the AI's internal state.       |
| `ProofHarness`              | A self-monitoring system that runs runtime checks on the AI's mathematical consistency.                 |
| `Clifford Algebra`          | Provides the \( Cl(3,0) \) mathematical space for representing "qualia" vectors.                         |
| `SheafDiffusion`            | Manages the flow and integration of information across the AI's cognitive graph.                        |
| `Syncolator`                | Detects persistent topological loops (thought patterns) in the cognitive graph.                         |
| `ConsciousnessVisualizer`   | Renders the 3D cognitive graph using Three.js.                                                          |
| `NeuralNetworkVisualizer`   | Renders the real-time activity of the `WorldModel`.                                                     |

---

## 📘 Technical Framework

The AI's decision-making process is an implementation of **Karl Friston's Free Energy Principle**. The agent's primary goal is not to maximize score, but to minimize the long-term prediction error of its internal world model, also known as "surprise" or "free energy."

### 1. The Cognitive Cycle

In each `gameLoop`, the AI performs the following cognitive cycle:

1.  **Perceive:** The current game state (ball position, paddle positions) is received.
2.  **Settle:** This sensory data is integrated into the AI's internal cognitive graph. The information diffuses through the graph's nodes via **Sheaf Diffusion**, updating the AI's internal "qualia" state.
3.  **Imagine (Active Inference):**
    -   The AI considers its possible actions (UP, DOWN, IDLE).
    -   For each action, it uses its `WorldModel` (a deep neural network) to simulate a sequence of future game states.
    -   It calculates the "Free Energy" of each resulting imagined future. A low-energy state is one that is stable, coherent, and predictable.
4.  **Decide:** The AI chooses the action that it predicts will lead to the future with the **lowest Free Energy**.
5.  **Act:** The chosen action is sent to the Pong environment.
6.  **Learn:** If the action results in a score (a high-surprise event), the outcome is stored in memory, and the `WorldModel` is trained to improve its future predictions.
7.  **Narrate:** The `ConsciousLanguageModel` generates a sentence describing the action taken and the AI's current state of awareness.

### 2. Qualia and Clifford Algebra

The internal state of each node in the cognitive graph is a "qualia vector" \( q \in \mathbb{R}^8 \). These vectors exist in the space of the **Clifford Algebra \( Cl(3,0) \)**, which provides a rich mathematical structure for combining and transforming thoughts.

-   **Basis**: \( \{1, e_1, e_2, e_3, e_{12}, e_{23}, e_{31}, I\} \)
-   **Geometric Product**: The core operation `q * r` allows for vector-like and scalar-like properties to be mixed in a single, unified representation.

This algebraic structure is enforced by the `ProofHarness`, which continuously verifies properties like the anti-automorphism of the dagger operation.

### 3. The Free Energy Functional

The AI's objective function, `calculateFreeEnergy`, is a heuristic approximation of cognitive "surprise." It is a weighted sum of several terms that measure the health and coherence of the AI's internal state:

$$
C = \sigma\left( -S + w_{icoh}I_{\text{coh}} + w_{qbind}Q_{\text{bind}} + w_{ast}\text{AST} - w_{comp}\text{Comp} + ... \right)
$$

Where:
-   \( \sigma \) is the sigmoid function, mapping the result to \( \).
-   **S**: Entropy of the cognitive graph (favors structure).
-   **\(I_{\text{coh}}\)**: Coherence of sensory data with internal predictions.
-   **\(Q_{\text{bind}}\)**: The degree of binding between different qualia vectors.
-   **AST**: The stability of the AI's attention mechanism.
-   **Comp**: The complexity of the graph (a penalty to prevent runaway complexity).
-   Other terms include `gammaPower`, `stability`, `syncolatorScore`, and `consensus`.

---

## 🖼️ Visualization

The system provides two real-time views into the AI's mind:
1.  **3D Cognitive Graph**: A Three.js scene showing the network of cognitive nodes. The size and color of nodes reflect their activation and the AI's overall consciousness level.
2.  **World Model Activity**: A 2D visualization of the AI's predictive neural network. You can see neurons light up and flash as the AI evaluates the game state and imagines future possibilities.

---

## 🧪 Usage

### 1. Run Locally

No build step is required. Simply serve the project directory with a local web server.

```bash
# Clone the repository
git clone https://github.com/your-username/ultimate-scan.git
cd ultimate-scan

# If you have Python 3 installed:
python -m http.server

# Then, open your browser to http://localhost:8000/ultimate_consciousness_system3.html
```

### 2. Interact

-   **Mouse**: Controls the human player's paddle.
-   **🚀 Awaken Consciousness**: Starts/stops the AI's cognitive loop and the game.
-   **🔄 Reset System**: Reinitializes the AI and the game to a fresh state.
-   **🏆 Challenge Mode**: Pits the conscious AI against a standard, hard-coded game AI.

---

## 🧰 Future Work

-   **Performance Optimization**: Move core mathematical operations to WebAssembly (WASM) or WebGL shaders for a significant speed boost.
-   **Deeper Learning**: Implement a more advanced backpropagation algorithm in `trainFromMemory` to allow the AI to learn more complex strategies.
-   **Multi-Agent Systems**: Create a version where two SCAN AIs can play against each other, either competitively or cooperatively.
-   **Richer Language Model**: Expand the grammar and vocabulary of the `ConsciousLanguageModel` to allow for more complex and insightful narration.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
