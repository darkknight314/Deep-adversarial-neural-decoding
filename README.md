# Deep adversarial neural decoding
Partial implementation of the a NIPS research paper based on neural decoding by combining probabllistic inferenceing with Deep Convolutional Generative Adversarial Network(DCGAN).
Paper link : https://arxiv.org/abs/1705.07109

The aim of the paper is to reconstruct perceived stimuli(i.e. images in case of the training of the model) from brain responses measured using blood oxygen level dependent(BOLD) responses. It makes use of two datasets-the CelebA dataset and fMRI dataset. The procedure undertaken in the paper involves to transform images to latent feature space and then learn the relationship between the latent feature space and brain responses through probablistic inferencing. Then the transformation from latent feature space back to the perceived stimuli is achieved by training a Convolutional Neural Network using adversarial training. The transformation to the latent feature space is achieved by truncating the VGG Face pretrained model to 14 layers to output 4096 features and then further applying Principal Component Analysis(PCA) to reduce latent features to 699.

# Details
The project was undertaken as a part of the course BITS F312 and was completed under the supervision of Prof. Surekha Bhanot. It was implemented in PyTorch and this implementation only covers the transformation from the latent feature space to perceived stimuli using DCGANs due to unavailability of the fMRI dataset to public. PCA was implemented manually due to non-interoperability with other implementations in python. The PCA transformation matrix was calculated beforehand and stored as a checkpoint.

To run
1) Download weights checkpoints folder from here :-
https://drive.google.com/open?id=1PJ2YMVBqbL253GCIVijgXkxyjKaWAvje

2) Download CelebA dataset(not needed to download entire) and store in train and test folder

The final presentation can be found here :-
https://github.com/darkknight314/Deep-adversarial-neural-decoding/wiki

# Screenshots of final results
