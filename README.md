# Tensorflow_more

I add more things on tensorflow, such as dropout and use tensorboard to visualization.

## Tensorflow Dropout
I add a dropout probality for hidden layer. This method may help to speed up convergence.

## Tensorflow CNN
I still use the mnist data.

+ input layer : 784 nodes (MNIST images size)
+ first convolution layer : 5x5x32
+ first max-pooling layer
+ second convolution layer : 5x5x64
+ second max-pooling layer
+ third fully-connected layer : 1024 nodes
+ output layer : 10 nodes (number of class for MNIST)
+ for learning rate, I use 0.0001

I also put a GPU version for CNN, we'd better run CNN in GPU, since CPU is so slower.
What we should take care of in GPU is that we can't put use all the data in one time. Since GPU would have out of memroy issue.
For my test, GPU is about 30 times faster than CPU.
My system is: i7-7700k + gtx 1080

## Tensorflow RNN
In the part I use a very simple RNN model.
But I didn't see a boosting in GPU, it is same speed with CPU.
GPU is faster in CNN and DNN in my experience.

## save and restore
Show a example of save and restore the RNN model we trained. We should keep the model structure the same. The NET file the model we saved.

## Tensorflow_quantity
We can also use tensorflow to do quantity prediction. Here I give you small example with two hidden layers.

## google inception

A example to use google inception on your own image. <br />
First download the inception.  <br />
Put your own images in the images folder.  <br />
Here I use four pictures as examples. The inception will return the top 5 categories. <br />
