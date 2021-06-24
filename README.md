# kron
Heuristic for Direct Product Graph Decomposition - Kronecker factorization

This software implements a heuristic for decomposing a directed graph into factors according to the direct product (also known as Kronecker, cardinal or tensor product). Given a directed, unweighted graph G with adjacency matrix Adj(G), our heuristic searches for a pair of graphs G1 and G2 such that G = G1×G2, where G1×G2 is the direct product of G1, G2. The heuristic relies on graphs' adjacency matrices.

Specifically, this software generates two random binary matrices B and C and a matrix A = B ⊗ C. A random permutation is applied to A, resulting in A'=PᵀAP. The program then looks for a permutation P' such that P'ᵀA'P' = B' ⊗ C'. By construction, it is evident that at least one feasible factorization exists.

The repository contains two files:

1- kron.mlapp: a MATLAB implementation of the heuristic providing a GUI
2- kron.txt: the source code of the application
