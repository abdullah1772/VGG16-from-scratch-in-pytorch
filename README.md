# VGG16-from-scratch-in-pytorch

For this classification problem I am going to implement a CNN based deep learning classification model from scratch in PyTorch. I’ll be using VGG16 to perform image classification on MNIST Fashion Dataset.

Fashion-MNIST is a dataset of Zalando's article images. There are a total of 60,000 images divided into 10 classes overall. Each image consists of 28x28 grayscale image.

VGG focuses on another crucial aspect of Convolutional Neural Networks (CNNs), depth. It was developed by Simonyan and Zisserman. It normally consists of 16 convolutional layers but can be extended to 19 layers and has another variant called VGG19. All the convolutional layers in the neural network consists of 3x3 filters.
Let’s look at the architecture of this network.

![image](https://user-images.githubusercontent.com/88187437/215269944-7565a834-ee12-482d-9833-7ba5d6631604.png)

As you can see the image enters the neural network, goes through multiple layers of convolutions and max pooling, with each convolution layer followed by a relu layer. After performing convolutions on the image we apply max pooling layer on the input image. At the end we have 3 fully connected layers, each containing a dropout layer, a linear layer and a relu activation function.

