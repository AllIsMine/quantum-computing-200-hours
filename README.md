# Quantum Computing: A 200-Hour Learning Journey

A structured, hands-on learning portfolio documenting my journey into quantum computing through mathematical foundations, quantum circuit programming, algorithm implementation, simulation, testing, and technical documentation.

> **Project goal:** Develop practical quantum-computing skills through focused study, hands-on coding, and reproducible experiments. The 200-hour target represents my learning plan, with progress documented as each milestone is completed.

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Qiskit](https://img.shields.io/badge/Qiskit-Quantum%20SDK-6929C4?logo=ibm&logoColor=white)](https://www.ibm.com/quantum/qiskit)
[![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Learning Plan](https://img.shields.io/badge/Learning%20Plan-200%20Hours-informational)](#learning-roadmap)

## Project Objectives

- Understand quantum states, superposition, measurement, gates, and entanglement.
- Develop quantum circuits using Qiskit and Qiskit Aer.
- Implement introductory quantum algorithms and validate their outputs.
- Connect mathematical concepts with practical quantum programming.
- Maintain reproducible notebooks and clear technical documentation.
- Build a public portfolio demonstrating practical skills and continuous learning.
- Progress toward advanced topics in quantum algorithms, quantum information, and quantum computing.

## Learning Roadmap

| Area | Topics |
|---|---|
| Quantum Foundations | Qubits, state vectors, superposition, measurement, probability |
| Quantum Gates | X, H, Z, phase gates, controlled operations |
| Entanglement | Bell states, GHZ states, quantum correlations |
| Quantum Algorithms | Deutsch–Jozsa, Bernstein–Vazirani, Grover's search, Simon's algorithm |
| Fourier and Phase Algorithms | Quantum Fourier Transform (QFT), inverse QFT, Quantum Phase Estimation (QPE) |
| Practical Programming | Qiskit circuits, simulation, measurement counts, assertions, debugging |
| Transpilation and Optimization | Optimization levels, circuit depth, gate counts, routing, qubit layouts, basis-gate decomposition |
| Quantum Hardware | Future experiments on IBM Quantum hardware and hardware-aware circuits |
| Noise and Reliability | Quantum noise, circuit limitations, introductory error mitigation |
| Portfolio Development | Jupyter notebooks, experiment summaries, Git, GitHub, technical writing |

## Progress Tracker

| Milestone | Status | Notebook and Documentation |
|---|---|---|
| Day 1 — Quantum Computing Foundations | Complete | [Notebook](day-01/Day01_Quantum_Computing_Foundations.ipynb) · [README](day-01/README.md) |
| Day 2 — Single-Qubit Gates | Complete | [Notebook](day-02/Day02_Single_Qubit_Gates.ipynb) · [README](day-02/README.md) |
| Day 3 — Entanglement and Bell States | Complete | [Notebook](day-03/Day03_Entanglement_Bell_States.ipynb) · [README](day-03/README.md) |
| Day 4 — Deutsch–Jozsa and Bernstein–Vazirani | Practical exercises complete | [Notebook](day-04/Day04_DJ_and_Bernstein_Vazirani.ipynb) · [README](day-04/README.md) |
| Day 5 — Grover's Algorithm and Quantum Search | Experiments complete | [Notebook](day-05/Day05_Grovers_Algorithm_Quantum_Search.ipynb) · [README](day-05/README.md) |
| Day 6 — Quantum Fourier Transform and Quantum Phase Estimation | Complete — ideal simulator checks passed | [Notebook](day-06/Day06_Quantum_Fourier_Transform.ipynb) · [README](day-06/README.md) |
| Day 7 — Simon's Algorithm | Complete | [Notebook](day-07/Day07_Simons_Algorithm.ipynb) · [README](day-07/README.md) |
| Day 8 — Advanced Quantum Phase Estimation (QPE) | Complete — precision experiments, exact-phase validation, and ideal/noisy simulation comparison | [Notebook](day-08/day08_Advanced_Quantum_Phase_Estimation.ipynb) · [README](day-08/README.md) |
| Day 9 — Transpilation and Backend Optimization | Complete — routing, optimization comparison, basis-gate decomposition, and layout-aware equivalence checks verified | [Notebook](day-09/Day09_Transpilation_Backend_Optimization.ipynb) · [README](day-09/README.md) |

## Day 1 — Quantum Computing Foundations

**Status: Complete**

Introduced the fundamental concepts of quantum computing and began implementing quantum circuits.

### Topics Covered

- Qubits and quantum states
- Superposition and measurement
- Basic circuit construction
- Running quantum circuits in a notebook environment

See the [Day 1 notebook](day-01/Day01_Quantum_Computing_Foundations.ipynb) and [Day 1 README](day-01/README.md).

## Day 2 — Single-Qubit Gates

**Status: Complete**

Explored single-qubit operations and their effects on quantum states.

### Topics Covered

- Quantum gate operations
- Hadamard transformations
- State changes and measurement
- Circuit construction and simulation

See the [Day 2 notebook](day-02/Day02_Single_Qubit_Gates.ipynb) and [Day 2 README](day-02/README.md).

## Day 3 — Entanglement and Bell States

**Status: Complete**

Studied entanglement and created circuits that demonstrate correlations between qubits.

### Topics Covered

- Bell-state preparation
- Multi-qubit circuits
- Entanglement and measurement
- GHZ-state concepts and related experiments

See the [Day 3 notebook](day-03/Day03_Entanglement_Bell_States.ipynb) and [Day 3 README](day-03/README.md).

## Day 4 — Deutsch–Jozsa and Bernstein–Vazirani

**Status: Practical exercises complete**

Implemented introductory quantum algorithms to investigate how quantum circuits can reveal properties of functions and recover hidden bit strings.

### Recorded Simulator Results

| Exercise | Observed Result |
|---|---|
| Deutsch–Jozsa: constant-zero oracle | `000` |
| Deutsch–Jozsa: constant-one oracle | `000` |
| Deutsch–Jozsa: balanced oracle | `001` |
| Bernstein–Vazirani: secret string `101` | `101` |

These results came from ideal Qiskit Aer simulation, not physical quantum hardware.

See the [Day 4 notebook](day-04/Day04_DJ_and_Bernstein_Vazirani.ipynb) and [Day 4 README](day-04/README.md).

## Day 5 — Grover's Algorithm and Quantum Search

**Status: Experiments complete**

Implemented a two-qubit example of Grover's search algorithm using Qiskit and Qiskit Aer.

Two target states were tested by modifying the oracle while retaining the diffusion operation.

### Recorded Simulator Results

| Experiment | Target State | Recorded Result |
|---|---|---|
| Experiment 1 | `11` | `{'11': 1000}` |
| Experiment 2 | `10` | `{'10': 1000}` |

Each experiment used 1,000 simulator shots, and the corresponding assertion passed.

### Topics Practiced

- Oracle construction
- Grover diffusion
- Amplitude amplification
- Measurement outcomes
- Qubit indexing and displayed bit ordering
- Debugging and validating circuit behavior

These results came from ideal simulation. This small demonstration illustrates Grover's algorithm but does not establish a practical speed advantage for large search problems.

See the [Day 5 notebook](day-05/Day05_Grovers_Algorithm_Quantum_Search.ipynb) and [Day 5 README](day-05/README.md).

## Day 6 — Quantum Fourier Transform and Quantum Phase Estimation

**Status: Complete — QFT, inverse QFT, and QPE validated in ideal simulation**

Day 6 focused on quantum phase, controlled-phase operations, the Quantum Fourier Transform, its inverse, and Quantum Phase Estimation.

### Experiments Completed

- Constructed a two-qubit QFT circuit.
- Compared the implemented QFT against the mathematical Fourier-transform unitary.
- Verified the inverse QFT.
- Tested recovery of all four computational basis states.
- Implemented and simulated a QPE circuit.
- Investigated measurement results and the relationship between phase and binary representation.

### Validation Results

| Test | Result |
|---|---|
| QFT matches mathematical unitary | `True` |
| QFT followed by inverse QFT returns identity | `True` |
| Recovery of `00`, `01`, `10`, and `11` | All passed |
| Selected QPE phase | `0.25 = 0.01₂` |
| QPE measurement counts | `{'01': 1024}` |
| Shots matching expected outcome | 1,024 out of 1,024 |

The QPE circuit used two counting qubits and one eigenstate qubit. In the ideal Qiskit Aer simulation, all 1,024 shots returned `01`, matching the selected phase of 0.25.

These results were obtained using an ideal simulator, not physical quantum hardware. Real hardware can produce different distributions because of noise and device limitations.

See the [Day 6 notebook](day-06/Day06_Quantum_Fourier_Transform.ipynb) and [Day 6 README](day-06/README.md).

## Day 7 — Simon's Algorithm

**Status: Complete — classical promise, oracle, and hidden-string recovery verified in simulation**

Implemented Simon's algorithm for the hidden string `110` using Qiskit and Qiskit Aer.

### Experiments Completed

- Verified the classical Simon promise.
- Constructed and tested the quantum oracle.
- Built and simulated the complete quantum circuit.
- Checked measurement results against the expected parity condition.
- Recovered the hidden string `110` from the measured equations.

### Results

- Oracle test: Passed.
- Simulator shots: 1,024.
- Parity verification: Passed for all observed outcomes.
- Hidden-string recovery: `110`.

These results were obtained in ideal simulation, not on physical quantum hardware.

See the [Day 7 notebook](day-07/Day07_Simons_Algorithm.ipynb) and [Day 7 README](day-07/README.md).

## Day 8 — Advanced Quantum Phase Estimation (QPE)

**Status: Complete — precision experiments, exact-phase validation, and ideal/noisy simulation comparison completed**

Extended Quantum Phase Estimation using Qiskit and Qiskit Aer to investigate phase-estimation precision and the effects of simulated noise.

### Experiments Completed

- Ran precision experiments using 2, 3, 4, and 5 counting qubits.
- Compared phase-grid spacing, modal estimates, sample means, and sampling spread.
- Ran exact-phase regression tests for five phase values.
- Evaluated a four-counting-qubit experiment using the target phase `0.30`.
- Compared ideal and illustrative noisy simulation results using 8,192 shots per run.

### Key Results

For the target phase `0.30`, the four-counting-qubit experiment produced:

- **Modal bitstring:** `0101`
- **Estimated phase:** `0.3125`
- **Absolute phase error:** `0.0125`

### Ideal-versus-Noisy Simulation Comparison

| Metric | Ideal Simulation | Noisy Simulation |
|---|---:|---:|
| Modal bitstring | `0101` | `0101` |
| Modal outcome frequency | 87.56% | 65.38% |
| Estimated phase from sample mean | 0.31264 | 0.33760 |
| Sample standard deviation | 0.05957 | 0.15620 |

The results illustrate how noise can broaden measurement distributions and affect phase estimates.

### Noise and Reproducibility

The ideal and noisy experiments were run in simulation. The noisy simulation used an illustrative noise model, including depolarizing and readout errors. These results are not measurements from real quantum hardware and do not represent a calibrated device noise model.

The notebook records the software versions used. Refer to its simulation setup cells for the exact noise-model parameters.

See the [Day 8 notebook](day-08/day08_Advanced_Quantum_Phase_Estimation.ipynb) and [Day 8 README](day-08/README.md).

## Day 9 — Transpilation and Backend Optimization

**Status: Complete**

Explored how Qiskit adapts quantum circuits to optimization settings, hardware connectivity constraints, and a specified gate basis.

### Environment

- Qiskit version: `2.6.0`
- Platform: Google Colab
- Circuit: Three-qubit example
- Connectivity model: Educational linear three-qubit coupling map

### Experiments Completed

- Built a three-qubit circuit and measured gate count and circuit depth.
- Compared optimization levels 0, 1, 2, and 3.
- Created an educational linear coupling map connecting neighboring qubits.
- Routed the circuit and observed one inserted SWAP gate.
- Measured routing overhead.
- Compared routed circuits at optimization levels 0 and 3.
- Inspected initial and final qubit layouts.
- Transpiled to the specified basis gates `rz`, `sx`, `x`, and `cx`.

### Results

| Experiment | Gate Count | Circuit Depth | SWAP Gates |
|---|---:|---:|---:|
| Original circuit | 5 | 4 | 0 |
| Routed, optimization level 0 | 6 | 5 | 1 |
| Routed, optimization level 3 | 6 | 5 | 1 |
| Specified basis-gate circuit | 12 | 9 | 0 native SWAP gates reported |

The basis-gate circuit contained 5 `rz` gates, 2 `sx` gates, and 5 `cx` gates.

Routing increased the gate count from 5 to 6, a 20% increase, and circuit depth from 4 to 5, a 25% increase.

### Validation Results

- Routed circuit: layout-aware equivalence check returned `True`.
- Optimization level 0: layout-aware equivalence check returned `True`.
- Optimization level 3: layout-aware equivalence check returned `True`.
- Basis-gate circuit: layout-aware equivalence check returned `True`.

### Key Findings

- Higher optimization levels do not guarantee fewer gates or lower circuit depth.
- Routing can add operations to satisfy connectivity constraints.
- Basis-gate decomposition can increase circuit size and depth.
- Qubit layouts can change during transpilation.
- Raw operator comparisons can be misleading when qubit layouts differ.
- Layout-aware verification is important when checking transformed circuits.

The connectivity map used here is an educational model, not a representation of a specific real quantum backend. These experiments used circuit transpilation and operator verification, not physical quantum hardware.

See the [Day 9 notebook](day-09/Day09_Transpilation_Backend_Optimization.ipynb) and [Day 9 README](day-09/README.md).

## Tools and Technologies

- **Language:** Python
- **Quantum SDK:** Qiskit
- **Simulator:** Qiskit Aer
- **Numerical computing:** NumPy
- **Notebook environment:** Google Colab / Jupyter Notebook
- **Version control:** Git and GitHub

## Repository Structure

```text
quantum-computing-200-hours/
├── README.md
├── day-01/
│   ├── Day01_Quantum_Computing_Foundations.ipynb
│   └── README.md
├── day-02/
│   ├── Day02_Single_Qubit_Gates.ipynb
│   └── README.md
├── day-03/
│   ├── Day03_Entanglement_Bell_States.ipynb
│   └── README.md
├── day-04/
│   ├── Day04_DJ_and_Bernstein_Vazirani.ipynb
│   └── README.md
├── day-05/
│   ├── Day05_Grovers_Algorithm_Quantum_Search.ipynb
│   └── README.md
├── day-06/
│   ├── Day06_Quantum_Fourier_Transform.ipynb
│   └── README.md
├── day-07/
│   ├── Day07_Simons_Algorithm.ipynb
│   └── README.md
├── day-08/
│   ├── day08_Advanced_Quantum_Phase_Estimation.ipynb
│   └── README.md
└── day-09/
    ├── Day09_Transpilation_Backend_Optimization.ipynb
    └── README.md
```

## Project Workflow

Each milestone follows a consistent workflow:

1. Study the underlying concept and mathematics.
2. Implement the quantum circuit in a notebook.
3. Execute the circuit and inspect the results.
4. Validate behavior with assertions or mathematical checks where appropriate.
5. Document the outcome, assumptions, and limitations.
6. Publish the notebook and a concise README.

## Next Steps

Days 1–9 are documented in the progress tracker. The next learning milestone will follow the existing **Quantum Computing Mastery** roadmap rather than introducing a replacement sequence.

Future work may include:

- Continuing the next scheduled roadmap milestone.
- Deepening practical Qiskit programming skills.
- Running suitable experiments on real quantum hardware when available.
- Exploring quantum noise and introductory error mitigation.
- Improving the portfolio with reproducible tests and technical explanations.

These are potential future activities, not claims of completed work. The next specific task should be selected from the established learning roadmap.

## About This Portfolio

This repository documents a hands-on learning journey from quantum-computing foundations to quantum algorithms, phase estimation, and circuit transpilation. It emphasizes practical programming, mathematical validation, transparent reporting, and continuous improvement.

The progress tracker distinguishes completed work from planned milestones and identifies simulator results separately from physical quantum hardware experiments.
