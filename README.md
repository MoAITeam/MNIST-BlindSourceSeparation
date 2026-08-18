# Overlay-Separation (_"BlindSourceSeparation"_)

## Deep Learning Lab Challenge at UniBo

An image is given in input, which is the overlay of two samples from MNIST and Fashion MNIST. 
The challenge consists into reconstructing the original samples with a neural network, as closely as possible (according to mean squared error). 
No preprocessing is allowed.

<div align="center">
<img src="assets/ex1.png" alt="Image 1" style="float: left; width: 10vw;" />
<img src="assets/ex2.png" alt="Image 2" style="float: left; width: 18vw;" />
  <br>
  Input combined image and desired output.
</div>

## Task and Dataset
- Task: Train a neural network to solve the challenge.
- Dataset: 70,000 images from MNIST and 70,000 images from Fashion MNIST
- Combination algorithm: It is known that test images are just a weighted sum of two samples
- Data format: 28×28 grayscale images

## Methods
- An autoencoder network is a good starting point
- We choose a U-Net specifically

## Future improvements
At the end of the challenge, it was revealed that an attention mechanism is beneficial, to achieve maximum pixel level accuracy.
