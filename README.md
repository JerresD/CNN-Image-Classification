# Image Classification for Hand Signs: Rock Paper Scissors Using CNN

## Problem Statement
Whether in childhood or now, hand games are what we use to bond when we're bored. It is also a trick similar to the turntable of fate. What if AI technology is applied to hand games? For example, when we want to decide 'yes' or 'no', in addition to flip a coin, we can choose to play rock-paper-scissors to battle with AI.Therefore, our goal is to develop a neural network model that could predict hand gestures corresponding to rock, paper, or scissors based on input images. By utilizing a dataset consisting of labeled images of hand gestures, the model will be trained to accurately identify and classify the hand gesture made by a player.

# Let's Start Building A CNN Model for Image Classification

# Data Preparation

CNN (Convolutional Neural Networks) is one of the best suited approach for image classification as it is able to learn the spatial hierarchies of features to avoid loss of information. Therefore, we are trying to get use CNN algorithm to classify image for hand signs: rock, paper and scissors.

### Data Description
We will be using Rock-Paper-Scissors Images dataset from [Kaggle](https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors/code?datasetId=107582&sortBy=voteCount) which consists of:
- 712 paper images
- 726 rock images
- 750 scissor images.

The dataset directory is now hosted on Google Cloud Storage. So for data preparation, the program will:
- download dataset directory and extract it automatically.
- divide dataset into 60% training sets and 40% validation sets.
- train model within 20 minutes
- have approximately 97% of accuracy of trained model

# Import Neccessary Libraries and Image Preprocessing

The images have been rescaled, rotated, enlarged, etc before splitting the data. Then, it will divide the dataset into 60% training sets and 40% validation sets.

> import os
> import pathlib
