# Fashion-MNIST with Pytorch
Building a neural network classifier using Fashion MNIST dataset and Pytorch.

# The Background
## Original MNIST
The original [MNIST](http://yann.lecun.com/exdb/mnist/) is a dataset of handwritten digits which contains 60,000 training images and 10,000 test images, each of size 28x28. MNIST is widely regarded as the "hello world" of deep learning and is often the starting place for many people who are new to deep learning to start building their first neural networks.

![MnistExamples](https://user-images.githubusercontent.com/53375807/123830693-29996900-d921-11eb-81e2-d6960d7ea00c.png)

*MNIST visualisation Source : [Wikipedia](https://en.wikipedia.org/wiki/MNIST_database)*

## Fashion MNIST
More recently, researchers at Zalando have developed a dataset [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist), intended to be a drop-in replacement for the original MNIST.

![fashion-mnist-sprite](https://user-images.githubusercontent.com/53375807/123830674-256d4b80-d921-11eb-814f-d8f8ee6c8f85.png)

*Fashion MNIST visualization (by Zalando, MIT License).*

This dataset also contains 60,000 training images and 10,000 test images, and has similar structure in train/test split as the original MNIST. Here, the 10 classes correspond to 10 different articles of clothing.

# Model
## Convolutional Neural Network (CNN)
Convolutional Neural Networks are excellent NN architectures to apply to computer vision tasks. CNNs have been proven to be very effective effective for image recognition, object recognition, and even natural language processing tasks. An excellent description on CNNs can be found in [Stanford's CS231n course notes](https://cs231n.github.io/convolutional-networks/):

We use the data set with  CNN model is based on the ResNet architecture with 18 layers.

![f941fa481a9d8987b5022f1a8bade653](https://user-images.githubusercontent.com/53375807/123834028-9b26e680-d924-11eb-9d9c-8299b87d2e92.png)

*Resnet-18 architechture implementation on [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html).*

## Hyperparameters

The model performance was comapred on different batch sizes of {64,256,512} images with learning rate set to 0.01 and 50 epochs.

# Performance

###Legend

![Screenshot (25)](https://user-images.githubusercontent.com/53375807/123836356-3d47ce00-d927-11eb-8fe7-f21c443e6f3a.png)

##Accuracy

![Accuracy](https://user-images.githubusercontent.com/53375807/123836406-4df84400-d927-11eb-8ed6-2260ea0351d5.png)

###Loss

![Loss](https://user-images.githubusercontent.com/53375807/123836402-4cc71700-d927-11eb-85fe-95b5eae22c93.png)


