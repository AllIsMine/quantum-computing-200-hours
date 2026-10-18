# Day 6 — Quantum Fourier Transform and Quantum Phase Estimation

## Learning Objectives
- Understand quantum phases and controlled-phase rotations.
- Implement a two-qubit Quantum Fourier Transform (QFT).
- Verify the QFT against its mathematical unitary matrix.
- Implement and validate the inverse QFT.
- Build a Quantum Phase Estimation (QPE) circuit using Qiskit.

## Experiments Completed
- [x] Hadamard gate and superposition
- [x] Relative phase and interference
- [x] Controlled-phase gate
- [x] Two-qubit QFT implementation
- [x] Mathematical QFT verification
- [x] Inverse QFT recovery tests
- [x] QPE simulation

## QPE Result
The ideal Aer simulation returned `01` in all 1,024 shots, correctly estimating the phase `0.01₂ = 0.25`.

## Tools
- Python
- Qiskit
- Qiskit Aer
- Google Colab

## Next Steps
Study Simon's algorithm and deepen the understanding of quantum algorithms.

**Note:** The QPE result was obtained using an ideal simulator, not physical quantum hardware.
