**Introduction**
Variational Autoencoders (VAEs) have emerged as powerful generative models that learn to
represent complex high-dimensional data in a low-dimensional latent space. They can generate
new data samples that are similar to the training data. In this report, we present the
implementation of a Variational Autoencoder for the MNIST digits dataset.
Variational Autoencoders (VAEs) are a type of generative model that learns to reconstruct input
data while simultaneously learning a latent representation of the data. By sampling from the
learned latent space, VAEs can generate new data that closely resembles the training data.
**Experiment Description
**
We have implemented a Variational Autoencoder (VAE) using PyTorch. The VAE is comprised
of an encoder and a decoder network. The encoder network takes the input image and maps it
into a latent space, where it computes the mean and the log variance of the latent variables. The
decoder network then uses these latent variables to reconstruct the input image..
**Methodology**
We implemented the Variational Autoencoder (VAE) for the MNIST digits dataset using a twostep approach. First, we designed the architecture of our VAE, which consists of an encoder
network, a decoder network, and a sampling layer for generating latent variables. We trained
VAE using the Adam optimizer with a learning rate of 0.001 for 12 epochs. During each epoch,
we computed the reconstruction loss and the KL divergence loss, and updated the model
parameters using backpropagation. After training, we evaluated the performance of VAE by
generating new images. We sampled random latent variables from the learned latent space and
passed them through the decoder network to generate new images. We also explored the effect
of changing the number of latent variables on the quality of the generated images
**Results and Discussion
**
After training VAE, we observed the following results:
Epochs Loss
1 544.472
2 418.784
3 371.340
4 350.623
5 341.861
6 337.413
7 331.953
8 329.167
9 326.386
10 323.614
11 322.446
12 320.234
As we can see, the loss decreases as the number of epochs increases, indicating that the model
is learning to reconstruct the input images more accurately
