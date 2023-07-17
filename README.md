In this project, I use neural networks to understand the phases of a spin system (see Refs.). In particular, my goal is twofold: 
* (i) identify whether a spin configuration is hot (paramagnetic phase) or cold (ferromagnetic phase)
* (ii) estimate the critical transition point of the phase transition.

The spin system is described a toy model, known as ["Ising model"](https://en.wikipedia.org/wiki/Ising_model), which is used to understand the temperature behavior of a magnet. Here, the spins have 2 states: up or down. At low tempatures, spins point in only one direction that leads to a net magnetic moment with ferromagnetic phase. Increasing the temperature leads to thermal fluctuation, and at one point, the magnetism is lost -- i.e. paramagnet state with alomst equal number of up and down spin appears.

`01_generateData.ipynb` -- Builds Ising model on a square lattice and generates the datasets.

`02_ising_neural_net.ipynb` -- NN models are trained and validated using the generated datasets.

Run `pip install pip install requirements.txt` to install dependencies.

Reference: [Carrasquilla et al., Nat. Phys. 13, 431–434 (2017)](https://www.nature.com/articles/nphys4035)