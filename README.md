Grover's Algorithm Implementation (2-Qubit System)

1.Overview

This project demonstrates an implementation of Grover's algorithm using Qiskit on a 2-qubit quantum system. Grover's algorithm is a quantum algorithm designed to search for a specific target state in an unsorted database with quadratic speedup compared to classical algorithms. In this example, we aim to find the target state ∣11⟩ from the set of all possible 2-qubit states.

2.Algorithm Steps

2.1 Initialization:

The qubits are initialized in a uniform superposition of all possible states using Hadamard gates.

2.2 Oracle:

The oracle marks the target state ∣11⟩ by flipping its phase using a controlled-Z (CZ) gate.

2.3 Diffuser:

The diffuser amplifies the probability of the target state by reflecting all amplitudes about their mean value. This involves a combination of Hadamard gates, X gates, and a controlled-X (CNOT) gate.

2.4 Measurement:

After applying the oracle and diffuser, the quantum state is measured. The target state ∣11⟩ has the highest probability of being observed.

2.5 Simulation:

The circuit is simulated using Qiskit’s Sampler, and the results are visualized in a histogram to show the probabilities of all possible measurement outcomes.
