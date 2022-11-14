# Deeplearning-lab2

In the first application we build image classifier from scratch on the Kaggle Cats vs Dogs dataset without applying 
any pre-made Keras application model. We also used data augmentation to increase the size of our data set and 
Keras preprocessing layers for image standarization.

In the second example we build an image classification model using BigTransfer which is transfer learning method for classifing 
images. The hyperparameters are simplified compared to the classic image classification model ( logistic regression for exemple
). We can train large supervised datasets ( labelled data sets) and fine-tuning the model on a target task but the main thing 
is the normalization layers ( data preprocessing ) and scaling the architecture capacity. This two who differs from a model to 
an other.

In exemple N°3 we have first of all prepared the data that we will work with and setting the hyperparameter for the builded model. Because our data is not big, and for training our model we need huge number of images to give us good results, there is a technique called data augmentation so we will try to apply that to our dataset. What data augmentation do is random horizontal flipping or small random rotations.
Second we implements three modern attention-free, multi-layer perceptron (MLP) based models for image classification :
1-The MLP-Mixer model
2-The FNet model
3-The gMLP model
The purpose is not to compare between them and theire performances but to practice the implementation of their main building blocks and how they works.

In example N°4 we build a simple image recognition using The MNIST database of handwritten digits.
we have import the dataset from keras library and split it into train/test sets then normalize each pixel in our images by deviding it by 255. so each pixel will be a number in [0,1] and that fast up training the model.
as activation function we used relu in hidden layer and softmax in output layer.
The model is evaluated by the accuracy method.

In the last exemple we have build and trained a handwriting recognition model with variable-length sequences to the IAM Dataset.
This dataset is similar to the famous MNIST dataset but this one contains image of some handwritten text and not numbers.
What the model need to do is to recognize and rewrite the text shown in the image.
we have choosed as Edit Distance as a metric for evaluating because we are using OCR models.
