# Fashion-MNIST
My try on the MNIST Dataset achieving a train accuracy of 98.5% and test accuracy of 93%

**About the Model**

The model is a single layer CNN (Conv2D) which takes input tensors of dimensions (image_height, image_width, image_channels) which is **(28,28,1)** which is the format of Fashion-MNIST dataset.

Layer 1 : Conv2D for convolution operation to extract features.

Layer 2 : MaxPooling2D to reduce dimension complexity and reduce training params

Layer 3 : BatchNormalization is used to normalize the output of the previous activation layer

Layer 4 : Dropout Layer to reduce overfitting

Flatten() is added to make the outout from 3D to 1D

Layer 5 and 6 : Dense Layers to process the output and finally pass the 10 labels for output and applying softmax activation

**Results**

Training Accuracy : `98.5%`

Test Accuracy : `93%`
