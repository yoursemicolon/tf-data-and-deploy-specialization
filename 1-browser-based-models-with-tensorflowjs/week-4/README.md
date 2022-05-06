# Transfer Learning with Pre-Trained Models

Last week you then saw how to take some pre-trained models in JSON format and use them before finally looking into how to convert your python models into JSON so that you can use them in the browser yourself. 

This week you'll take that a little further by looking into transfer learning. In this case, you're going to get an existing pre-trained model mobile net and you'll freeze some of its layers training a new neural network using the features that you've extracted from the mobile net. You'll capture images in the browser using the webcam, sort these into your desired classes. And then with transfer learning, you'll build a new model that classifies only those images.

## Rock Paper Scissors

In the next example, we will use a pre-trained MobileNet model to classify hand gestures of Rock, Paper, and Scissors captured by a webcam.

You can use Brackets to open the index.js file and take a look at the code. You can find the index.js file in the following folder in the GitHub repository for this course:

[tensorflow-2-public/C1_Browser-based-TF-JS/W4/ungraded_lab/](../../tensorflow-2-public/C1_Browser-based-TF-JS/W4/ungraded_lab/)