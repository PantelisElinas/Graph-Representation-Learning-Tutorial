# Graph Representation Learning Tutorial

Welcome to the source code repo for Data61's tutorial on Graph Representation Learning. 

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


## Books and Papers: General

A short (and incomplete) list of survey papers and books listed at no particular order.

1. (survey paper) [Representation Learning on Graphs: Methods and Applications](https://www.thejournal.club/c/paper/130785/) by William L. Hamilton, Rex Ying, and Jure Leskovec, 2017
2. (survey paper) [Graph Learning: A Survey](https://www.thejournal.club/c/paper/344933/) by Feng Xia, Ke Sun, Shuo Yu, Abdul Aziz, Liangtian Wan, Shirui Pan, and Huan Liu, IEEE Transactions on Artificial Intelligence, 2021
3. (survey paper) [Geometric deep learning: going beyond Euclidean data](https://www.thejournal.club/c/paper/106946/) by Michael M. Bronstein, Joan Bruna, Yann LeCun, Arthur Szlam, and Pierre Vandergheynst, IEEE Signal Processing Magazine, 2017 
4. (book) [Graph representation learning](https://www.thejournal.club/c/paper/377948/) by W.L. Hamilton, 2020
5. (book) [Geometric Deep Learning: Grids, Groups, Graphs, Geodesics, and Gauges](https://www.thejournal.club/c/paper/343835/) by Michael M. Bronstein, Joan Bruna, Taco Cohen, and Petar Veličković, 2021

## Papers: Tutorial Part I

1. [Laplacian Eigenmaps and Spectral Techniques for Embedding and Clustering
](https://www.thejournal.club/c/paper/384453/), M. Belkin and P. Niyogi, NeurIPS 2001
2. [Deepwalk: Online learning of social representations](https://www.thejournal.club/c/paper/54593/), B. Perozzi, R. Al-Rfou, and S. Skiena, KDD 2014
3. [node2vec: Scalable feature learning for networks](https://www.thejournal.club/c/paper/97424/), A. Grover and J. Leskovec, KDD 2016
4. [metapath2vec: Scalable Representation Learning for Heterogeneous Networks](https://www.thejournal.club/c/paper/290795/), Y. Dong, N.V. Chawla, and A. Swami, KDD 2017

## Papers: Tutorial Part II

1. [Convolutional Neural Networks on Graphs with Fast Localized Spectral Filtering](https://www.thejournal.club/c/paper/97237/), M. Defferrard, X. Bresson, and P. Vandergheynst, NeurIPS 2016
2. [Semi-Supervised Classification with Graph Convolutional Networks](https://www.thejournal.club/c/paper/101516/), T.N. Kipf and M. Welling, ICLR 2017
3. [Graph Attention Networks](https://www.thejournal.club/c/paper/134548/), P. Velickovic, G. Cucurull, A. Casanova, A. Romero, P. Lio, and Y. Bengio, ICLR 2018
4. [Simplifying Graph Convolutional Networks](https://www.thejournal.club/c/paper/187881/), F. Wu, T. Zhang, A.H. de Souza, C. Fifty, T. Yu, K.Q. Weinberger, ICML 2019
5. [Predict then Propagate: Graph Neural Networks meet Personalized PageRank](https://www.thejournal.club/c/paper/172090/), J. Klicpera, A. Bojchevski, and S. Günnemann, ICLR 2019
6. [Inductive Representation Learning on Large Graphs](https://www.thejournal.club/c/paper/122200/), W.L. Hamilton, R. Ying, and J. Leskovec, NeurIPS 2017
7. [Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional Networks](https://www.thejournal.club/c/paper/200627/), W. Chiang, X. Liu, S. Si, Y. Li, S. Bengio, and C. Hsieh, KDD 2019
8. [GraphSAINT: Graph Sampling Based Inductive Learning Method](https://www.thejournal.club/c/paper/209589/), H. Zeng, H. Zhou, A. Srivastava, R. Kannan, and V. Prasanna, ICLR 2020
9. [Representation Learning on Graphs with Jumping Knowledge Networks](https://www.thejournal.club/c/paper/157808/), K. Xu, C. Li, Y. Tian, T. Sonobe, K. Kawarabayashi, and S. Jegelka, ICML 2018
10. [Self-Attention Graph Pooling](https://www.thejournal.club/c/paper/196055/), J. Lee, I. Lee, and J. Kang, ICML 2019
11. [Hierarchical Graph Representation Learning with Differentiable Pooling](https://www.thejournal.club/c/paper/159426/), R. Ying, J. You, C. Morris, X. Ren, W.L. Hamilton, and J. Leskovec
12. [How Powerful are Graph Neural Networks?](https://www.thejournal.club/c/paper/170569/), K. Xu, W. Hu, J. Leskovec, S. Jegelka, ICLR 2019
13. [Principal Neighbourhood Aggregation for Graph Nets](https://www.thejournal.club/c/paper/257161/),G. Corso, L. Cavalleri, D. Beaini, P. Liò, P. Veličković, NeurIPS 2020
14. [Deep Sets](https://www.thejournal.club/c/paper/115378/), M. Zaheer, S. Kottur, S. Ravanbakhsh, B. Poczos, R. Salakhutdinov, A. Smola, NeurIPS 2017