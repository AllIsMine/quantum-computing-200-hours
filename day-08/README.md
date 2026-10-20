
# Day 8 — Advanced Quantum Phase Estimation (QPE)

## Overview

Day 8 extends the Quantum Phase Estimation (QPE) work through precision experiments, exact-phase validation, and a comparison of ideal and illustrative noisy simulations.

## Notebook

- **Notebook:** [`day08_Advanced_Quantum_Phase_Estimation.ipynb`](day08_Advanced_Quantum_Phase_Estimation.ipynb)
- **Environment:** Google Colab
- **Qiskit version:** 2.6.0
- **Qiskit Aer version:** 0.18.0

## Experiments Completed

- Implemented QPE precision experiments using 2, 3, 4, and 5 counting qubits.
- Compared phase-grid spacing, modal estimates, sample means, and sampling spread.
- Ran exact-phase regression tests for five phase values.
- Evaluated the four-counting-qubit experiment using the target phase `0.30`.
- Compared ideal and illustrative noisy simulation results using 8,192 shots per run.

## Key Results

For the target phase `0.30`, the four-counting-qubit experiment produced:

- **Modal bitstring:** `0101`
- **Estimated phase:** `0.3125`
- **Absolute phase error:** `0.0125`

The ideal-versus-noisy comparison produced:

| Metric | Ideal simulation | Noisy simulation |
|---|---:|---:|
| Modal bitstring | `0101` | `0101` |
| Modal outcome frequency | 87.56% | 65.38% |
| Estimated phase from sample mean | 0.31264 | 0.33760 |
| Sample standard deviation | 0.05957 | 0.15620 |

These results illustrate how noise can broaden measurement distributions and affect phase estimates.

## Noise and Reproducibility

The ideal and noisy experiments were run in simulation. The noisy simulation uses an illustrative noise model, including depolarizing and readout errors.

These results are not measurements from real quantum hardware and do not represent a calibrated device noise model.

The notebook records the software versions used. Refer to its simulation setup cells for the exact noise-model parameters.

## Validation Status

- [x] Notebook executed from top to bottom in Google Colab.
- [x] Precision experiments completed for 2–5 counting qubits.
- [x] Exact-phase regression tests passed.
- [x] Four-counting-qubit phase estimate recorded.
- [x] Ideal-versus-noisy simulation comparison completed.
- [x] Qiskit and Qiskit Aer versions recorded.
- [ ] Final executed notebook and progress note committed to GitHub.

## Next Roadmap Task

**Day 9 — Transpilation + Backend Optimization**

The next task follows the existing learning roadmap and will cover transpilation optimization levels, circuit depth and gate counts, layout, and routing.
