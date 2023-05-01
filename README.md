# pytorch-vggnet16

OVERVIEW
This project aims to implement VGGNet, a deep convolutional neural network (CNN) architecture, using the PyTorch framework from scratch. The objective is to efficiently use the PyTorch framework and create a model without using any pre-trained models.

STRUCTURE
The project contains the following files:

model.ipynb
README.md - A detailed description of the project, how to run the code, dependencies, and reference materials.

DEPENDENCIES
This project requires the following dependencies to be installed:

Python 3.6 or later
PyTorch 1.8.0 or later
Torchvision 0.9.0 or later
NumPy 1.19.5 or later

DATASET
The dataset used for this project is taken from kaggle. its a dataset with 8 classes each representing an individual avenger. it contains a training and testing set of data. However due to the huge time it took me to train the model I had to cut the dataset to contain only 2 classes. the details of the number of images for each set can be found in the code.

INFERENCES
since the model is a very deep neural network with 16 layers it has a lot of parameters to tune. so it took a very long time to trian just one epoch(45mins) approx.
finally i was able to reduce the dataset size and it took 3.5 hrs to finish 10 epochs. <img width="1363" alt="Screenshot 2023-05-01 at 10 09 30 PM" src="https://user-images.githubusercontent.com/105579183/235492727-a1b918c8-d52e-49ac-8110-364de10be59f.png">
in some epochs the train accuracy was more than the test accuracy which is indicative of overfitting
to prevent overfitting its necassary to add more data so that a very complex model like vgg16 can be trained properly.
i also added batchnormaliation layers to normalize the input to every layers and reduce overfitting.
trivial augment wide function was also incorporated to increase the randomness of the training set and reduce overfitting.



