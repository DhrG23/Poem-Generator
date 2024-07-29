# Poem-Generator
Code for traning a Tensor Flow LSTM (Long Short-Term Memory) model 
This allow you to genrate poem with different styles depending the tye of dataset you train it on. A sample dataset in inc. in the reop - poem.txt 

# Project Info
Model Architecture:

Embedding Layer:

The input text data is converted into dense vectors using an embedding layer. Each word is represented as a fixed-size vector in a high-dimensional space.
Bidirectional LSTM Layers:

The embedding vectors are passed through Bidirectional LSTM (Long Short-Term Memory) layers. LSTM is a type of recurrent neural network (RNN) that can capture long-term dependencies in sequential data.
The Bidirectional LSTM layers process the input sequences in both forward and backward directions, capturing information from past and future contexts.
Dropout Layer:

A dropout layer is added to prevent overfitting. Dropout randomly drops a fraction of input units to zero during training, which helps in regularization and improves generalization.
Dense Layers:

The output from the LSTM layers is fed into fully connected dense layers. These layers perform non-linear transformations on the input data, allowing the model to learn complex patterns.
Output Layer:

The final dense layer with a softmax activation function generates probabilities for the next word in the sequence. The word with the highest probability is selected as the predicted next word.
Compilation:

The model is compiled using the categorical cross-entropy loss function and the Adam optimizer. Categorical cross-entropy is commonly used for multi-class classification tasks, while Adam is an efficient optimizer for training neural networks.
Training:

The model is trained on the input sequences and corresponding labels (one-hot encoded). During training, the model adjusts its parameters (weights and biases) to minimize the loss function, i.e., the difference between predicted and actual outputs.
Model Summary:

The model summary provides a detailed overview of the layers, their output shapes, and the number of trainable parameters.
