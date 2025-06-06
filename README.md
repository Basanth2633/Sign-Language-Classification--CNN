Objective:
Build a CNN model to classify American Sign Language (ASL) hand gestures (A–Z) using the Sign Language MNIST dataset.

Data Source:

Training & validation data are CSV files containing pixel values of 28×28 grayscale images and corresponding labels.

Data Preprocessing:

Parsed CSV into image arrays and labels using numpy.

Reshaped images to 28×28 format.

Normalized pixel values (0–255 → 0–1).

Augmented training images using ImageDataGenerator (rotation, shift, zoom, flip).

Visualization:

Displayed sample training images with labels.

Plotted histogram and count plot to check class distribution.

Model Architecture:
A custom CNN built using Keras Sequential API:

Conv2D → MaxPooling2D

Conv2D → MaxPooling2D

Flatten → Dense(512) → Dense(26 with softmax)

Training Details:

Optimizer: Adam

Loss: Sparse Categorical Crossentropy

Metric: Accuracy

Trained for 30 epochs with batch size 32.

Output:

Model predicts one of 26 letters based on hand gesture input.

Achieves good classification performance using basic CNN layers.
