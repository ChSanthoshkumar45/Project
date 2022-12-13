** **Implementation of Traffic Sign Recognition with voice alert using CNN

In this project, I used deep neural networks and three classic convolutional neural network architecture to classify traffic signs. I will train and validate a model so it can classify traffic sign images using the German Traffic Sign Dataset. After the model is trained, I used German Traffic Sign dataset from kaggle.
First we need to import the data 
Import the necessary libraries 
Dependencies
python3.5
matplotlib (2.1.1)
opencv-python (3.3.1.11)
numpy (1.13.3)
tensorflow-gpu (1.4.1)
sklearn (0.19.1)
Need to undergo some pre-processing methods like changing the images to an arrays
I used the numpy library to calculate summary statistics of the traffic signs data set:
Split the data for training and validating the model
using one hot encoding changing the target variables to numerical
The size of training set is: 34799
The size of the validation set is: 4410
The size of test set is: 12630
The shape of a traffic sign image is: (32, 32 ,3)
The number of unique classes/labels in the data set is: 43
![image](https://user-images.githubusercontent.com/110654308/207247647-0846569c-67fc-42d4-904a-3d5813ff26df.png)
Training
I have turned the following two hyperparameters to train my model.

EPOCHS = 20
BATCH_SIZE = 32
It takes about 2 minutes to train the model on GetForce 750 ti.

The results are:

accuracy of training set: 94.6%
accuracy of validation set: 98.0%
plot the graph for loss and accuracy as in epochs
now import the test data from the folder name testcsv
and using accuracy score
accuracy of test set: 95.7%
then import python text to speach recognization library if not install it first
then you can also hear the voice by predicting the image
