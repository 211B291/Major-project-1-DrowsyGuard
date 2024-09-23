# Major-project-1-DrowsyGuard

## Overview
This project implements a *Driver Drowsiness Detection System* using deep learning techniques to prevent accidents caused by driver fatigue. The system monitors the driver's facial expressions and eye movements to detect signs of drowsiness in real-time. If drowsiness is detected, the system triggers an alert, enhancing road safety.

## Features
- *Real-time Detection*: The system processes video feed in real-time and continuously monitors the driver’s face and eyes.
- *Facial Landmark Detection*: Utilizes facial landmark detection to monitor eye closures, yawning, and other facial indicators of drowsiness.
- *Deep Learning Models*: Powered by Convolutional Neural Networks (CNNs) for detecting eye states (open or closed).
- *Alert System*: Generates a warning alert (audio or visual) when drowsiness is detected.

## Dataset
The project uses the *MRL Eyes Dataset (mrlEyes_2018_01)* to train the deep learning model. The dataset contains thousands of images of human eyes in various states (open, closed, and partially open). The model is trained to classify eye states based on these images, enabling it to detect drowsiness in real-time.

> *Note*: The mrlEyes_2018_01 dataset is excluded from this repository. You can download it from the [official source](http://mrl.cs.vsb.cz/eyedataset).

## Project Structure

```plaintext
driver-drowsiness-detection/
│
├── models/
│   ├── trained_model.h5        # Pre-trained model (if available)
│
├── src/
│   ├── detect_drowsiness.py    # Main script for detecting drowsiness
│   ├── train_model.py          # Script to train the model on the dataset
│   ├── utils/
│   │   └── preprocess.py       # Data preprocessing utilities
│
├── data/
│   └── mrlEyes_2018_01/        # Folder for storing the dataset (ignored by Git)
│
├── requirements.txt            # Python dependencies
├── README.md                   # Project documentation
├── .gitignore                  # Specifies files/folders to be ignored by Git
└── LICENSE                     # License information
