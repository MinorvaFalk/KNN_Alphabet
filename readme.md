# Alphabet Recognition using MediaPipe

Estimate alphabet hand gesture using MediaPipe + KNN algorithm.
This repository contains : 
- Dataset from [link](https://www.kaggle.com/grassknoted/asl-alphabet) which already converted into landmark.
- Dataset generator (generate landmark dataset from images).
- Notebook for alphabet recognition

# Requirements
- anaconda [link] (https://www.anaconda.com/products/individual)
- mediapipe 0.8.1
- opencv 3.4.2 or Later
- scikit-learn 0.23.2 or Later
- matplotlib 3.3.2 or Later

# Directory
```bash

│   Generate Dataset.ipynb
│   readme.md
│   Visual Programming Project.ipynb
│
├───.ipynb_checkpoints
│       Generate Dataset-checkpoint.ipynb
│       Generate Test-checkpoint.ipynb
│       Visual Programming Project-checkpoint.ipynb
│
├───archive
│   └───asl_alphabet_train
└───Dataset
        hand_dataset.csv
        hand_dataset_100.csv
        hand_dataset_1000_24.csv
        hand_dataset_1000_Z.csv
        hand_dataset_100_24_Z.csv
```

### Generate Dataset.ipynb
Generating dataset from image to landmark in csv.

### Visual Programming Project.ipynb
Training model and recognize alphabet gestures.

### archive
Unzipped folder of dataset. Make sure child directory is the same as above.

### Dataset
- hand_dataset_x_24, contain 24 alphabet dataset (ignoring moving gesture alphabet)
- hand_dataset_x_24_Z, contain 24 alphabet dataset with Z landmark ([check here for Z landmark](https://google.github.io/mediapipe/solutions/hands.html#output))

# Training
1. Importing libraries and defining dataset.
2. Creating Train and Test Data.
3. Creating classifier model for our alphabet recognition.
4. Calculate model accuracy.
5. Show graph for adjusting number of n_neighbors.
6. Intialize Mediapipe Hands for alphabet recognition.