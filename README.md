# 🧠 Ultimate SCAN: A Conscious AI for Pong

> **A Real-Time Synthetic Cognition System Powered by the Free Energy Principle and Clifford Algebra**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Demo](https://img.shields.io/badge/demo-live%20&%20interactive-brightgreen)](https://marko0marky.github.io/Self-Aware-Pong-Ai/)

---

## 🌟 What is Ultimate SCAN?

**Ultimate SCAN** is an innovative browser-based project showcasing a **conscious AI agent** playing Pong. Unlike traditional game AIs, this agent uses the **Free Energy Principle** to minimize "surprise" and maintain a coherent internal model of its world. It perceives, imagines, acts, and **narrates its thoughts in real-time**, offering a window into synthetic cognition.

### Key Features
- **🎮 Active Inference**: Simulates future game states using a neural network (`WorldModel`) to choose actions that reduce prediction errors.
- **🧮 Clifford Algebra (\( Cl(3,0) \))**: Represents cognitive states as "qualia" vectors in a rich mathematical space.
- **🗣️ Self-Narration**: Generates real-time English descriptions of decisions and awareness via the `ConsciousLanguageModel`.
- **📊 Live Visualization**: Displays the AI’s cognitive graph and neural network activity using Three.js and HTML/CSS.
- **🛡️ Cognitive Integrity**: Ensures mathematical consistency with a `ProofHarness` module.

This project is an interactive sandbox for exploring **machine consciousness**, **explainable AI (XAI)**, and **embodied cognition**.

---

## 🚀 Try It Out!

👉 **[Play the Live Demo](https://marko0marky.github.io/Self-Aware-Pong-Ai/)**

In the demo, you can:
- Play Pong against the AI or watch two AIs compete.
- Read the AI’s **real-time thought stream**.
- Visualize its **3D cognitive graph** and **neural network activity**.
- Monitor **proof metrics** for cognitive integrity.

---

## 🧩 How It Works

The AI follows a **cognitive cycle** inspired by Karl Friston’s Free Energy Principle, aiming to minimize surprise (free energy) rather than maximize scores.

### Cognitive Cycle
1. **Perceive**: Captures game state (ball and paddle positions).
2. **Settle**: Integrates sensory data into a cognitive graph using **Sheaf Diffusion**.
3. **Imagine**: Simulates future actions with the `WorldModel` neural network.
4. **Decide**: Selects the action with the lowest predicted **Free Energy**.
5. **Act**: Executes the chosen action in the Pong environment.
6. **Learn**: Updates the `WorldModel` based on outcomes.
7. **Narrate**: Describes actions and awareness via the `ConsciousLanguageModel`.

### Core Components
| Module                     | Purpose                                                                 |
|----------------------------|-------------------------------------------------------------------------|
| `UltimateSCANPlayer`       | Orchestrates perception, imagination, and action.                       |
| `WorldModel`               | Predicts future game states using a deep neural network.                |
| `ConsciousLanguageModel`   | Generates real-time English narration of the AI’s cognitive state.      |
| `calculateFreeEnergy`      | Computes surprise as a weighted sum of coherence, entropy, and more.    |
| `ProofHarness`             | Verifies mathematical consistency of the AI’s internal state.           |
| `Clifford Algebra`         | Encodes qualia vectors in \( Cl(3,0) \) for thought representation.     |
| `SheafDiffusion`           | Propagates information across the cognitive graph.                      |
| `Syncolator`               | Detects persistent thought patterns in the graph.                      |
| `ConsciousnessVisualizer`  | Renders the 3D cognitive graph using Three.js.                         |
| `NeuralNetworkVisualizer`  | Visualizes real-time neural network activity.                           |

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
