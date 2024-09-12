# Power-Aware Deep Unfolding Learned Optimization for Modular Receive Beamforming

This repository contains the source code for simulations and experiments presented in the paper **[Rapid and Power-Aware Learned Optimization for Modular Receive Beamforming](https://arxiv.org/pdf/2408.00439)**.

## Paper Link
Access the full paper on ArXiv: [arxiv.org/2408.00439](https://arxiv.org/pdf/2408.00439)

## Overview
This repository includes the code and results for the experimental study described in **Section V** of the paper. 

Some simulations require external data, specifically generated using the **QuDRiGA channel generator**. The relevant data file, `H_1100_32_12_5`, is provided as a MATLAB file, representing the matrix H with:
- 1100 samples of 32 frequency bins
- MIMO channel realizations with 12 antennas and 5 users

Note: In our simulations, only 4 of the 32 frequency bins were used.

## Contents

The simulations are structured into multiple Jupyter Notebooks, each corresponding to different sections of the study:

### 1. **Notebook 1** - Unconstrained Simulations
- Contains simulations for **Scenario 1** and **Scenario 2**.

### 2. **Notebook 2** - Model Training & Transfer
- Example of training the model on **Scenario 4** and evaluating on a different scenario with more users (**Scenario 3**).
- Includes a **parameter comparison** between the CNN network and the unfolded network.

### 3. **Notebook 3** - Model Training on Different Antenna Configurations
- Example of training on **Scenario 5** and testing on a different configuration with more antennas and panels (**Scenario 6**).

### 4. **Notebook 4** - Power-Aware Sparse Beamforming
- Demonstrates the power-aware implementation of sparse beamforming.

### 5. **Notebook 5** - Power-Aware Quantized Beamforming
- Shows results of quantized low-resolution beamforming using our algorithms.

### 6. **Notebook 6** - Runtime Analysis
- Provides an analysis of the running time of different benchmarks, specifically on **Scenario 2**.

## External Data Requirements
For some simulations, you will need the QuDRiGA-generated channel data. The dataset is provided as `H_1100_32_12_5.mat`. Ensure that the file is placed in the appropriate directory before running the simulations.

## Citation
If you use this code or data in your research, please cite our paper:

```bibtex
@misc{levy2024rapidpowerawarelearnedoptimization,
      title={Rapid and Power-Aware Learned Optimization for Modular Receive Beamforming}, 
      author={Ohad Levy and Nir Shlezinger},
      year={2024},
      eprint={2408.00439},
      archivePrefix={arXiv},
      primaryClass={eess.SP},
      url={https://arxiv.org/abs/2408.00439}, 
}
```
