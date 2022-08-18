# Variational-autoencoders
# Project 1:
Here we create a 2 dimensional latent vector space and map each image of number to a unique point in the vector space using an encoder trained on the mnist dataset.
We also create a decoder which extracts the digit from a point in the vector space.
On visualizing the vector space, we observe certain directions represent certain properties such as zeroness or fiveness. 
Hence we can transform the numbers in the vector space and decode it two get the required number.\

# Project 2:
Here we extend the idea discussed above for images of faces. The link to dataset of celebrity has been provided. We create a 64 dimensional vector space.\
(As face image has much more 'information' than digit image, mapping to anything less than 64 dimensions results in substantial loss of information. Using more dimensions does not respect the continuity of vector space ie we need every point in the space to be mapped to some percievable image)\
We create an encoder which is trained on the celebrity dataset and map the image of face to a unique point in the 64-dimensional space. We also create a decoder which extracts the image of face from any point in the latent space.
It is difficult to visualize 64 dimensional information on 2 dimensional page. However an attempt is made to visualize the variation in decoded image with small variations in 2 dimensions and keeping other dimensions fixed. We observe certain directions of increasing shadow intensities and other properties. \
It is difficult to extract some direction vectors which are meaningful, however a smile vector was identified in the latent space by subtracting the image of smiling person and sad person in the 64 dimensional space.

# Requirements:
python3\
tensorflow\
keras\
numpy\
matplotlib
