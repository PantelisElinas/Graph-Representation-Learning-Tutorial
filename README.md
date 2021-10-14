# Graph Representation Learning Tutorial

Welcome to the source code repo for Data61's tutorial on Graph Representation Learning. 

Instructions on how to setup your computer and the code to be used during the tutorial will be made available here on **October 16th, 2021**.

Regards,

Pantelis

## Setup Instructions

The code for this tutorial requires Python 3.7 or newer. If you do not have Python installed on you system then please install a suitable version from [python.org](https://www.python.org/). A better and recommended alternative is to install the most current version of the [Anaconda distribution](https://www.anaconda.com/products/individual). The setup instructions assume that you have installed Anaconda.

First, you need to create a new Python virtual environment. We recommend using `conda` for this because it makes it easy to specify the Python version.

> conda create --name grl-course-env python=3.7

Then, activate the new environment.

> conda activate grl-course-env

Check that you are using the correct Python version. The following command,

> python --version

should show `Python 3.7.11` or the most recent `3.7` version available for your OS.

Next, install the required Python libraries using the command,

> pip install -r requirements.txt

If the above fails to install the PyTorch library then please follow the official installation instructions [here](https://pytorch.org/). Similarly for the [Deep Graph Library](https://www.dgl.ai/) follow the official installation instructions [here](https://www.dgl.ai/pages/start.html).

Finally, register your new environment with IPykernel,

> python -m ipykernel install --user --name grl-course-env --display-name "grl-course-env"

## Running the example code

Code examples are provided as Jupyter notebooks. All notebooks are located in the `notebooks` folder. To run the examples first change to the `notebooks` folder using,

> cd notebooks

Then start Jupyter using the following command,

> jupyter notebook

You can now run the examples using your web browser.

## Tutorial description

Networks also known as graphs are fundamental to many aspects of modern society, from the internet, to transport, social networks, energy grids, health, and businesses. To effectively analyse these systems we need a deeper understanding of networks and the techniques available to work with them. Recently, new machine learning methods based on advancements in neural network representation learning have been developed to analyse graphs for prediction, visualisation and decision making. 

This tutorial will give an introduction to machine learning on graphs and more specifically representation learning using graph neural networks (GNNs). We will discuss several state-of-the-art techniques for small and large graphs. We will cover fundamental graph data structures and predictive analytics using manual feature engineering and modern GNNs. Additional topics will include unsupervised, supervised and semi-supervised learning for node clustering, node classification, link prediction and graph property prediction. We are also going to briefly discuss how to scale graph neural networks to huge graphs with billions of nodes. 

Participants will gain experience applying machine learning on graphs solving real-world problems using Python's machine learning modules, [PyTorch](https://pytorch.org/), and the [Deep Graph Library (DGL)](https://www.dgl.ai/). Participants should have a basic understanding of machine learning concepts and Python programming skills.


## Books and Papers

A short (and incomplete) list of survey papers and books listed at no particular order.

1. (survey paper) [Representation Learning on Graphs: Methods and Applications](https://www.thejournal.club/c/paper/130785/) by William L. Hamilton, Rex Ying, and Jure Leskovec, 2017
2. (survey paper) [Graph Learning: A Survey](https://www.thejournal.club/c/paper/344933/) by Feng Xia, Ke Sun, Shuo Yu, Abdul Aziz, Liangtian Wan, Shirui Pan, and Huan Liu, IEEE Transactions on Artificial Intelligence, 2021
3. (survey paper) [Geometric deep learning: going beyond Euclidean data](https://www.thejournal.club/c/paper/106946/) by Michael M. Bronstein, Joan Bruna, Yann LeCun, Arthur Szlam, and Pierre Vandergheynst, IEEE Signal Processing Magazine, 2017 
4. (book) [Graph representation learning](https://www.thejournal.club/c/paper/377948/) by W.L. Hamilton, 2020
5. (book) [Geometric Deep Learning: Grids, Groups, Graphs, Geodesics, and Gauges](https://www.thejournal.club/c/paper/343835/) by Michael M. Bronstein, Joan Bruna, Taco Cohen, and Petar Veličković, 2021
