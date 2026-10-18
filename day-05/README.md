# Day 5 — Grover's Algorithm and Quantum Search

## Overview

This exercise implements a two-qubit example of Grover's quantum search algorithm using Qiskit and Qiskit Aer. It demonstrates how an oracle marks a target state and how a diffusion operator amplifies its amplitude.

Two target states are tested: `11` and `10`. Both experiments use an ideal simulator and 1,000 shots.


## Learning Objectives

- Prepare an equal superposition of two qubits.
- Implement a phase oracle using a controlled-Z gate.
- Modify the oracle to search for a different target state.
- Construct and apply the diffusion operator.
- Simulate quantum circuits using Qiskit Aer.
- Validate measurement results with Python assertions.
- Understand qubit indexing, measurement output, and simulator limitations.

## Algorithm Workflow

1. **Superposition:** Apply Hadamard gates to both qubits to prepare an equal superposition of the four computational basis states.
2. **Oracle:** Mark the target state by applying a phase change. For target `11`, a controlled-Z gate is used directly. For target `10`, X gates on qubit 0 are applied before and after the controlled-Z gate.
3. **Diffusion:** Apply the diffusion operator to amplify the target state's amplitude.
4. **Measurement:** Measure both qubits and inspect the output counts.
5. **Validation:** Compare the observed counts with the expected target state using assertions.

## Experiments and Results

### Experiment 1 — Target `11`

The circuit prepares a superposition, marks `11` with a controlled-Z oracle, applies the diffusion operator, and measures both qubits.

Ideal Qiskit Aer result for 1,000 shots:

```text
Measurement counts: {'11': 1000}
Day 5 Grover's algorithm test passed!
```

### Experiment 2 — Target `10`

The oracle is modified to mark `10`. An X gate is applied to qubit 0 before and after the controlled-Z gate, while the diffusion operator remains unchanged.

Ideal Qiskit Aer result for 1,000 shots:

```text
Measurement counts: {'10': 1000}
Grover target-10 test passed!
```

## Interpretation

Both target states appeared in all 1,000 shots in their respective ideal simulations, and both assertions passed. These results demonstrate the expected behavior of these particular two-qubit circuits with one Grover iteration.

The target-10 experiment also provided a debugging lesson: an initial oracle modification produced `01` instead of `10`. Reviewing Qiskit's qubit indexing and displayed measurement-bit order helped identify the issue and correct the oracle.

## Limitations

These are ideal simulator results, not measurements from real quantum hardware. Actual hardware results can vary because of noise, gate errors, and measurement errors. This small two-qubit example illustrates the mechanism of Grover's algorithm; it does not establish a practical speed advantage for large search problems.

## Tools and Environment

- Python
- Qiskit
- Qiskit Aer
- Google Colab
- Git and GitHub

## Learning Outcome

This exercise connects superposition, phase marking, interference, measurement, assertions, and debugging in a small quantum search circuit. It also demonstrates how changing the oracle changes the target state being searched for.

## Status

Both target-state experiments have been implemented and validated using the ideal Qiskit Aer simulator. The notebook and this documentation are published in the repository.
