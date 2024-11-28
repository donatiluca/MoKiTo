# MoKiTo: Molecular Kinetics via Topology

MoKiTo (Molecular Kinetics via Topology) is a Python-based toolkit designed for analyzing and extracting topological insights from molecular dynamics (MD) simulations.   
It enables researchers to study structural transitions and kinetic pathways in molecular systems.

## Installation
git clone https://github.com/donatiluca/MoKiTo.git  
pip install -r requirements.txt


## How to Use MoKiTo
The workflow depends on whether you're working with toy model systems (typically one- or two-dimensional systems driven by overdamped Langevin dynamics) or all-atom MD simulations.  
The directory `examples/` contains sample workflows for both use cases. Modify the scripts as needed for your specific data and analysis.

### Low-Dimensional Systems

For low-dimensional systems, follow these steps:

1. Use `generate_trajectories.ipynb` to create the initial trajectory and the short trajectories.
2. Use `isokann.ipynb` to learn the $\chi$-function.
3. Use `mokito.ipynb` to load the trajectories and the $\chi$-function to generate the graph and the energy landscape.