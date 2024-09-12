# Power-Aware-Deep-Unfolding-Learned-Optimization-for-Modular-Receive-Beamforming

Source code for the results and simulations described in the paper "Rapid and Power-Aware Learned Optimization for
Modular Receive Beamforming".

link to arxiv paper:

arxiv.org/pdf/2408.00439

Some of the simulatons require external data. To this end, the QuDRiGA channel generator was used. The data file named "H_1200_32_12_5" is attached is MATLAB files.
The name indicated that the file contains the matrix H, with 1200 samples of 32 frequncy bins channel realizations, of a MIMO channel with 12 antennas and 5 users.
In our simlulations, not all 32 frequency bins were used, but only 4.

In this repo, the relevant simulations for the Experimental study (Section V in the paper) can be found.

Notebook 1 contains the unconstrained simulations - Scenarions 1 and 2.


Notebook 2 contains the example of training the model on a certain scenario (e.g. Scenario 4) and the inspecting its results on a different scenraio, with more users (e.g. Scenario 3). This notebook also contains a chapter of parameters count, comparing the number of parameters between the CNN network, and the unfolded network.


Notebook 3 contains the example of training the model on a certain scenario (e.g. Scenario 5) and the inspecting its results on a different scenraio, with more antennas and panels (e.g. Scenario 6)

Notebooks 4 and 5 show the results of power aware implementations of our algorithms, where the the first shows sparse beamforming, and the latter shows quantized low-resolution beamformers.

Notebook 6 provides an analysis of running time of defferent benchmarks running on Scenario 2.
