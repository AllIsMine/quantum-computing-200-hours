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
| Day 8 | Quantum Phase Estimation (QPE) | ⏳ In Progress |

## Day 1 — Quantum Computing Foundations

**Status: Complete**

Introduced the fundamental concepts of quantum computing and began implementing quantum circuits.

Topics include:
- Qubits and quantum states
- Superposition and measurement
- Basic circuit construction
- Running quantum circuits in a notebook environment

See the [Day 1 notebook](day-01/Day01_Quantum_Computing_Foundations.ipynb).

## Day 2 — Single-Qubit Gates

**Status: Complete**

Explored single-qubit operations and their effects on quantum states.

Topics include:
- Quantum gate operations
- Hadamard transformations
- State changes and measurement
- Circuit construction and simulation

See the [Day 2 notebook](day-02/Day02_Single_Qubit_Gates.ipynb).

## Day 3 — Entanglement and Bell States

**Status: Complete**

Studied entanglement and created circuits that demonstrate correlations between qubits.

Topics include:
- Bell-state preparation
- Multi-qubit circuits
- Entanglement and measurement
- GHZ-state concepts and related experiments

See the [Day 3 notebook](day-03/Day03_Entanglement_Bell_States.ipynb).

## Day 4 — Deutsch–Jozsa and Bernstein–Vazirani

**Status: Practical exercises complete**

Implemented introductory quantum algorithms to investigate how quantum circuits can reveal properties of functions and recover hidden bit strings.

Recorded ideal Qiskit Aer simulator results:

| Exercise | Observed Result |
|---|---|
| Deutsch–Jozsa: constant-zero oracle | `000` |
| Deutsch–Jozsa: constant-one oracle | `000` |
| Deutsch–Jozsa: balanced oracle | `001` |
| Bernstein–Vazirani: secret string `101` | `101` |

These results came from ideal simulation, not physical quantum hardware.

See the [Day 4 notebook](day-04/Day04_DJ_and_Bernstein_Vazirani.ipynb) and [Day 4 README](day-04/README.md).

## Day 5 — Grover's Algorithm and Quantum Search

**Status: Experiments complete**

Implemented a two-qubit example of Grover's search algorithm using Qiskit and Qiskit Aer.

Two target states were tested by modifying the oracle while retaining the diffusion operation.

| Experiment | Target State | Recorded Simulator Result |
|---|---|---|
| Experiment 1 | `11` | `{'11': 1000}` |
| Experiment 2 | `10` | `{'10': 1000}` |

Each experiment used 1,000 simulator shots, and the corresponding assertion passed.

The experiments provided practice with:
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
└── day-06/
    ├── Day06_Quantum_Fourier_Transform.ipynb
    └── README.md
└── day-07/
    ├── Day07_Simons_Algorithm.ipynb
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

The next planned milestone is Simon's algorithm, followed by further quantum-algorithm practice and deeper study of quantum information.

Future milestones may include:
- Simon's algorithm and hidden-bit-string recovery
- More advanced quantum algorithms
- Qiskit transpilation and circuit optimization
- Running suitable experiments on real quantum hardware
- Exploring noise and introductory error mitigation
- Improving the portfolio with reproducible tests and technical explanations

These are planned topics, not claims of completed work.

## About This Portfolio

This repository documents a hands-on learning journey from quantum-computing foundations to quantum algorithms and phase estimation. It emphasizes practical programming, mathematical validation, transparent reporting, and continuous improvement.

The progress tracker distinguishes completed work from planned milestones and identifies ideal simulator results separately from physical quantum hardware experiments.
