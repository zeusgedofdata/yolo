# yolo



1. First we Parse the arguments for command line. 
	a. Can adjust: batch size, object confidence, non-max supression threshold, config file, input resolution
2.  Load the class names
3. Create the architecture by loading in the config file that defines the layers
4. Create each layers as a sequence as defined by the config file. 
5. Load the weights for each layer, from the weights file. This file is a binary file that contains the weights for each neuron in the network.
6. Set the meta data for the input resolution. 
7. Load our batch of images from the filepath given in command line
8. Save a list of the original dims of the image so that we can reset the scale later
9. Create the batches for the images, create last batch as the left overs that don't fit into a full batch
10. Loop through the batches 
	a. 