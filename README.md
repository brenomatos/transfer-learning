# Transfer Learning


In this repository You'll find a machine learning task that consists in comparing three strategies for training CNNs on a image classification problem, with two of those strategies using Transfer Learning.

Transfer learning or inductive transfer is a research problem in machine learning that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem.

Here, we use the the [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) dataset, which consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.

First, we split the dataset into two groups A and B. the latter contains classes 0 and 7 and the former contains the remaining classes. Then, 4 models are created:
* CNN with dataset A: Train a CNN from scratch using the A dataset.

Then, we test three strategies to train a model using the B dataset:
* No Transfer Learning: Train the network from scratch, initialising the weights randomly.
* Fine-tuning in one layer: Use the weights of the network trained for part A and fine-tuning
in the last Fully Connected layer.
* Fine-tuning in two layers: Use the weights of the network trained for part A and fine-tuning
in both Fully Connected layers.
<!-- Transfer learning assignment from Machine Learning class @ UFMG. If You want further description for the assignment, you can read the assignment's description [here](SpecificationTP2.pdf). -->

# Jupyter Notebook
In this repo, You'll find both a jupyter notebook and a regular python scipt. You can choose which to use, given your application. However, the jupyter notebook
contains analisys regarding the methods used, along with code and graphs.

# Graphs Examples
Here are some examples of graphs created using code in this repository

### Each Model
For every model created, we can compare accuracy and loss for train/test:
![Train/Test Acc](/images/traintestacc.png "Acc Graph")
![Train/Test Loss](/images/traintestloss.png "Loss Graph")


Also, for every model, a Acc/Loss comparison graph is created:

![Test Acc/Loss](/images/testaccloss.png "Test Acc/Loss")


### All Models
We also plot graphs comparing all models. For train/test, we plot accuracy and loss for all models, as examplified below:

![Train Acc All](/images/trainaccall.png "All Train Acc")
![Train Loss ALl](/images/trainlossall.png "All Train Loss")
![Test Acc All](/images/testaccall.png "All Test Acc")
![Test Loss All](/images/testlossall.png "All Test Loss")
# Built With
[Keras](https://keras.io)

[Seaborn](https://seaborn.pydata.org)

[Pandas](https://pandas.pydata.org/)

[Scikit Learn](https://scikit-learn.org)
