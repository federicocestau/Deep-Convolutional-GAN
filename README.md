# Deep-Convolutional-GAN
Data Scientists use Generative Adversarial Networks (GANs) for a wide range of tasks, with image generation being one of the most common. A particular type of GAN known as DCGAN (Deep Convolutional GAN) has been created specifically for this.

GAN only uses dense layers into its deep neural network architecture, since it does not use convolutional layers, we can create shapes available in python libraries but NOT necessarily recreate images in jpg or png format for example. 

Let me start by highlighting that DCGAN utilizes Convolutional and Transposed Convolutional layers, which it strategically embeds into a GAN architecture.

We will use Convolutional layers inside the Discriminator model and the final layer of the Generator model.

Transposed Convolutions also use filters to process the data, but their goal is the opposite of a regular Convolution. I.e., we use them to upsample the data to a larger output feature map, while regular Convolutions downsample.

A Generative Adversarial Network (GAN) combines the Generator and the Discriminator models that compete against each other in a zero-sum game, making them adversaries.
The Generator creates fake images attempting to fool the Discriminator into believing they are real. Meanwhile, the Discriminator learns the essential features of the pictures in order to differentiate between real and fake examples.

The Discriminator model is just a Convolutional classification model. In contrast, the Generator model is more complex as it learns to convert latent inputs into an actual image with the help of Transposed and regular Convolutions (last layer uses convolution not transposed). 
