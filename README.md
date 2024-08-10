# Development-of-Novel-Quantum-Algorithms
Womanium Quantum+AI 2024 Projects

**Please review the participation guidelines [here](https://github.com/womanium-quantum/Quantum-AI-2024) before starting the project.**

_**Do NOT delete/ edit the format of this read.me file.**_

_**Include all necessary information only as per the given format.**_

## Project Information:

### Team Size:
  - Maximum team size = 3
  - While individual participation is also welcome, we highly recommend team participation :)

### Eligibility:
  - All nationalities, genders, and age groups are welcome to participate in the projects.
  - All team participants must be enrolled in Womanium Quantum+AI 2024.
  - Everyone is eligible to participate in this project and win Womanium grants.
  - All successful project submissions earn the Womanium Project Certificate.
  - Best participants win Womanium QSL fellowships with Classiq. Please review the eligibility criteria for QSL fellowships in the project description below.

### Project Description:
  - Click [here](https://drive.google.com/file/d/1PGNUShboB4ik_JHZGcIPTh3KYi-aajzp/view?usp=sharing) to view the project description.

## Project Submission:
All information in this section will be considered for project submission and judging.

Ensure your repository is public and submitted by **August 9, 2024, 23:59pm US ET**.

Ensure your repository does not contain any personal or team tokens/access information to access backends. Ensure your repository does not contain any third-party intellectual property (logos, company names, copied literature, or code). Any resources used must be open source or appropriately referenced.

### Team Information:
Team Member 1:
 - Full Name: Dimitrios Kranas
 - Womanium Program Enrollment ID: WQ24-jxmwGzz36ksdTAF


Team Member 2:
 - Full Name: Haemanth Velmurugan
 - Womanium Program Enrollment ID: WQ24-Fihy1HfM5HbXvCz


Team Member 3:
 - Full Name: N/A
 - Womanium Program Enrollment ID (see Welcome Email, format- WQ24-xxxxxxxxxxxxxxx): N/A


### Project Solution:
We have worked on implementing the paper **"Exponential quantum speedup in simulating coupled classical oscillators"**

The collection of notebooks in our repository describes extensively our work in which we have achieved the following goals:

* Completion of the basic required tasks:
  * Preparation of the initial quantum state in which we encoded the initial positions and velocities of the oscillators
  * Implementation of the Hamiltonian simulation utilizing the quantization method.
We provide a pedagogical explanation and implementation of our code for N=2 oscillators and then generalize it for arbitrary number N.

* Developing our own quantum circuits to address obstacles in the implementation, especially, with encoding phase and initial state preparation, by extending the inbuilt functions of Classiq:
  * Developed an algorithm to perform the LCU decomposition of Pauli strings (i.e. tensor products of Pauli matrices) for Hamiltonian matrices of arbitrary dimensionality N x N.
  * Extended Classiq's function apply_pauli_term() to allow for LCU decomposition of a Hamiltonian with negative expansion coefficients
  * Integrated Classiq's prepare_amplitudes() function, using a unitary `U_matrix` that contains 1's and "i"'s appropriately in its diagonal, to construct a state with complex (purely imaginary) amplitudes

* Post-analysis: Performed resource investigation studying the dependence of the optimized depths on the model parameters such as the ratio of spring constants over masses, the initial positions and velocities and the sparsity of the Hamiltonian. From this analysis we identify critical values beyond which the quantum algorithm becomes inefficient, i.e. requires an extremely large number of gates. (In Progress)

### Project Presentation Deck:
[Slides](./Womanium_slides.pdf)

See project presentation guidelines [here](https://docs.google.com/document/d/13nWF8AxFAfFYTWEYPT3BpPdYkqtxxSAjmuXj_zcMh-E/edit?usp=sharing)

