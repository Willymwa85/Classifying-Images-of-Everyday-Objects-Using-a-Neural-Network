# Classifying-Images-of-Everyday-Objects-Using-a-Neural-Network
Exploring the CIFAR10 Dataset
The CIFAR10 dataset contains 50,000 training images and 10,000 test images, divided into 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, and truck). Each image is a 3-channel (RGB) color image with a size of 32x32 pixels.

Base Model Architecture

The base model architecture consists of the following layers:

Flatten layer
Fully connected layer with 512 units, ReLU activation, and 20% dropout
Fully connected layer with 256 units, ReLU activation, and 20% dropout
Output layer with 10 units (one for each class)

Training Process

The model was trained using the following hyperparameters:

Learning rates: [0.1, 0.05, 0.01, 0.005]
Number of epochs: [10, 10, 10, 10]
The training process involved multiple phases, adjusting the learning rate after each phase based on the validation loss and accuracy.

Results

The final test accuracy achieved by the model was 0.5178 (51.78%), with a test loss of 1.3442.

Model Saving

The trained model weights were saved to the file 'cifar10-feedforward.pth' for future use.

Hyperparameter and Metric Logging

The hyperparameters (architecture, learning rates, and number of epochs) and metrics (test loss and test accuracy) were logged using the Jovian library for tracking and comparison purposes.

Continued Experimentation

The report encourages further experimentation with different network architectures and hyperparameters to improve the model's performance on the CIFAR10 dataset. It also suggests applying the same training pipeline to different datasets or writing a blog post to articulate the learnings and insights gained from the process.
