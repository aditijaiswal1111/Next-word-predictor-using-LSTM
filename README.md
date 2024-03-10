# Text Generator using LSTM with TensorFlow and Keras

This project is aimed at building a text generator using LSTM (Long Short-Term Memory) networks implemented with TensorFlow and Keras. The text generator is trained on a dataset of text sequences and is capable of generating new text based on the patterns learned during training.

## Overview

The text generator operates in the following steps:

1. **Data Preprocessing:** Input text data is preprocessed to tokenize the text into individual words and assign unique integer indices to each word. This preprocessing step also involves sequence padding to ensure uniform input lengths.
   
2. **Creating Input-Output Pairs:** The preprocessed text data is segmented into sequences of fixed length, with each sequence serving as an input to the model. Corresponding to each input sequence is the next word in the text, which serves as the output label for the model.
   
3. **Model Architecture:** The LSTM-based neural network architecture is designed using TensorFlow's Keras API. The model consists of an embedding layer for word representation, followed by one or more LSTM layers, and finally a dense layer for output prediction.
   
4. **Training the Model:** The model is trained using the input-output pairs generated in the previous step. During training, the model learns to predict the next word in a sequence based on the input sequence provided.
   
5. **Text Generation:** Once trained, the model can be used to generate text. Starting with a seed sequence, the model predicts the next word, which is then appended to the sequence. This process is iterated to generate longer sequences of text.

## Usage

To use the text generator:

1. **Install Dependencies:** Ensure you have the required dependencies installed, including TensorFlow and Keras.
   
2. **Data Preprocessing:** Use the provided preprocessing script to tokenize and preprocess your input text data. This step is crucial for preparing the data for training.
   
3. **Training:** Execute the training script or Jupyter Notebook to train the text generation model on your preprocessed data. Training may take some time depending on the size of the dataset and complexity of the model architecture.
   
4. **Generating Text:** Once the model is trained, you can use it to generate text. Provide a seed sequence as input to the model, and it will generate the next word in the sequence. Repeat this process to generate longer passages of text.

## Files and Directories

- `text_generator.ipynb`: Jupyter Notebook containing the code for training and using the text generator.
- `preprocessing.py`: Python script for preprocessing input text data.
- `data/`: Directory containing sample input text data for demonstration purposes.

## Dependencies

- TensorFlow
- Keras



