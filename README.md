
# Sinhala Kavi generation with LSTM 

This repository contains code for training an LSTM-based language model to generate Sinhala text. The code is implemented in Python using the Keras framework, and makes use of the TensorFlow backend.

One of the key challenges in working with Sinhala text is the need to process Unicode characters. This can often pose difficulties for NLP models, as many libraries and tools do not natively support Unicode. However, this code successfully overcomes this challenge and is capable of processing Sinhala Unicode characters.

# Getting Started

The code is provided as a Jupyter Notebook, which can be run on Google Colab. Simply click the "Open in Colab" button above to get started. The notebook includes all the code and explanations needed to train the model, as well as to generate text using the trained model.

# Dependencies

The code requires the following Python packages:

    Keras
    TensorFlow
    Numpy
    Pandas
    Matplotlib

## Usage/Examples

seed phase 
```
සඳුන් සුවඳ විහිදෙයි වට
```

Output

```
සඳුන් සුවඳ විහිදෙයි   වට
සුවඳ විහිදෙයි වට     යත
විහිදෙයි වට යත      මිතුර
වට යත මිතුර        වට
```

