# Bird Species Detection using TensorFlow Object Detection API
This project is about detecting species of birds using Convolutional Neural Networks architectures. The dataset I used has 2400 total images with 800 images per class of 3 classes of birds species. These classes are TurdusMerula, ErithacusRubecula and PeriparusAter. These images are tagged using Renom Tag annotation tool. The TFRecords were created using the images and XML files and then fed into the model for training. I used Faster R-CNN and SSD ResNet50 for training. Faster R-CNN is a powerful state of the art model with good performnce and accuracy. But because of its power its slow in detecting from videos and in real time. I also trained an SSD ResNet50 which is a faster model but the accuracy is less. 

For both the models I checked the evaluation metrics and choose the better model for deployment and inferencing.

The whole project is distributed into 5 juyter notebooks, they are preprocessing.ipynb, training.ipynb, evluation.ipynb, tensorboard.ipynb, inference.ipynb. Please refere to the notebooks for more details. The notebooks should be followed in the following order.
1. preprocessing.ipynb
2. training.ipynb
3. evluation.ipynb
4. tensorboard.ipynb
5. inference.ipynb

## Installation
To run the jupyter notebooks and code files of this repository, TensorFlow object detection API ia required. Please follow the official documentation to install it, the link is given below. 

https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html

After the installation this repository can be used for running the codes.

## Dataset
The dataset was provided by the Liverpool John Moores University. This was a university project. The dataset contains of total 2400 images of three different classes of birds with 800 images in each class. The three classes of birds are TurdusMerula, ErithacusRubecula and PeriparusAter. The collage of some images from the dataset is given below.
![Picture1](https://user-images.githubusercontent.com/30217266/194096203-94c174bd-151c-4203-9f57-a0b3baadfce1.jpg)

## Pre-processing
The preprocessing.ipynb notebook contains the pre-processing steps that were taken before training the models. Some of the steps performed were cleaning of the data, visualising the resoltion of the images, and removing the No Good images from the directory.

## Training
The training.ipynb notebook contains the creation of TF records, setting up the hyperparametrs, training of the models, and exporting the trained inferfence graph. 

## Evaluation
The evaluation.ipynb notebook contains the models evaluation results and their corresponding tensorboard plots. 

## Tensorboard
The tensoroard.ipynb notebook contains the commands to run the tensorboard and plots of losses during training of the both the models. 

## Inference
The inference.ipynb notebook contains the inference results and the steps to perform inference using the models. Screenshot of some inference results are given below.
![Screenshot_4](https://user-images.githubusercontent.com/30217266/194104228-27c132d4-f33a-4980-b389-75ff718b0aa0.png)

