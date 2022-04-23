# Programming Assignment: Week 1 - Breast Cancer Classification

This week you looked at doing a multi-class classification of Iris flowers, trained on CSV data. For your exercise, you’ll do something very similar -- but working with breast cancer data adapted from the  [Wisconsin dataset](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). 

In this exercise, you will try to build and train a neural network that can predict from new data whether the diagnosis is malignant or benign. To train your network you will be using the given CSV data. The data has already been split for you into a [training](https://github.com/https-deeplearning-ai/tensorflow-2-public/blob/main/C1_Browser-based-TF-JS/W1/assignment/data/wdbc-train.csv) and a [validation](https://github.com/https-deeplearning-ai/tensorflow-2-public/blob/main/C1_Browser-based-TF-JS/W1/assignment/data/wdbc-test.csv) set. If you look at the CSV files, you will notice that the first column corresponds to the  ‘diagnosis’ . The values in this column correspond to the diagnosis where a value of 1 indicates a malignant cancer, and a 0 indicates a benign one. Try to build a model that gives a very high accuracy on the test data. 

Use Brackets to open the **C1_W1_Assignment.html** file found in the following folder in the GitHub repository:

[tensorflow-2-public/C1_Browser-based-TF-JS/W1/assignment/](https://github.com/https-deeplearning-ai/tensorflow-2-public/blob/main/C1_Browser-based-TF-JS/W1/assignment/data/wdbc-test.csv)

Follow the instructions given in the code and fill-in the missing code in the parts labeled:

// Your Code Here

Once you have filled-in the missing code, run the **C1_W1_Assignment.html** file in the Chrome browser using the Web Server. Once you have trained your model, and ran the code successfully, the code will automatically download your model and its weights to your downloads folder. **It is important to note that your browser might prompt you to allow multiple files to be downloaded. If this happens, allow the browser to download multiple files.** 

Once the files have been downloaded, you must upload these two files in a single Zip file to be graded. This single Zip file must only contain 2 files:    
1. my_model.json: Contains the model architecture, i.e. the type and size of each layer.
2. my_model.weights.bin: Contains the weights of the model.    