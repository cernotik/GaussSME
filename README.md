# Adiabatic elimination of Gaussian subsystems in stochastic quantum dynamics

## Author

Ondrej Cernotik

Institute for Theoretical Physics, Institute for Gravitational Physics (Albert Einstein Institute), Leibniz University Hannover, Germany

## About this repository

This project deals with numerical simulations of conditional dynamics
of composite quantum systems. The main goal is to compare the method of
adiabatic elimination presented in Ref. [1] with exact numerical solution
of the full stochastic master equation and with other adiabatic elimination
methods. The files in this repository simulate the dynamics of
superconducting qubits coupled to harmonic oscillators in various settings,
including the presence of thermal bath. The code can however be readily
adapted to simulate other quantum systems under continuous monitoring.
 
Refer to the list of files below and the individual IPython notebook
files for more information.
 
The quantum dynamics is implemented using the QuTiP package [2,3].
 
For license terms, see LICENSE.

### Files

* Dispersive qubit readout.ipynb

Simulates dispersive readout of a superconducting qubit using a cavity mode coupled to a thermal bath, as studied in Sec. III.A of Ref. [1]. The results obtained by approximate adiabatic elimination methods are compared with the exact solution by taking the trace distance between the exact and approximate solutions.

* Jaynes-Cummings coupling.ipynb

Similar to 'Dispersive qubit readout.ipynb' but with the qubit-cavity coupling that takes the form of Jaynes-Cummings Hamiltonian.

* Parity measurement.ipynb

Analyzes protocol for generating two-qubit entanglement by
measurement, following the approach of Ref. [4]. Both qubits
dispersively couple to a single cavity mode that is being measured.
Starting from a suitable initial state and using postselection,
the two qubits can be found in an entangled state. Here we
generalize the results of Ref. [4] by considering a cavity field
that is coupled to a thermal reservoir.

* Two-oscillator transducer.ipynb

Here we analyze the accuracy of approximate solution of a
dispersive qubit readout by a system comprising two coupled
harmonic oscillators. The first oscillator interacts with the
qubit and couples to a thermal bath, while the second one
interacts with vacuum bath which is also used for the state
readout. This file uses the general formalism of Ref. [1],
making it possible to apply the method to other quantum systems.

* LICENSE.txt

License terms. This work is published under the GNU GPL v2 license.

* README.md

This file

## References

[1] O. Cernotik, D. Vasilyev, and K. Hammerer, *Adiabatic elimination of Gaussian subsystems in stochastic quantum dynamics*, [arXiv:1503.07484](http://www.arxiv.org/abs/1503.07484).

[2] J. R. Johansson, P. D. Nation, and F. Nori, *QuTiP: An open-source Python framework for the dynamics of open quantum systems*, [Computer Physics communications **183**, 1760 (2012)](http://dx.doi.org/10.1016/j.cpc.2012.02.021).

[3] J. R. Johansson, P. D. Nation, and F. Nori, *QuTiP2: A Python framework for the dynamics of open quantum systems*, [Computer Physics Communications **184**, 1234 (2013)](http://dx.doi.org/10.1016/j.cpc.2012.11.019).

[4] C. L. Hutchison, J. Gambetta, A. Blais, and F. K. Wilhelm, *Quantum trajectory equation for multiple qubits in circuit QED: Generating entanglement by measurement*, [Canadian Journal of Physics **87**, 225 (2009)](http://dx.doi.org/10.1139/P08-140).
