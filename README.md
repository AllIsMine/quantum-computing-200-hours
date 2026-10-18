# Quantum Computing: A 200-Hour Learning Journey

A structured, hands-on portfolio documenting my progress in quantum computing through mathematical foundations, quantum circuit programming, algorithm implementation, simulation, testing, and technical documentation.

> **Project goal:** Build practical quantum-computing skills through focused study and reproducible coding exercises. This repository records progress as it is completed; it does not imply that the full 200 hours have already been completed.

[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Qiskit](https://img.shields.io/badge/Qiskit-Quantum%20SDK-6929C4?logo=ibm&logoColor=white)](https://www.ibm.com/quantum/qiskit)
[![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Learning sprint](https://img.shields.io/badge/Plan-200%20hours-informational)](#project-approach)

## Project Objectives

- Develop a solid understanding of quantum states, gates, measurement, and entanglement.
- Build and simulate quantum circuits using Qiskit and Qiskit Aer.
- Implement introductory quantum algorithms and validate their outputs.
- Maintain readable, reproducible notebooks with clear technical explanations.
- Develop a public portfolio demonstrating practical implementation and conceptual understanding.

## Learning Roadmap

| Area | Topics |
|---|---|
| Quantum Foundations | Qubits, state vectors, superposition, measurement |
| Quantum Gates | X, H, Z, phase gates, controlled operations |
| Entanglement | Bell states, GHZ states, quantum correlations |
| Quantum Algorithms | Deutsch–Jozsa, Bernstein–Vazirani, Grover's search |
| Practical Programming | Qiskit circuits, simulation, measurement counts, assertions |
| Portfolio Development | Jupyter notebooks, experiment summaries, version control |

## Progress Tracker

| Milestone | Status | Evidence |
|---|---|---|
| [Day 1 — Foundations and Quantum Circuits](day-01/Day01_Quantum_Computing_Foundations.ipynb) | Complete | Notebook published |
| [Day 2 — Single-Qubit Gates](day-02/Day02_Single_Qubit_Gates.ipynb) | Complete | Notebook published |
| [Day 3 — Entanglement and Bell States](day-03/Day03_Entanglement_Bell_States.ipynb) | Complete | Notebook and README published |
| [Day 4 — Deutsch–Jozsa and Bernstein–Vazirani](Day-04/Day04_DJ_and_Bernstein_Vazirani.ipynb) | Practical exercises complete | Notebook and README published |
| [Day 5 — Grover's Algorithm and Quantum Search](Day-05/Day05_Grovers_Algorithm_Quantum_Search.ipynb) | Experiments complete | Notebook and README published |
| [Day 6 — QFT and QPE](day-06/Day06_Quantum_Fourier_Transform.ipynb) | Complete | [Notebook](day-06/Day06_Quantum_Fourier_Transform.ipynb) · [README](day-06/README.md) |

## Day 4 — Recorded Simulator Results

The completed exercises recorded the following results using the ideal Qiskit Aer simulator, with 1,000 shots per exercise.

| Exercise | Observed Result |
|---|---|
| Deutsch–Jozsa: constant-zero oracle | `000` |
| Deutsch–Jozsa: constant-one oracle | `000` |
| Deutsch–Jozsa: balanced oracle | `001` |
| Bernstein–Vazirani: secret string `101` | `101` |

These are ideal simulator results, not measurements from real quantum hardware.

## Day 5 — Grover's Algorithm and Quantum Search

**Status: Experiments complete; ideal simulator validation recorded.**

The Day 5 notebook implements a two-qubit example of Grover's search algorithm using Qiskit and Qiskit Aer. Two target states were tested by modifying the oracle while retaining the diffusion operation.

| Experiment | Target State | Simulator Result |
|---|---|---|
| Experiment 1 | `11` | `{'11': 1000}` |
| Experiment 2 | `10` | `{'10': 1000}` |

Each experiment used 1,000 simulator shots, and the corresponding assertion passed.

The second experiment also provided practical debugging experience with Qiskit qubit indexing and displayed measurement-bit ordering.

These results are from ideal simulation, not real quantum hardware. This small example demonstrates the basic mechanism of Grover's algorithm; it does not establish a practical speed advantage for large search problems.

See the [Day 5 README](Day-05/README.md) for the methodology, results, interpretation, and limitations.

## Tools and Environment

- Python
- Qiskit
- Qiskit Aer
- Jupyter Notebook / Google Colab
- Git and GitHub

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
├── Day-04/
│   ├── Day04_DJ_and_Bernstein_Vazirani.ipynb
│   └── README.md
├── Day-05/
│   ├── Day05_Grovers_Algorithm_Quantum_Search.ipynb
│   └── README.md
└── day-06/
    ├── Day06_Quantum_Fourier_Transform.ipynb
    └── README.md
```

## Project Workflow

Each milestone follows a consistent workflow:

1. Understand the concept and its mathematical meaning.
2. Implement the circuit in a notebook.
3. Execute the notebook and inspect the results.
4. Add meaningful checks where appropriate.
5. Explain the outcome, assumptions, and limitations.
6. Publish the notebook and a concise README.

## About This Portfolio

This repository documents a practical learning journey in quantum computing, progressing from foundational concepts to quantum algorithms and increasingly advanced experiments. Completed milestones, simulator results, and hardware experiments are identified accurately so readers can distinguish verified work from planned work.
