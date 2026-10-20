# Day 9 — Transpilation and Backend Optimization

## Objective

Understand how Qiskit transpilation adapts a quantum circuit to hardware connectivity constraints, optimization settings, and a specified gate basis.

## Environment

- Qiskit: 2.6.0
- Platform: Google Colab
- Circuit: Three-qubit example
- Hardware model: Linear three-qubit coupling map

## Experiments

1. Built a three-qubit circuit and measured its depth and gate counts.
2. Compared transpilation optimization levels 0, 1, 2, and 3.
3. Created a linear coupling map with connections between neighboring qubits.
4. Transpiled the circuit with hardware connectivity constraints.
5. Measured routing overhead.
6. Compared optimization levels 0 and 3 under the same connectivity constraints.
7. Investigated qubit layout and verified circuit equivalence.
8. Decomposed the circuit into the specified basis gates: `rz`, `sx`, `x`, and `cx`.
9. Verified the basis-gate circuit using layout-aware operator conversion.

## Results

| Experiment | Gate count | Circuit depth | SWAP gates |
|---|---:|---:|---:|
| Original circuit | 5 | 4 | 0 |
| Routed, optimization level 0 | 6 | 5 | 1 |
| Routed, optimization level 3 | 6 | 5 | 1 |
| Specified basis-gate circuit | 12 | 9 | 0 reported as a native SWAP gate |

The basis-gate circuit used 5 `rz` gates, 2 `sx` gates, and 5 `cx` gates.

## Key Findings

- Higher optimization levels do not guarantee fewer gates or lower circuit depth.
- Routing can add operations to satisfy connectivity constraints.
- In this experiment, routing increased gate count by 20% and circuit depth by 25%.
- Basis-gate decomposition changed the circuit representation and increased its gate count and depth.
- Raw operator comparisons can be misleading when qubit layouts differ.
- Layout-aware verification returned `True` for the routed circuits and the basis-gate circuit.

## Conclusion

This experiment demonstrated how transpilation, routing, layout, optimization, and basis-gate decomposition work together. It also highlighted the importance of verifying quantum operations after circuit transformations.

The connectivity map used here is an educational model, not a representation of a specific real quantum backend.

## Files

- `Day09_Transpilation_Backend_Optimization.ipynb` — code, outputs, experiments, and learning notes.
