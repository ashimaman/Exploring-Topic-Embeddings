# Exploring-Topic-Embeddings

This repository contains the jupyter notebook as a submission for the test task Exploring-Topic-Embeddings given in the ML for NLP course. I have summarized the steps in the notebook here below:

1. The first step we do here is import some importatnt libraries which we will be using in the course of this test task.
2. The next step is to import the 20 Newsgroups dataset from the given link and vectorize it. We also split the data into training and validation sets.
3. Next we define the architecture of our neural network. This is how is model is designed: 

The model is here is used for text classification using the bag-of-words (BoW) representation. The input layer has a size of input_size, which corresponds to the number of unique words in the vocabulary. The first hidden layer has hidden_size neurons and is fully connected to the input layer. The activation function used in this layer is the rectified linear unit (ReLU). The output layer has output_size neurons, one for each class in the dataset, and is fully connected to the first hidden layer. The activation function used in this layer is the softmax function, which outputs a probability distribution over the classes.

During forward propagation, the input x is passed through the first fully connected layer (fc1) followed by the ReLU activation function. The resulting activations are then passed through the second fully connected layer (fc2) followed by the softmax activation function, which outputs the predicted probability distribution over the classes.

4. In the next step we perfrom the actual training and evaluate the model on the validation set. Here we print the training loss and accuracy as well as the validation loss and accuracy.

5. In the last step we plot the accuracy on the training and the validation dataset.
