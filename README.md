# RLithium

## What is RLithium
RLithium is a library for Lithium-Ion Battery simulation. It models and simulates a domestic environment composed of a house that consumes electric energy and a photo-voltaic panel that procuces energy. The domestic environment is linked to a controller that decides how much of the net power coming from the domestic environment will be directed on an accumulation system and how much will be bought/sold on the electric grid.
The simulator has been written following the standard framework [Gym](https://gym.openai.com/) from [OpenAI](https://openai.com/). The repository contains a wrapper for the library [MushroomRL](https://mushroomrl.readthedocs.io/en/latest/), used to design and test RL agents.

## Installation
Use [Conda](https://docs.conda.io/en/latest/) to install all the dependecies of RLithium using the provided configuration file _requirements.yml_.
```sh
conda env create -f requirements.yml
```

RLithium depends on depencendies of [Gym](https://gym.openai.com/docs/) and [MushroomRL](https://github.com/MushroomRL/mushroom-rl). Visit their installation page for instruction on external dependecies.
On some systems, it may be necessary to set an environment variable for the _open-mpi_ dependency.
```sh
MPICC=/path/to/your/mpicc/executable
```

## Repository Structure
The repository is structured in the following way:
* **current_directory**: contains the scripts used to train and test an agent using the Fitted Q-iteration algorithm
* **./rse_lib**: contains the source code of the repository and the definition of the Gym and MushroomRL environments
* **./data**: contains data used to perform the simulations
* **./notebooks**: contains some python notebooks with examples and visualization


