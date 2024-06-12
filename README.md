# PRODIGY_ML_04
**Leap Gesture Recognition with Convolutional Neural Network**


This repository contains code for training and evaluating a Convolutional Neural Network (CNN) model for Leap Gesture Recognition. The model is trained to recognize various hand gestures captured using the Leap Motion sensor.

**Dataset**


The dataset used for training consists of images of hand gestures categorized into different classes. The images are grayscale and resized to a uniform size of 50x50 pixels. The dataset is structured in the following directory format:


input/
└── leapGestRecog/
    ├── 00/
    ├── 01_palm/
    ├── 02_l/
    ├── 03_fist/
    ├── 04_fist_moved/
    ├── 05_thumb/
    ├── 06_index/
    ├── 07_ok/
    ├── 08_palm_moved/
    ├── 09_c/
    └── 10_down/

    
**Model Architecture**


The CNN model architecture is as follows:


Convolutional layer with 32 filters and a kernel size of (3,3), followed by ReLU activation.

Convolutional layer with 32 filters and a kernel size of (3,3), followed by ReLU activation, max pooling, and dropout (30%).

Convolutional layer with 64 filters and a kernel size of (3,3), followed by ReLU activation, max pooling, and dropout (30%).

Flatten layer to convert the output to 1D.

Fully connected dense layer with 256 neurons and ReLU activation.

Output layer with 10 neurons and softmax activation.


**Training**


The model is compiled using sparse categorical crossentropy loss and the RMSprop optimizer. It is trained for 7 epochs with a batch size of 32. The training and validation accuracy and loss are monitored during training.

Evaluation
The model achieves a test accuracy of 99.98%. The loss and accuracy plots for both training and validation data are visualized.

Confusion Matrix
A confusion matrix is generated to visualize the model's performance on different classes of hand gestures.**
