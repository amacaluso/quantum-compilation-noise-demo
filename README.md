# Quantum Circuit Compilation and Noise Comparison

This repository contains a minimal, reproducible example that compares a logical quantum circuit with its compiled version on a constrained device model, then evaluates measurement outcomes under noise.

## What This Repo Contains

1. `simple_compilation_noise.ipynb`
   End-to-end notebook with three steps:
   Define a logical circuit.
   Build and compile a routed circuit for a linear 3-qubit device.
   Simulate noisy measurements and compare logical vs compiled results.
2. `requirements.txt`
   Minimal Python dependencies required by the notebook.

## Why This Example Is Useful

1. Shows how hardware constraints (connectivity and basis gates) change a circuit.
2. Makes SWAP overhead explicit in routing.
3. Demonstrates that deeper compiled circuits are often more sensitive to noise.
4. Keeps the workflow intentionally small and easy to reuse.

## Quick Start

1. Create and activate a Python environment.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Start Jupyter:

```bash
jupyter notebook
```

4. Open `simple_compilation_noise.ipynb` and run all cells from top to bottom.

## Notebook Flow

1. Step 1: Define the logical circuit.
2. Step 2: Route with two explicit SWAPs and compile to target basis gates.
3. Step 3: Build a noise model and compare ideal vs noisy measurement distributions for both logical and compiled circuits.

## Notes

1. State sorting in the notebook is numeric by bitstring value for stable comparisons.
2. The current branch (`main`) keeps only the minimal notebook example.
3. Other notebook history is preserved in branch `notebooks-archive`.
