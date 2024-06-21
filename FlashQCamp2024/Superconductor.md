# How to build a quantum computer
According to DiVincenzo's criteria, constructing a quantum computer requires that the experimental setup meet seven conditions. The first five are necessary for quantum computation:

1. A scalable physical system with well-characterized qubit
2. The ability to initialize the state of the qubits to a simple fiducial state
3. Long relevant Quantum coherence times
4. A "universal" set of quantum gates
5. A qubit-specific measurement capability

The remaining two are necessary for quantum communication:

6. The ability to interconvert stationary and flying qubits
7. The ability to faithfully transmit flying qubits between specified locations

# Cooper pairs
Normal metals like copper and gold are very efficient in carrying electric currents and, in many situations, their resistance can be considered to be zero. But this is just an approximation. In any metal, flowing electrons constantly bump (or more precisely, scatter) onto the ions that compose the material. Because of these obstacles, the electrons reach a maximum velocity that is related to the resistivity of the metal.

But metals have a hidden feature, a very weak interaction that went by unnoticed for too long: the fields cast out by ions can make two electrons attract each other. In principle, these two electrons should be pushed apart due to their negative charges. However, when they are moving in opposite directions, the lattice of ions effectively makes them pair up. When two electrons are connected in that way (forming a Cooper pair), they avoid the ion scattering altogether. Without the scattering, there is no maximum velocity and the resistivity becomes actually zero.

This microscopic mechanism was proposed by Bardeen, Cooper and Schrieffer in 1957 to explain superconductivity. Their calculations also show that, even though this electron-pairing effect is always present, high thermal energy easily breaks the Cooper pairs. That is why superconductivity occurs at very cold temperatures.

# Properties of Superconductors
1. Zero resistance
	- current can flow without voltage drop
2. Meissner effect
	- magnetic field cannot penetrate ($T<T_{c}$)
3. Flux quantization
	- persistent currents will maintain a constant magnetic field through holes
	- $\Phi = B \cdot A = n\phi_{0}$
	- $\phi_{0} = \frac{h}{2e}$

# Types of Superconductors
A strong magnetic field will break apart the Cooper pairs

1. Type I (explained by BCS)
	- Al, Nb, Ta, Hg etc
2. Type II (Higher $B_{c}$ and $T_{c}$)
	- Mixture of normal and superconducting
	- NbTi, YBCO, NB$_{3}$Sn etc

# The Josephson Junction
A Josephson junction is a quantum mechanical device made up of two superconducting materials separated by a very thin insulating layer. This configuration allows for some unique and fascinating electrical properties, primarily due to the phenomenon of quantum tunnelling. 
### Basic Structure

- **Superconductors**: These are materials that can conduct electricity without resistance below a certain temperature (the critical temperature).
- **Insulating Layer**: This thin layer (often just a few nanometers thick) separates the two superconductors and is crucial for the Josephson effect.

### Josephson Effect

The Josephson junction operates based on the principles of quantum mechanics. There are two key effects:

**DC Josephson Effect**
Even without any voltage applied across the junction, a supercurrent (a current with no resistance) can flow between the two superconductors due to quantum tunnelling. This current depends on the phase difference of the superconducting wave functions on either side of the insulator.

$$I=I_{c}sin⁡(ϕ)$$
Here, $I$ is the supercurrent, $I_{c}$​ is the critical current (the maximum supercurrent that can flow without resistance), and $ϕ$ is the phase difference of the superconducting wave functions.

**AC Josephson Effect**
When a constant voltage $V$ is applied across the junction, the phase difference $ϕ$ changes over time, leading to an alternating current (AC) at a frequency $f$ given by:

$$f= \frac{2eV}{h}$$

where 
$e$ is the electron charge  
$h$ is Planck's constant.

or

$$\frac{dϕ}{dt}​=\frac{2\pi}{\Phi_{0}}V$$

where 
$ϕ$: The phase difference between the superconducting wave functions on either side of the junction.
$V$: The voltage applied across the Josephson junction.
$Φ_{0}$​: The magnetic flux quantum, which is a fundamental constant given by $Φ_{0} = \frac{h}{2e}$​

### Relation with Ohm's Law
The Josephson junction and Ohm's law describe different aspects of electrical behaviour: classical resistive behaviour vs. quantum superconducting behaviour. The Josephson junction reflects the quantum mechanical properties of superconductors, where current can flow without resistance and the relationship between voltage and current involves phase differences and quantum tunnelling. While not a direct analogue, the study of Josephson junctions provides insights into quantum mechanical effects in electrical systems, enriching our understanding beyond classical concepts like Ohm's law.

#physics #nus #qcamp