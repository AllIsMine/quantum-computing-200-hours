# Day 6 — Quantum Fourier Transform (QFT) and Quantum Phase Estimation (QPE)

## 🎯 Learning Objectives

- Understand quantum superposition, relative phase, and interference.
- Explore controlled-phase rotations.
- Implement a two-qubit Quantum Fourier Transform (QFT) using Qiskit.
- Verify the QFT against its mathematical unitary matrix.
- Implement the inverse QFT and validate state recovery.
- Build and simulate a Quantum Phase Estimation (QPE) circuit.

## 🧪 Experiments Completed

- [x] Hadamard gate and quantum superposition
- [x] Relative phase and quantum interference
- [x] Controlled-phase gate with angle π/2
- [x] Two-qubit QFT implementation
- [x] Mathematical QFT unitary verification
- [x] Inverse QFT validation
- [x] Recovery tests for all four computational basis states
- [x] QPE circuit implementation and simulation

## 📊 Key Results

### Quantum Fourier Transform
- Verified the implemented QFT against the mathematical Fourier-transform matrix.
- Result: `True`

### Inverse QFT
- Verified that QFT followed by inverse QFT returns the identity operation.
- Confirmed successful recovery of all four computational basis states.

### Quantum Phase Estimation
- Estimated the phase of a known unitary eigenstate.
- Expected phase: φ = 0.25 = 0.01₂
- Measurement result: `{'01': 1024}`
- Shots: 1,024
- Observed frequency for the expected outcome: 100%

**Important:** These results were obtained using an ideal Qiskit Aer simulation, not physical quantum hardware.

## 🛠️ Tools and Technologies

- Python
- Qiskit 2.x
- Qiskit Aer
- NumPy
- Google Colab

## 🧠 Key Takeaways

This project demonstrates how quantum phase information can be transformed and estimated using QFT, inverse QFT, and QPE. It also emphasizes mathematical verification, circuit debugging, and reproducible simulation.

## 🚀 Next Steps

- Study Simon's algorithm and hidden-bit-string recovery.
- Explore the relationship between quantum algorithms and hidden periodic structure.
- Continue developing and documenting quantum programming experiments.

## 📁 Project Structure

```text
day-06/
├── README.md
└── Day06_Quantum_Fourier_Transform.ipynb
```

**Day 6 status: Completed — QFT and QPE validated in simulation.**
