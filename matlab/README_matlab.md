Contains neuron and synapse information in MATLAB-readable format. When the archives are unzipped, you will have two files: `neurons.csv` and `J.mat`. 

`neurons = readtable('neurons.csv')` will create a MATLAB table with each row containing single-neuron information.

`load('J.mat')` will produce 7 variables: `J`, the synapse counts between all neuron pairs, and `J_ach`, `J_gaba`, `J_glut`, `J_da`, `J_ser`, `J_oct`, the synapse counts broken down by neurotransmitter type. `J` is the sum of these six matrices. 
