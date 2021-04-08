# MetaClassifier-for-FCNNs
In this project a meta classifier is built. It takes the features of pytorch fully connected neural networks as inputs, and makes inferrence about whether the original training data contains a certain property.

This implementation is practical in a federated learning process. When a malicious party is trying to steal information from the classifiers, this kind of meta classifier is in the common use.


This is the very first stage of my master thesis project. And for now I'm trying to realize what they did in [this paper](https://dl.acm.org/doi/abs/10.1145/3243734.3243834).


The data is from <http://archive.ics.uci.edu/ml/datasets/Census+Income>.
