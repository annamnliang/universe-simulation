# Choose Your Own Universe
An interactive N-body simulation of stars moving in a box

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/annamnliang/universe-simulation/master)

## Introduction
This interactive Jupyter Notebook generates simple simulations of particles moving in a box with only gravitational interactions. It uses widgets to take in user inputs for a system of particles (e.g. the number of particles, their mass, their initial configuration) and displays the animation of the particles' movements, as well as the corresponding correlation function and power spectrum over time. 

## Installing Dependencies
This notebook requires a Python3 kernel to run. The best way to run this offline is to install [Anaconda](https://docs.anaconda.com/anaconda/install/), which has the Jupyter Notebook application. The required packages are listed in the file 'environment.yml'. These packages can be installed in a Conda environment using 
```
git clone https://github.com/annamnliang/universe-simulation
cd universe-simulation
conda env create -f environment.yml
````
Alternatively, this notebook is also hosted on [Binder](https://mybinder.org/v2/gh/annamnliang/universe-simulation/master) which has been pre-built to run with the required conda environment and requires no downloads. It works fastest in Chrome or Safari (avoid Firefox). The first time the link runs will take a little time to load so it can build the environment. 

## Running The Notebook
To run the notebook in Conda in the installed environment, use 
```
conda activate simulation-environment
jupyter notebook universe-simulation.ipynb
````
Or in Binder, the link will take you to the Jupyter Notebook homepage for this repository where you can then open "universe-simulation.ipynb". 

To turn the notebook into an interactive applet, the "Hide input all" extension needs to be added to the toolbar. To do so, go to the menu toolbar >> "Edit" >> "nbextensions config" which opens up the full list of settings in another window. Uncheck the option "disable configuration for nbextensions without explicit compatibility" at the top of page. Enable "Hide input all" and restart the notebook. In the toolbar at the top of the notebook, there should now be an eye icon. Clicking it will hide all the code. Then to run the notebook, first run all cells via menu >> "Kernel" >> "Restart and Run All".

Running all the cells will generate the results for a preset initial configuration and parameters but will also show all the widgets to enable the user to choose their own parameters. Each time a parameters has been varied, to rerun the simulation, click "Simulate my universe!" and the results will load. For each different intial distribution of particles, a corresponding description and interpretation of the animation will also be generated. 

## Using the code
The code provides a manual of how the particle dynamics are calculated, as well as the correlation function and power spectrum. Then, the user can choose the parameters they want to test. Some preset options can be used by selecting the initial configuration desired in the dropdown menu and not changing the other parameters. Or, the parameters can be changed to any combination of the widget's allowed values. Once this has been done, click "Simulate my universe!" to generate the animation of the output. While the animation loads, some insights and interesting analysis, as well as suggestions for the next run, will be displayed. The parameters can be changed at any time and clicking "Simulate my universe!" will rerun the code with the new inputs. 

To view the source code, simply uncheck the "Hide input all" icon and the code cells will be displayed. 
