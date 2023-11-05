# quantum-neural-network

A Qbit seems to be a simple spin-1/2 system. The state space of such a system is the 2d Hilbert space (one dimension for each possible measurement). The quantum state of a qbit has the form

$$
|\textrm{qbit}> = \alpha |0> + \beta |1> 
$$

this is normalized, which means that the entire state can be parametrized by one variable. Since that variable is complex, the number of degrees of freedom is 2 and the entire state space for the qbit can be fit into a 2d, the bloch sphere. 

A quantum computer will have N qbits, thus the state space of a quantum computer is the tensor product of N such spaces.

$$
|\textrm{qbit}_1, \textrm{qbit}_2, ..., \textrm{qbit}_n> = \sum_i^n \alpha_i |e_i>
$$

where $|e_i> \in \left ( |00..0>, |100..0>, ..., |111..1> \right ) $.

To implement logic, the qbits go through quantum gates which shape the state of the qbits. The final state of the set of qbits is determined by repeatedly making the qbits go through the gates and measuring the result. The distribution is the result. 



