# Emoji Recognition
Emoji detection using hand gestures.

Used contour detection for Emoji Recognition using hand gestures.

Used 12 emojis to classify hand gesture.
Emoji dataset can be downloaded from https://www.kaggle.com/eliasdabbas/emoji-data-descriptions-codepoints?select=Screen+Shot+2019-04-04+at+12.59.10+AM.png

Procedure :-
1. Create hand gestures dataset using Create_Dataset.ipynb
2. Create ".csv" file for all hand gestures using Create_csv.ipynb
3. Train our model using Training.ipynb
4. Run Emoji detection using Emoji_Detection.ipynb

Methodology :-

Creating hand gesture dataset
Used webacam to captue hand gestures.
Detected hand colors using cv2.inRange().
Detected contours of hand gestures and captured 1000 images of each classes.

Creating csv file for gesture dataset
Converted images in array using np.asarray()
added class number in the first column of the dataframe
and stored in a csv file.

Pre-processing of data
Imported teh dataset
Shuffled all the rows in our dataset.
And sliced the Data and class labels from our dataset.

Then, we split the data and labels into training and testing part
To feed our labels to our model, one-hot encode them.

Building the model
After preparing our data
We will build our CNN based Deep Neural Network using Keras library.
After building our model
Compile our model with
Loss = "Categorical_Crossentropy"
Optimizer = "Adam"

Training the model
Then we will train our model on prepares Data and labels.
We acheived 99.96% traning accuracy.

Saving the Model
Then we will save our model for future use.

Then Emoji_recognition.ipynb to runn our real time model.
A sample of our model is shown below :-

[![SC2 Video](https://github.com/gearhead0909/Emoji-Recognition/blob/master/Emoji%20Recognition.mp4)]
