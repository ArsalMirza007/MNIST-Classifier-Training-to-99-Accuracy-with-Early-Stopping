# MNIST-Classifier-Training-to-99-Accuracy-with-Early-Stopping

# Instruction:
Tasks performed in the provided code:

1. **Data Loading**:
   - Load the MNIST dataset, specifically the training images and labels.

2. **Data Preprocessing**:
   - Normalize the pixel values of the training images to the range [0, 1].

3. **Callback Definition**:
   - Define a custom callback class named `myCallback`.
   - Implement the `on_epoch_end` method to monitor the training accuracy at the end of each epoch.
   - If the training accuracy reaches 99% or higher, print a message indicating that training will be stopped.

4. **Model Architecture**:
   - Define the neural network model using the `train_mnist` function.
   - The model includes:
     - One Flatten layer to flatten the input images.
     - One Dense layer with 512 units and ReLU activation.
     - One Dense output layer with 10 units and softmax activation for multi-class classification (MNIST has 10 classes).

5. **Model Compilation and Training**:
   - Compile the model using Adam optimizer and sparse categorical cross-entropy loss.
   - Fit the model for 10 epochs.
   - Use the custom callback to stop training when the accuracy reaches 99%.
   - Ensure that training stops before the 9th epoch.

6. **Validation**:
   - Verify that the callback stops training once the desired accuracy is reached.


# Problem:
![Screenshot (29)](https://github.com/ArsalMirza007/MNIST-Classifier-Training-to-99-Accuracy-with-Early-Stopping/assets/121928372/1fcec5ee-6ee4-4b6d-a8df-944b3d45b54b)


# Solution:
![Screenshot (28)](https://github.com/ArsalMirza007/MNIST-Classifier-Training-to-99-Accuracy-with-Early-Stopping/assets/121928372/9a718ccf-c4eb-43d8-b646-99723d4986bc)
