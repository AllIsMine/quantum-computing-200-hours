# Day 8 — Advanced Quantum Phase Estimation

## Overview

This project extends Quantum Phase Estimation (QPE) using Qiskit and Qiskit Aer. It investigates phase-estimation precision, validates exact-phase cases, and compares ideal and illustrative noisy simulations.

## Objectives

- Understand how the number of counting qubits affects phase-estimation precision.
- Implement and validate QPE experiments.
- Test exact phases using regression checks.
- Compare modal estimates, sample means, and sampling spread.
- Investigate how a configured noise model affects measurement results.
- Document reproducible experiments and simulator limitations.

## Implementation

The notebook extends the existing QPE experiment with precision comparisons for two to five counting qubits, exact-phase regression tests, and ideal-versus-noisy simulation.

The target phase in the four-counting-qubit experiment is φ = 0.30.

## Tools

- Python
- Qiskit 2.x
- Qiskit Aer
- NumPy
- Google Colab
- Git and GitHub

## Results

For the target phase φ = 0.30, the four-counting-qubit experiment produced the modal bitstring `0101`, corresponding to an estimated phase of 5/16 = 0.3125.

The absolute error was 0.0125.

In an 8,192-shot comparison, the modal outcome frequency was approximately 87.56% in the ideal simulation and 65.38% in the illustrative noisy simulation.

The exact-phase regression tests passed for all tested phases.

**Important:** These results are from simulation. The noisy model is illustrative and does not represent calibration data from physical quantum hardware.

## Key Learning

This project develops an understanding of phase-estimation precision, measurement distributions, regression testing, and the effects of simulated noise on quantum algorithm outcomes.

## Limitations

The results depend on the chosen circuit, shot count, simulator, and noise assumptions. They do not establish performance on real quantum hardware.

## Notebook

`day08_Advanced_Quantum_Phase_Estimation_Continued.ipynb`

## Quantum Computing Learning Sprint

Part of my ongoing quantum programming sprint, documenting hands-on learning and implementation with Qiskit.
