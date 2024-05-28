# GLCPN
This is the supplementary file, PyTorch implementation, and prepared datasets for the paper entitled “Graph Linear Convolution Pooling for Learning in Incomplete High-Dimensional Data”. 

## GLCPN-Supplementary File.pdf
The supplementary model discussions including proofs, details of experimental settings, additional experimental results are put into this file and cited.

## GLCPN-Codes.zip
This is the PyTorch implementation for our proposed GLCPN model.

We implement all the experiments in Python 3.7, and deploy them on a server with one 2.4-GHz Intel Xeon 4214R CPU, four NVIDIA RTX 3090 GPUs, and 128-GB RAM. 
We may create an environment using: `conda create --name <env> --file requirements.txt`, or install the required packages using: `conda install --file requirements.txt`

## GLCPN-Datasets.zip
This file contains all the prepared datasets used in our paper. 

- [T-208964](https://version-12-0.string-db.org/organism/208964), [T-227321](https://version-12-0.string-db.org/organism/227321), [T-9544](htt ps://version-12-0.string-db.org/organism/9544), and [T-9796](https://version-12-0.string-db.org/organism/9796) are undirected PPI networks gathered from the protein interactome database STRING [1], [2]. They respectively record the protein-protein interactions for the species Macaca mulatta, Equus caballus, Pseudomonas aeruginosa, and Aspergillus nidulans. In a PPI network, the nodes represent specific proteins, the edges represent the observed protein-protein interactions, and the weights represent the confidences of interactomes between proteins. All the weight values have been normalized to the range between 0 and 1. T-208964 consists of 5,565 proteins and 1,559,616 interactomes; T-227321 consists of 7,963 proteins and 1,120,030 interactomes; T-9544 consists of 20,462 proteins and 15,597,778 interactomes; and T-9796 consists of 19,664 proteins and 12,149,608 interactomes. Their densities are respectively 5.04%, 1.77%, 3.73%, and 3.14%.
