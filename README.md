# MetaClassifier-for-FCNNs
In this project a meta classifier is built. It takes the features of pytorch fully connected neural networks as inputs, and makes inferrence about whether the original training data contains a certain property.This implementation is practical in a federated learning process. When a malicious party is trying to steal information from the classifiers, this kind of meta classifier is in the common use.


It's the very first stage of my master thesis project. And for now I'm trying to realize what they did in [this paper](https://dl.acm.org/doi/abs/10.1145/3243734.3243834). They use the US Census data from <http://archive.ics.uci.edu/ml/datasets/Census+Income>. The neural networks are of 3 hidden layers of sizes 32, 16 and 8, to do a binary classification task. Adam optimizer is used, with ReLu as the activation function, a learning rate of 0.001, a weight decay of 0.01 and 40 maximum epochs of training. 

2048 such FCNNs are trained with the original distributed data and other 2048 are trained with data of 65% are women. Then I'll get the feature vectors of those FCNNs and use them to train a meta-classifier. The meta-classifier is trained to infer whether the training data of FCNNs is unbalanced distributed.



