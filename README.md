# Image Classification on CIFAR-100 dataset
This is an implementation of Convolutional Neural Networks in Tensorflow to classify images in the CIFAR-100 dataset. Consult the jupyter notebook named cifar-100_cnn.ipynb for the complete breakdown of the training procedure. There is also a comparison made between the performance of decision trees, random forest and CNNs for this task, CNNs outperform heavily even without proper preprocessing methods.

## Dataset 
The CIFAR-100 dataset consists of 100 classes containg 600 images each. There is another variant of the dataset, the more popular and simpler dataset - CIFAR-10. More details about these datasets can be found on https://www.cs.toronto.edu/~kriz/cifar.html

## Preprocessing techniques
### Data Augmentation
The data augmentation process involves random image rotation, translation and horizontal flips to the dataset, generating data that is more varied than the original dataset. This helps in making the model inference translational and rotational invariant.

### ZCA Whitening
The ZCA whitening process results in a  whitened image that consists of decorrelated features making it easier for the model to learn the important features for a given image class.

## Observations
It is observed that a deep learning model with only 3 convolutional layers and 358,100 parameters can produce an accuracy of 64% on the image classification task. This showcases the prowess of proper pre-processing techniques applied to the training data.

