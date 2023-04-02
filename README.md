# DCGAN-to-generate-faces
Program in python to generate faces with DCGAN extension of GAN 

## DCGAN to generate faces.

For the project, we used an extension of GAN called DCGAN (Deep Convolutional Generative Adversarial Network), which explicitly uses convolutional and convolutional-transpose layers in the discriminator and generator. The discriminator is composed of convolutional layers with stride, batch normalization layers, and LeakyReLU activations. The input is a 3x64x64 input image, and the output is a scalar probability that the input comes from the real data distribution. The generator is composed of convolutional-transpose layers, batch normalization layers, and ReLU activations. The input is a latent vector z drawn from a standard normal distribution, and the output is an RGB image of 3x64x64. The convolutional-transpose layers allow the latent vector to be transformed into a volume with the same shape as an image.

In the program we use the dataset of celeb_a, using 20,000 celebrity images and 300 epoch, and the result of the code were:

<p align="center">
  <img src="Fakes_images/animation.gif" width="500" height="500">
</p>

<p align="center">
This animation, we can se all the images that create the algorithm in a gif.
</p>
 

<p align="center">
  <img src="Fakes_images/image_95.png" width="500" height="500">
</p>

<p align="center">
This image is the last image of the code process
</p>


<p align="center">
  <img src="Fakes_images/Grafica_Dloss_Gloss.jpg" width="500" height="250">
</p>

<p align="center">
This graph represents the losses of the generator and the discriminator
</p>


<p align="center">
  <img src="Fakes_images/r&fimage.jpg" width="600" height="250">
</p>

<p align="center">
Finally this image shows the real images vs the false images that the code performs
</p>

