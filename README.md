# EC-Simulator
![GitHub commit activity](https://img.shields.io/github/commit-activity/w/anon98/EC_simulator)
![GitHub License](https://img.shields.io/github/license/anon98/EC_simulator)
[![Build](https://github.com/anon98/EC-simulator/actions/workflows/main.yml/badge.svg)](https://github.com/anon98/EC-simulator/blob/main/.github/workflows/main.yml)




## Overview

This is a Julia-based simulation test project that models an energy community with solar generation, battery storage, and cooperative energy management.

## Setup Instructions

1. **Julia Installation and Setup:**\
    ``
    sudo add-apt-repository ppa:staticfloat/juliareleases
   ``
   
     ``
    sudo apt-get update
    ``
   
     ``
    sudo apt-get install julia
    ``
   
Install Packages:
       
    (@v1.7) pkg> add Random
    (@v1.7) pkg> add Plots
    (@v1.7) pkg> add FilePathsBase
    (@v1.7) pkg> add JSON
3. **Clone the Repository:**

   ```bash
   git clone https://github.com/anon98/test_julia.git
   cd EC-simulator
3. **Config File**
    Settings/config.json
    example:
   ```bash
   {
    "simulation_parameters": {
        "dt": 0.1,
        "simulation_hours": 24
    },
    "grid_parameters": {
        "num_nodes": 16,
        "pv_nodes": [1, 2, 3, 4, 6, 8, 9, 10],
        "battery_nodes": [2, 3, 5, 7, 9, 10, 11, 12],
        "cooperative": false,
        "cooperative_nodes": [1, 2, 3, 4]
    }
}

   
   

5.  **Run the simulation**

 ```bash
   julia src/energy_community.jl 
```
6. Directory Structure

    simulation.jl: Main simulation script.
   
    local_market.jl: Local market logic.
   
    output/: Directory for simulation output.
   
   
        images/: Contains simulation output images.

