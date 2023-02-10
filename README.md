
# Sinhala Text Generation with LSTM

This repository contains a Colab Notebook for generating Sinhala text using a Long-Short Term Memory (LSTM) Recurrent Neural Network (RNN). The code implements a character-based generation model that can produce coherent and stylistically consistent text given a seed string. The model is trained on a dataset of Sinhala poems and news titles, allowing it to generate new text in the same style.

The repository includes two Colab Notebooks for text generation:

    A Notebook for generating Sinhala කවි, with a specified number of lines and a fixed line length.
    A Notebook for generating Sinhala news titles, without any line restrictions.

this project was undertaken as a part of a social experiment, where AI-generated poems and news were posted on social media to study the reactions of the audience. 

## Dependencies

The code requires the following Python packages:

    Keras
    TensorFlow
    Numpy
    Pandas
    Matplotlib

## Usage

The code can be executed in a Colab environment, which provides a free GPU for faster training and inference. Simply follow the instructions in the corresponding Colab Notebook to train and generate new text using the model.
Model Training

The model is trained using a character-based approach, where each character in the text is treated as a separate time step. The model learns to predict the next character given the sequence of previous characters. The LSTM network architecture consists of multiple layers and is trained using the categorical cross-entropy loss function. The network can be trained on a custom dataset by loading the data and specifying the appropriate parameters in the code.
Text Generation

Text generation is performed by inputting a seed string and iteratively predicting the next character based on the internal state of the network and the seed string. The model generates new text by repeating this process until a stopping criterion is met, such as a maximum number of characters or reaching a specific end-of-sequence token. The generated text can be further adjusted by fine-tuning the temperature parameter, which controls the randomness of the prediction process.
Advanced Features

## This code implements several techniques for text generation using LSTMs, including:

Character-based generation for improved coherence and consistency compared to word-based approaches
The use of LSTMs to capture long-term dependencies in the text data
The ability to process Sinhala Unicode characters, making it possible to generate text in a variety of scripts and languages.
The ability to fine-tune the temperature parameter for controlling the randomness and creativity of the generated text.

## Example Output

seed phase for news title generation
```
    ට්‍රම්ප්
```

output
```
    ට්රම්ප් නවසීලන්තයට යයි ඡායාරූප සහිතයි
```

seed phase for poem generation
```
සඳුන් සුවඳ විහිදෙයි වට
```
output
```
සඳුන් සුවඳ විහිදෙයි     වට
සුවඳ විහිදෙයි වට       යත
විහිදෙයි වට යත       මිතුර
වට යත මිතුර         වට
```
