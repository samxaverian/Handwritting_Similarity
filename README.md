# Handwritting_Similarity
Finding if 2 given handwritting are of the same person or different.

**hand3.ipynb** has the preprocessing steps for the whole data set: train and validation folders.
We have used the EAST network to determine regions with handwritten sentences.
We have used OpenCV's KNN and thresholding and some more preprocessing to get a good segment out from each of the images.

**handwriting-siamese-pytorch.ipynb** contains the model for training and predictions.
We have created a Siamese network which calculates contrastive loss for the twin network and backpropagstes to learn.
The twin networks are simpe CNN networks for images.
