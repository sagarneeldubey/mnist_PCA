# mnist_PCA
Summary: Application of PCA on mnist data with the aim to a) compress and b) recover comoressed data. 
Description: mnist (http://yann.lecun.com/exdb/mnist/) is a popular handwritten digit database used by in AI/ML academia. Here, we will demonstrate 
the power of PCA in compressing the data by identifying and capturing patterns in it. If you are new to PCA, we suggest going through this manuscript 
by Lindsay Smith. https://ourarchive.otago.ac.nz/bitstream/handle/10523/7534/OUCS-2002-12.pdf?sequence=1&isAllowed=y 

We will use XGBOOST classifier on the full dataset with the aim of determining the possible accuracy (of predicting the digits). We will use this 
accuracy as our benchamrk against all subsequent prediction models. Note that we will run the subsequent prediction models on reduced datasets by using
only a handful of principal components rather than all. We will use the same family of classifiers (XGBOOST) throughout to keep all other aspects constant.

We will see that even when the dataset is by reduced to a third of the original size, the accuracy will reduce by only 3 percentage points. 
