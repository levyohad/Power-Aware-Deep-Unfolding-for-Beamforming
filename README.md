# Power-Aware-Deep-Unfolding-Learned-Optimization-for-Modular-Receive-Beamforming

Source code for the results and simulations described in the paper "Rapid and Power-Aware Learned Optimization for
Modular Receive Beamforming".

link to arxiv paper:

arxiv.org/pdf/2408.00439

Some of the simulatons require external data. To this end, the QuDRiGA channel generator was used. The data file named "H_1200_32_12_5" is attached is MATLAB files.
The name indicated that the file contains the matrix H, with 1200 samples of 32 frequncy bins channel realizations, of a MIMO channel with 12 antennas and 5 users.
In our simlulations, not all 32 frequency bins were used, but only 4.

The simluations were conducted usind pytorch version 1.13, so each code starts with installing the correct version.
