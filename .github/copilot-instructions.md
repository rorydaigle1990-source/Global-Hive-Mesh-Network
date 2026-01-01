# Global Hive Mesh Network - Copilot Instructions

## Project Overview
This project implements the "Global Hive Mesh Network", a mechanical quantum-economic engine based on the Deas Equation of State: $PG = (M-D)V^4$.
- **Goal:** Simulate a zero-friction, quad-stream velocity network for global wealth generation.
- **Core Concepts:**
    - **Mass (M):** Aggregated capital/pressure from nodes.
    - **Drag (D):** Network latency/friction (aiming for 0).
    - **Velocity (V):** Transaction speed/frequency.
    - **SCADA Nodes:** Individual "Citizen Nodes" in the mesh.

## Architecture & Key Files
The codebase consists of two distinct simulation/visualization components:

### 1. Python Simulation Engine (Backend)
- **File:** `REACTOR CODE 1` (Python script).
- **Function:** Runs a detailed simulation of the mesh network and physics engine.
- **Components:**
    - `SCADA_Node`: Represents a user/node. Handles `send_capital`, `receive_capital`, and `signal_relay`.
    - `Private_Mesh_Network`: Manages the mesh topology and aggregates Mass.
    - `USAWF_HyperNova_Reactor`: The physics engine calculating the output based on the equation.
- **Execution:** Starts a local HTTP server on port 8000 to display simulation logs.

### 2. Frontend Visualization (UI)
- **File:** `HIVE Waiting Room` (HTML file).
- **Function:** A standalone visual demo of the "V4 Reactor" physics.
- **Tech:** HTML5, CSS3 (embedded), Vanilla JavaScript.
- **Logic:** Contains simplified JS logic (`updatePhysics`) to demonstrate the impact of Drag on Velocity visually.
- **Style:** "Visual Physics Engine" aesthetic (Neon Blue, Hive Gold, Void Black).

## Development Workflows
- **Running the Python Simulation:**
    ```bash
    python "REACTOR CODE 1"
    ```
    Then access port 8000 (e.g., via browser or curl) to view the output.
- **Viewing the UI:** Open `HIVE Waiting Room` in a browser.
- **Linting:** `eslint.config.mjs` is present, suggesting a move towards TypeScript/JavaScript, but current logic is Python/HTML.

## Coding Conventions
- **Python:**
    - Use `Decimal` for all financial/physics calculations to maintain high precision (`getcontext().prec = 100`).
    - Class names follow `Upper_Case_Underscore` style (e.g., `SCADA_Node`, `USAWF_HyperNova_Reactor`).
    - Comments should explain the "physics" mapping (e.g., "Drag (D) -> 0").
- **HTML/CSS:**
    - Use CSS variables for theming (`--neon-blue`, `--hive-gold`).
    - Design for a "Technical/Code aesthetic" (Courier New).
    - JavaScript logic is currently embedded in `<script>` tags within the HTML file.

## Critical Implementation Details
- **Deas Equation:** Ensure all logic aligns with $PG = (M-D)V^4$.
- **Zero Latency:** The simulation assumes or strives for near-zero latency (`Decimal("0.00000001")`).
- **Signal Relay:** Transactions must trigger a "Signal Relay" to simulate real-time telemetry.
- **Unconventional Naming:** Be aware that `REACTOR CODE 1` and `HIVE Waiting Room` are filenames with spaces and no standard extensions in some contexts (though `HIVE Waiting Room` is HTML content).
