# Quantum Algorithms

## Introduction 
We begin with the (somewhat vague) definition of quantum computation and quantum information - "The study of information processing with the aid of quantum mechanics". This served as our starting point. Then we got to know about a brief history of information theory and computer science, and saw where the need for quantum computation arised. We learned that a quantum computer can carry out any classical computation.

Just like the _bit_ in classical computation, in quantum computation we deal with _qubits_. The basic difference between them arises from the fact that qubits can exist in _superposition_. We adopt the dirac notation from quantum mechanics, and denote our fundamental unit of quantum computation - the qubit - as,

![equation](https://user-images.githubusercontent.com/73712898/125337962-43996980-e36d-11eb-9663-c9500023b762.png)

where the 0 and 1 'basic states' (enclosed in the _ket_) are our quantum analogues of the classical bits 0 and 1, and, the coefficients satisfy a property called normalisation. Our qubit exists in a linear superposition of these 'basic' states.

In the above equation lies the heart of the matter - We do not know what the quantum computer is made of - nor do we need to - we studied the abstract concept of a qubit, which enables us to study this further without worrying about any physical realisation. Moreover, the '+' in the said equation plays a key role (Superposition!).

## Elementary Quantum Mechanics 
We learned about the bra-ket notation used to represent wavefunctions in quantum mechanics, and for our purposes, qubits. Then went on to vector spaces, the notion of span, dimenstion, linear independence and basis. Then starting with the definition of inner products, we moved on to linear  operators, the definition of hermitian conjugate, and their representation in various basis. Eigenvalues and eigenvectors of operators were discussed, along with the idea of the _completeness relation_. Then we encountered adjoint, hermitian and unitary operators (their matrix representations to be precise - which turns out to be very convinient) along with the definition of _tensor products_, which form the framework for working with multiple qubits. 

With these tools in hand, we studied the postulates of quantum mechanics. Then we devoted some time studing _measurement_ in quantum mechanics. We developed some intuition for the representation of quibits as column vectors, amd quantum gates as matrices.

## Quantum Circuits
Here, we delved into details of the notion of a qubit, and learned about the _gates_ used for quantum computation. We saw some fundamental quantum gates and discussed associated decompositions of arbitrary quantum gates in terms of the former. 
 
We started to look at the basic operations that can be performed on qubits by these gates such as modular addition. Then we extended this idea by looking at _controlled operations_ to move on to circuits like the Quantum SWAP.

We studied the concept of _oracles_ and implemented the same for algorithms such as the Deutch-Josza algorithm. 

Herein we dealt with measurements, and understood the principles of deferred and implicit measurements. Then measurements in different basis were dealt with.

Finally we concluded this section by understanding how some gates are universal, and note that, an arbitrary unitary matrix acting on some _n_ number of qubits can be written as product of two level unitary matrices. Further we saw that single qubit gates and the CNOT gate can be usedf to implement arbitrary unitary operations on some _n_ number of qubits.

## The Quantum Fourier Transform
Just like the discrete fourier transform is a powerful tool in classical computation, we have the QFT in quantum computation. But at the same time, we note that the QFT does not speed up computation of the FT of classical variables in any way. We investigated the use of the QFT in the problem of phase estimation. While looking at the computational resources required for implementing the phase estimation algorithm, we also saw how this is used in the problems of order-finding and factoring, thus studied _Shor's Algorithm_.

## Quantum Search 
We learned about the _Grover's Search Algorithm_ and how it is implemented as an oracle in quantum circuit. We appreciated the quadratic increase in speed that this algorithm enables in the paradigm of "search problems" as compared to classical search algorithms. Then after looking at the algorithm from a geometric perspective we looked at the computational resources required for implementing the same.
## In the end
It does matter. Throughout the project we noticed certain nitty gritties that play a role in the algorithms - from phase kickback to the _Hadamard Magic_. To conclude, we developed a basic idea of the math (Linear Algebra!) behind the physics of it all, and the physics behind the implementation of the algorithms, and implemented some of the algorithms.
### Note
One can see the algorithms rendered properly in the following links
1. [Bernstein-Vazirani Algorithm](https://mybinder.org/v2/gh/midhasid21/Quantum-Algorithms---SoC-21/main?filepath=Bernstein-Vazirani%20Algorithm.ipynb)
2. [Deutsch-Josza Algorithm](https://mybinder.org/v2/gh/midhasid21/Quantum-Algorithms---SoC-21/main?filepath=Deutsch-Jozsa%20Algorithm%20.ipynb)
3. [Super Dense Coding]()
4. [Quantum Fourier Transform]()
5. [Grover's Algorithm](https://mybinder.org/v2/gh/midhasid21/Quantum-Algorithms---SoC-21/main?filepath=Grover%27s%20Algorithm.ipynb)
