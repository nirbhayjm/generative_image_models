# Computer Vision Project - Generative Image Models
Nirbhay Modhe, Vikas Jain  
Recent Adavances in Computer Vision, Prof Gaurav Sharma, Autumn 2016 
## Description
The project is based on the work by google Deepmind "DRAW: A recurrent neural network for image generation" by K Gregor et al. The purpose of the project was to implement and understand the paper and possible enhance the model for better image generation.
## Workdone
1. Implemented the model proposed in the paper. The code is adapted from the implementation by Eric Jang ([link here](http://blog.evjang.com/2016/06/understanding-and-implementing.html)).
2. Analyzed the network parameters of DRAW model.
3. Analyzed the latent space of the encoded images. This deems as an important step which was missing and produced interesting observations.
4. Proposed and trained 3 models incorporating CNN in the original DRAW model:
	1. Model I - *Each Step Convolution*
	2. Model II - *Supervised Encoder*
	3. Model III - *Convolutional Encoder*  
Each model shows better performance than the original DRAW model.

## Code Contribution
1. Implemented **stochastic data generation** part of the paper.
2. Added an **interface for the SVHN dataset** to be given as input to the draw network.
3. Added **convolution and deconvolution wrappers** for training the proposed **models I, II and III**.
4. Implemented the evaluation phase to calculate the **negative log-likelihood of the generated images**.
5. Added new sampling functionalities to **visualize the latent space**.
6. **Visualizing and plotting kernels** of the learned CNN.

## Code Directory
1. DRAW-replication: implementation of original paper on two datasets -- MNIST and SVHN.
2. models: code for three new model proposed
3. error-calculation: code for calculating negative log likelihood of the images generated by different models.
4. plotting: code for plotting kernels and generated images.
5. report: final report and presentation of the project.

## Results
For the performance measure of the three proposed models, and analysis of the DRAW model, see final report and presentation in the 'report' folder.