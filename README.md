# Bell State and Quantum Entanglement with Qiskit

A beginner quantum computing project built using Python and Qiskit.

## Project Objective

The goal of this project is to understand how two qubits can become entangled using a Hadamard gate and a CNOT gate.

## What This Project Does

This notebook:

- Creates a quantum circuit with two qubits and two classical bits
- Starts both qubits in the default state `|00⟩`
- Applies a Hadamard gate to the first qubit
- Applies a CNOT gate using the first qubit as the control and the second as the target
- Creates a Bell state
- Measures both qubits 1,000 times using the Qiskit Aer Simulator
- Displays measurement counts and a bar graph

## Quantum Concept

The circuit starts with:

$$
|00⟩
$$

After applying a Hadamard gate to the first qubit:

$$
|00⟩ \rightarrow \frac{|00⟩ + |10⟩}{\sqrt{2}}
$$

After applying the CNOT gate:

$$
\frac{|00⟩ + |10⟩}{\sqrt{2}}
\rightarrow
\frac{|00⟩ + |11⟩}{\sqrt{2}}
$$

The final state is called a **Bell state**.

## Expected Result

After 1,000 measurements, the expected results are approximately:

- `00`: 50%
- `11`: 50%
- `01`: 0%
- `10`: 0%

The exact counts can vary each time because quantum measurement is probabilistic.

## What Is Entanglement?

Entanglement means the two qubits are correlated.

Each qubit result is individually random, but the pair of results is not random. If the first qubit is measured as `0`, the second is also measured as `0`. If the first is measured as `1`, the second is also measured as `1`.

## Tools Used

- Python
- Qiskit
- Qiskit Aer Simulator
- Matplotlib
- Jupyter Notebook

## Requirements

Install the required libraries before running the notebook:

```python
!pip install qiskit qiskit-aer matplotlib
```

## How to Run

1. Open `bell_state_entanglement.ipynb` in Jupyter Notebook or JupyterLab.
2. Run the installation cell if the required libraries are not installed.
3. Run all notebook cells.
4. Observe the quantum circuit, measurement counts, and bar graph.

## Key Concepts Learned

- Multi-qubit quantum circuits
- Hadamard gate
- CNOT gate
- Bell states
- Quantum entanglement
- Quantum measurement
- Correlated measurement results
- Qiskit circuit simulation

## Future Improvements

- Create the other Bell states
- Compare entangled qubits with classical random bits
- Add a quantum teleportation circuit
- Run the circuit on real quantum hardware
