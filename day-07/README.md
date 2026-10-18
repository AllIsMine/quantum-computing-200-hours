# Day 7 — Simon's Algorithm with Qiskit

## Overview
This project implements Simon's algorithm using Qiskit and the Qiskit Aer simulator to identify a hidden three-bit binary string.

## Objectives
- Understand the XOR operation and Simon's promise.
- Explore quantum superposition using Hadamard gates.
- Construct and test a quantum oracle.
- Simulate quantum measurements.
- Recover a hidden string from binary equations.

## Implementation
The example uses the function:

`f(x0, x1, x2) = (x0 XOR x1, x2)`

The hidden string is `110`.

The notebook verifies the classical function, tests the oracle, constructs the complete quantum circuit, simulates 1,024 shots, and checks the measurement results against Simon's parity condition.

## Tools
- Python
- Qiskit
- Qiskit Aer
- Google Colab

## Result
The simulated measurement results satisfy the expected parity condition, and the recovery step identifies the hidden string `110`.

## Key Learning
This project strengthened my understanding of quantum superposition, CNOT gates, qubit ordering, quantum measurement, and binary equations.

## Limitations
This is a small, simulator-based demonstration. It illustrates Simon's algorithm but does not establish a practical speed advantage on real quantum hardware.

## Notebook
`Day07_Simons_Algorithm.ipynb`

## Quantum Computing Learning Sprint
Part of my 15-day quantum programming sprint, documenting hands-on learning and implementation with Qiskit.
