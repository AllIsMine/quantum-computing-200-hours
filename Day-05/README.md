# Day 5 — Grover's Algorithm and Quantum Search

## Overview

This practical exercise implements a two-qubit example of Grover's quantum search algorithm using Qiskit and Qiskit Aer.

The circuit searches for the target computational basis state `11`. It demonstrates how an oracle marks a target state and how a diffusion operation amplifies its amplitude.

## Learning Objectives

- Understand the purpose of a quantum search algorithm.
- Prepare an equal superposition of two qubits.
- Implement a phase oracle using a controlled-Z gate.
- Construct the diffusion operation.
- Measure the circuit using Qiskit Aer.
- Validate the observed result with a simple assertion.

## Algorithm Workflow

1. **Superposition:** Apply Hadamard gates to both qubits to prepare four equally weighted basis states.
2. **Oracle:** Apply a controlled-Z gate to mark the target state `11` through a phase change.
3. **Diffusion:** Apply the diffusion operation to amplify the target state's amplitude.
4. **Measurement:** Measure both qubits and inspect the output counts.
5. **Validation:** Check that the ideal simulator returns the expected target state.

## Implementation

The notebook is named `Day05_Grovers_Algorithm_Quantum_Search.ipynb`.

It uses Python, Qiskit, and Qiskit Aer for circuit construction and simulation.

## Recorded Result

The Colab simulation returned the following measurement counts over 1,000 shots:

\`\`\`text
{'11': 1000}
\`\`\`

The target state `11` appeared in all 1,000 shots in this ideal simulation.

## Interpretation

The result demonstrates the expected behavior of this particular two-qubit circuit with one Grover iteration. It is a simulator result and should not be interpreted as a measurement from real quantum hardware.

## Tools

- Python
- Qiskit
- Qiskit Aer
- Google Colab
- GitHub

## Learning Outcome

This exercise connects quantum superposition, phase marking, interference, and measurement in a small quantum search circuit.

## Status

Practical circuit executed successfully in Google Colab. Repository publication of the notebook and final validation are pending.
