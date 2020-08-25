# universe-simulation
An interactive N-body simulation of stars moving in a box
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/annamnliang/universe-simulation/master)

## Introduction
This interactive Jupyter Notebook generates simple simulations of particles moving in a box with only gravitational interactions. It uses widgets to take in user inputs for a system of particles (e.g. the number of particles, their mass, their initial configuration) and displays the animation of the particles' movements, as well as the corresponding correlation function and power spectrum over time. 

## Installing Dependencies
This notebook requires a Python3 kernel to run. The best way to run this it is to install Anaconda, which has the Jupyter Notebook application. The required packages are listed in the file 'environment.yml'. These packages can be installed in a Conda environment using 
```
git clone https://github.com/annamnliang/universe-simulation
cd universe-simulation
conda env create -f environment.yml
````
Alternatively, this notebook is also hosted on [Binder](https://mybinder.org/v2/gh/annamnliang/universe-simulation/master) which has been pre-built to run with the required conda environment. This will run the applet slower than in Conda. 

## Running The Notebook
To run the notebook in Conda in the installed environment, use 
```
conda activate simulation-environment
jupyter notebook universe-simulation.ipynb
````
To turn the notebook into an interactive applet, the "Hide input all" extension needs to be added to the toolbar. To do so, go to the toolbar "Edit" >> "nbextensions config" which opens up the full list of settings in another window. Enable "Hide input all" and restart the notebook. In the toolbar at the top of the notebook, there should now be an eye icon. Clicking it will hide all the code. To run the notebook, first run all cells via "Kernel" >> "Restart and Run All".

Running all the cells will generate the results for a preset initial configuration and parameters but will also show all the widgets to enable the user to choose their own parameters. Each time a parameters has been varied, to rerun the simulation, click "Simulate my universe!" and the results will load. For each different intial distribution of particles, a corresponding description and interpretation of the animation will also be generated. 
