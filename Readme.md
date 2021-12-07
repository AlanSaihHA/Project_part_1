# Changes to architecture of TBNN

This program proposes three different new architectures for the neural network designed by [Ling(2016)](https://www.cambridge.org/core/journals/journal-of-fluid-mechanics/article/abs/reynolds-averaged-turbulence-modelling-using-deep-neural-networks-with-embedded-invariance/0B280EEE89C74A7BF651C422F8FBD1EB).

To run this code it is necessary to install some required packages, this is described [here](https://github.com/tbnn/tbnn). The program with the changes is inside the directory “notebooks”, which calls code_for_trainning.

The repository includes three directories:
* Data: The data used for the NN. A channel flow case is used.
* Notebooks: Includes the notebook where the changes were made and the necessary modules to run the program.
* Results: Includes the plots for each case.

Some important parameters are modified from the original code: Number of layers, number of nodes, number maximal of epochs and fraction of data used for training. The values for each setting are

- First structure
    - Number of layers: 5
    - Number of nodes: 25
    - Max. Epochs: 5000
    - Split fraction: 0.9

- Second structure
    - Number of layers: 3
    - Number of nodes: 20
    - Max. Epochs: 3000
    - Split fraction: 0.75

- Third structure
    - Number of layers: 1
    - Number of nodes: 30
    - Max. Epochs: 2000
    - Split fraction: 0.5