**Autoencoder for Image Compression**

**Introduction**

This project demonstrates the use of an autoencoder to compress and reconstruct image data. An autoencoder is a type of artificial neural network used to learn efficient representations (encodings) of input data, typically for the purpose of dimensionality reduction. In this project, we use the MNIST dataset to train the autoencoder, compress the images, and then reconstruct them.

**Requirements**

Python 3.x

TensorFlow

Keras

NumPy

Matplotlib

**Acknowledgements**

The MNIST dataset was used in this project, which is freely available from Yann LeCun's website.

**Autoencoder Architecture**

An autoencoder consists of two parts:

**Encoder:** This part compresses the input into a smaller, dense representation, called the latent space or bottleneck layer.
**Decoder:** This part reconstructs the input from the compressed latent space representation.

**Model Layers:**

**Input Layer:** Takes a flattened 28x28 image, which results in 784 input neurons.

**Bottleneck Layer:** The layer where the compression happens, reducing the dimensionality of the input. For example, from 784 dimensions to 32.

**Output Layer:** Reconstructs the input image from the compressed representation.

**Key Parameters:**

**Input shape:** (784,) — each image is flattened into a 1D vector of 784 elements.

**Latent space (bottleneck):** 32 neurons — this is the compressed version of the input.

**Activation functions:** ReLU for hidden layers, Sigmoid for the output layer.

**Dataset**

We use the **MNIST dataset**, which contains 60,000 training images and 10,000 test images of handwritten digits (0-9). Each image is of size 28x28 pixels.

**Dataset Preprocessing:**

**Normalization:** We scale the pixel values to a range of [0, 1] by dividing by 255.

**Flattening:** The 28x28 pixel images are flattened into vectors of size 784 to feed them into the model.

**Training the Autoencoder**

Load the MNIST dataset.
Build the autoencoder model.
Train the model on the dataset for a specified number of epochs.

**Visualizing the Results**

After training, the script will plot:

**Original Images**: A set of images from the MNIST test dataset.

**Reconstructed Images:** The corresponding reconstructed images from the autoencoder.

**Training and Reconstruction**

After training,

**Compression:** The autoencoder will compress each 784-dimensional input image into a 32-dimensional vector.

**Reconstruction:** The model will attempt to reconstruct the original image from the 32-dimensional compressed representation.

**Evaluate the Model**
Visualize how well the autoencoder has compressed and reconstructed the input data by comparing the original and reconstructed images.

![image](https://github.com/user-attachments/assets/a5d65d84-833b-4bdb-ab47-05cd148660e4)




