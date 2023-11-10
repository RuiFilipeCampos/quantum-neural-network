# quantum-neural-network

A Qbit seems to be a simple spin-1/2 system. The state space of such a system is the 2d Hilbert space (one dimension for each possible measurement). The quantum state of a qbit has the form

$$
|\textrm{qbit}> = \alpha |0> + \beta |1> 
$$

this is normalized, which means that the entire state can be parametrized by one variable. Since that variable is complex, the number of degrees of freedom is 2 and the entire state space for the qbit can be fit into a 2d sphere, often called the bloch sphere. 

A quantum computer will have N qbits, thus the state space of a quantum computer is the tensor product of N such spaces.

$$
|\textrm{qbit}_1, \textrm{qbit}_2, ..., \textrm{qbit}_n> = \sum_i^n \alpha_i |e_i>
$$

where $|e_i> \in \left ( |00..0>, |100..0>, ..., |111..1> \right ) $.

To implement logic, the qbits go through quantum gates which shape the state of the qbits. The final state of the set of qbits is determined by repeatedly making the qbits go through the gates and measuring the result. The distribution is the result. 


## Quantum Neuron

![image](https://github.com/RuiFilipeCampos/quantum-neural-network/assets/63464503/e6345dbe-2429-43ef-9bee-fe3333c11bdb)


- The horizontal lines represent qubits in the quantum system. The |0⟩ indicates that the qubits start in the zero state.
- The H gates are Hadamard gates, which create superpositions of qubit states. They are applied to each of the top qubits, placing them into an equal superposition of |0⟩ and |1⟩.
- The vertical lines with dots at the top and a box at the bottom represent controlled gates, specifically controlled phase shift gates. The dots represent control qubits and the boxes are the target qubits. The notation ( $U_{\omega}^{2^k}$ ) indicates a controlled rotation, with ω being a complex root of unity and k depending on the position of the gate in the circuit.
- The $QFT^{-1}$ box represents the inverse Quantum Fourier Transform being applied to the top qubits. The QFT is a quantum version of the discrete Fourier transform, and it is fundamental to many quantum algorithms.
- The symbol on the right is a measurement gate, indicating the qubit's state is being measured, collapsing the superposition to a definite state.


