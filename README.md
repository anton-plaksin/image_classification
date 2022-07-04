# Image Classification

The repository present the part of my experience in Image Classification. 

### Classification of CIFAR-10 dataset via deep convalutional neural network

The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images: 

![cifar10_examples](https://github.com/anton-plaksin/image_classification/blob/main/cifar10_via_cnn/pic/cifar10_8examples.png)

We train a neuron network, containing 2 convolutional and 2 dense layers, to classify the images. Our best accuracy on the test dataset is **79.53%**. The loss and accuracy curves are presented below:

![cifar10_via_cnn](https://github.com/anton-plaksin/image_classification/blob/main/cifar10_via_cnn/pic/cifar10_via_cnn.png)

The source code can be found [here](https://github.com/anton-plaksin/image_classification/blob/main/cifar10_via_cnn/cifar10_via_cnn.ipynb)

*TODO: add stop criteria, add the accuracy curve on train dataset, to save the best networks, to use pre-train networks, to use GPU*

### Image Classification of Dogs and Cats via Pre-trained Network

The dataset taken from https://www.kaggle.com/c/dogs-vs-cats contains 25k images of dogs and cats.

![cats_dogs_examples](https://github.com/anton-plaksin/image_classification/blob/main/dogs_cats_via_inception/pic/cats_dogs_examples.png)

Using pre-trained model called inception_v3, we get 1000 features for each image. Then we solve the classification problem by means of Logistic Regression, Ridge Classifier, and Random Forest algorithms. According to the experiments, the best classifier is Ridge Classifier with **0.99%** accuracy.

