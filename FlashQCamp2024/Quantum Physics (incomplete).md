# The Basics of a Qubit

The qubit (standing in for quantum bit) is the simplest case because it is a quantum system with a “two-levelled degree of freedom”, i.e. two-level quantum system (0 or 1) 

It is mathematically described by a vector, usually denoted by a _"ket"_ $\ket{\psi}$, that lives in

$$\{\ket{\psi} \in \mathbb{C}^2 \}$$

>💡 ket notation $\ket{ }$ $\equiv$ vector
> - a notation for linear algebra and linear operators on complex vector spaces together with their dual space both in the finite-dimensional and infinite-dimensional case.

The space of quantum states is sometimes called the (complex) Hilbert space, denoted by $H$. 

A qubit state **must** be normalised (i.e. reduced to 1)

$$
\braket{\psi|\psi} = 1
$$
# Computational Basis/Orthonormal Basis

This two-level nature of qubits brings us to the computational basis ($\ket{0}, \ket{1}$)

$$
\braket{0|0} = 1
$$
$$
\braket{1|1} = 1
$$
$$
\braket{0|1} = 0
$$
Note: $\ket{0}, \ket{1}$ is just a notation, we could also use $\ket{g}, \ket{e}$ or $\ket{\uparrow}, \ket{\downarrow}$ or $\ket{一}, \ket{零}$ etc...

These are the two possible outcomes if we make a measurement “along the 0/1 basis”. A qubit can only give one of two outcomes specific to that kind of measurement. Note that every ket (in a complex space like ($ℂ^2$)) can be represented by vectors. For instance |0i and |1i can be represented as vectors as such:

$$
\ket{0} \hat{=} \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \ket{1} \hat{=} \begin{bmatrix} 0 \\ 1 \end{bmatrix} \
$$

# Superposition

Consider the following states, 

$$\ket{+} = \frac{\ket{0}+ \ket{1}}{\sqrt{2}}$$
$$\ket{-} = \frac{\ket{0} - \ket{1}}{\sqrt{2}}$$

or in matrices,

$$\ket{+} \hat{=} \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}$$
$$\ket{-} \hat{=} \frac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix}$$

These states are a **superposition** of $\ket{0}$ and $\ket{1}$. 

# A General Qubit

Are there other states than $\ket{0}$, $\ket{1}$, $\ket{+}$ and $\ket{-}$?

Every qubit can be written as 

$$\ket{\psi} = a\ket{0} + b\ket{1} $$

where $a$, $b$ are complex numbers and $|a|^2 + |b|^2 = 1$








## Ideas to explore
- spin (spin-down, spin-up)
- polarisation of photons (horizontal, vertical)
- atomic energy levels (ground state, excited state)
- beamsplitter
- transmon energy levels


#physics #nus #qcamp
