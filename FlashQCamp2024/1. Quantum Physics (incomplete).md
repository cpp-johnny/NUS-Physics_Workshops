# The Basics of a Qubit

The qubit (standing in for quantum bit) is the simplest case because it is a quantum system with a “two-levelled degree of freedom”, i.e. two-level quantum system (0 or 1) 

It is mathematically described by a vector, usually denoted by a _"ket"_ $\ket{\psi}$, that lives in

$$\ket{\psi} \in \mathbb{C}^2 $$


>💡 ket notation $\ket{ }$ $\equiv$ vector
> - a notation for linear algebra and linear operators on complex vector spaces together with their dual space both in the finite-dimensional and infinite-dimensional case.

The space of quantum states is sometimes called the (complex) Hilbert space, denoted by $H$. 

A qubit state **must** be normalised (i.e. reduced to 1)

$$
\braket{\psi|\psi} = 1
$$
# Computational Basis/Orthonormal Basis

This two-level nature of qubits brings us to the computational basis ($\ket{0}, \ket{1}$)

$$\braket{0|0} = 1$$
$$\braket{1|1} = 1$$
$$\braket{0|1} = 0$$

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

# Measurement of a Qubit - Born's Rule

Given a state $\ket{\psi}$, the probability of measuring $\ket{0}$ or $\ket{1}$ is given by

$$P(0|\psi) = |\braket{0|\psi}|^2$$
$$P(1|\psi) = |\braket{1|\psi}|^2$$


For qubits, this can be expressed as such:

$$P(0|\psi) + P(1|\psi) = 1$$

Naturally, this applies to the $\ket{+}$, $\ket{-}$ basis too:

$$P(+|\psi) + P(-|\psi) = 1$$
# Measurement collapses the state

One of the more peculiar phenomenon in quantum mechanics that you might’ve heard is how measurement change the state of the system being observed.

When we measure $\ket{\psi}$ and find the result $i$, the state ==collapses== to $\ket{i}$. 
> ⚠️ note: some people hate the word collapse, but let's leave that for the discussion circle

# Superposition and Randomness

Consider the state
$$\ket{+} = \frac{\ket{0} + \ket{1}}{\sqrt{2}} $$

When we measure it in the computational basis, there is a 50-50 probability of finding it in either of the basis vectors. 

Sometimes states like $\ket{+}$ and $\ket{-}$ are likened to a coin toss. Half of the time we get heads and the other half of the time we get tails. But this analogy is only good up to a point. Coin tosses are not quantum superpositions. This is because the randomness of a superposition and the “randomness” of a coin toss are very different. Coin tosses seem random to us because we do not know how the coin was flipped and all the various factors that would affect its trajectory and its upward face. Such apparent randomness is really randomness due to ignorance, from lack of knowledge. If we were an expert physicist armed with a supercomputer and all the information relevant to the coin toss, the process would be shown as completely deterministic to us. We would know the outcome once the coin is tossed and win every bet thereafter (that's if the supercomputer can account for every single forces acting on the coin, air resistance and whatnot)!

> 💡 Superpositions do not represent randomness due to ignorance.

This was what the Schrödinger’s Cat thought experiment tries to illustrate. In this thought
experiment, we put a cat into a large sealed box that contains a qubit system and a device.
Preparing the qubit in the $\ket{+}$ state, we connect it to the device, such that if the device measures the system to be in $\ket{0}$ state it would dispense a delicious cat treat. Meanwhile if the device measures the system to be $\ket{1}$ it would dispense a poisonous gas, which kills the cat. It can be described as follows:

$$\ket{cat} = \frac{\ket{0} \otimes \ket{no \space posion} \otimes \ket{alive} + \ket{1} \otimes \ket{poison} \otimes \ket{dead}}{\sqrt{ 2 }}$$

Why Schrodinger came up with this thought experiment is not to say that we will not know if the cat is dead or alive until we open the box. This happens classically (imagine a coin toss that determines the cat being dead or alive). In a classical setting we also don’t know if the cat is dead or alive until we open the box but, note, it had always been alive or dead before that. The result was predetermined prior to measurement.

Rather, with this illustration, Schrödinger was raising the the bizarre conclusion that since we are dealing with a quantum scenario (no coin tosses but a qubit in a relevant superposition), the randomness is genuine and therefore, prior to measurement, the cat was neither dead nor alive but a superposition of both.

But how can life and death be put into superposition? This is the absurd conclusion that
Schrödinger was getting us to consider to see the wild implications of the indeterminism found in quantum theory.







## Ideas to explore
- spin (spin-down, spin-up)
- polarisation of photons (horizontal, vertical)
- atomic energy levels (ground state, excited state)
- beamsplitter
- transmon energy levels


# Reference
1. Qubits & Superposition (Lecture notes by Aw Cenxin Clive, Revised by Peter Sidajaya)

#physics #nus #qcamp
