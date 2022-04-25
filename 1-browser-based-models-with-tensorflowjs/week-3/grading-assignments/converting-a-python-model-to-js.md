# Programming Assignment: Week 3 - Converting a Python Model to JavaScript

In this exercise, you’ll train a model in Python, and convert it to JavaScript. Open the C1_W3_Assignment.ipynb Jupyter notebook found in the following folder in the GitHub repository:

[tensorflow-2-public/C1_Browser-based-TF-JS/W3/assignment/](../../../tensorflow-2-public/C1_Browser-based-TF-JS/W3/assignment/)

To run this notebook you will need have installed Jupyter with Python 3, TensorFlow 2.0, Tensorflow.js, NumPy, and Matplotlib.

In this notebook we train a neural network to classy images of Cats and Dogs. It was used in the Introduction to TensorFlow class here at Coursera, which can give you a primer in using Python to build models. At the bottom of the notebook are sections for you to fill-in --  saving your model as a Keras HDF5 file, and then using the TensorFlow.js converter to convert it to JavaScript. You must fill-in the missing code in the parts labeled:

```python
# YOUR CODE HERE
```

NOTE: The convolutional neural network in this notebook can take about 4 minutes to train, however, this time can vary depending on your setup. 

If you do things correctly and run the code successfully, you will end up with a single JSON file named model.json and various .bin files, such as group1-shard1of10.bin. The number of .bin files will depend on the size of your model: the larger your model, the greater the number of .bin files. If you have a small model you will end up with just 1 .bin file.

You must upload the model.json and all the .bin files in a single Zip file to be graded. This single Zip file must contain a single model.json file and all the .bin files:
1. model.json: Contains the model architecture, i.e. the type and size of each layer.
2. group1-shard1of10.bin: Contains part of the weights of the model.
3. group1-shard2of10.bin: Contains part of the weights of the model.
4. group1-shard3of10.bin: Contains part of the weights of the model.
5. group1-shard4of10.bin: Contains part of the weights of the model.
6. 6. etc...