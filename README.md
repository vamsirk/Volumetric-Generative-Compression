# Volumetric-Generative-Compression

We propose a Generative 3D Compression model for

compressing 3D volumetric objects. The model has an ad-
vantage over traditional compression method using linear

transformation in a sense that the model can learn an arbi-
trary encoding function via backpropagation. While a sim-
ple autoencoder models can easily achieve that, the recon-
structed object are usually lossy and quite unpleasant. Our

model uses generative network(3D GAN) to guide the di-
rection of the decoder to further improve the quality of the

reconstructed object.

We worked on implementing 3D-GAN, with the method-
ologies developed by Wu et al.[13], for 3D object genera-
tion. The 3D-GAN model is then extended to a Generative

3D Compression network by using the adversarially trained

genenerator network as a decoder. In addition, we incorpo-
rate perceptual loss into the training of the network to help

the network capture low-level features. The model is able to
compress volumetric objects by over 164 times and is still
able to recover most of the important features of the objects.
Finally, we compare the object reconstructions produced by
this network with the traditional auto-encoder reconstructed
models to compare the quality of the reconstruction.
