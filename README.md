# Simple Quantum Compilation Demo

This project contains a minimal notebook that demonstrates:
- logical circuit definition
- routing/compilation for a constrained device
- noisy measurement simulation
- comparison between logical and compiled behavior

## Files
- `simple_compilation_noise.ipynb`: main demo notebook

## Requirements
- Python 3.10+
- qiskit
- qiskit-aer
- matplotlib
- numpy

Install quickly with:

```bash
pip install qiskit qiskit-aer matplotlib numpy
```

## How to run
1. Open `simple_compilation_noise.ipynb`.
2. Run cells from top to bottom.
3. Check:
   - routed circuit (with two SWAPs)
   - compiled circuit
   - logical vs compiled noisy measurement comparison
