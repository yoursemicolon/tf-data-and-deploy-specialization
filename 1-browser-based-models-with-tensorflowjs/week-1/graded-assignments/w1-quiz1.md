# Week 1 - Quiz 1

### Question 1
What is the name of the API at the heart of TensorFlow.js which allows things like layers to be used?
- [x] Core API
- [ ] Core TF API
- [ ] TFJS API
- [ ] JS API

### Question 2
How does TensorFlow.js use GPU acceleration in the browser?
- [ ] 
You have to install GPU runtimes for each browser, and explicitly use them
- [x] You access GPU through WebGL in the browser
- [ ] It doesn't
- [ ] It works natively through GPU libraries in TensorFlow

### Question 3
How can you use a TPU with TensorFlow.js?
- [ ] You have to serve your JS from a GCP instance
- [ ] Only using Colab
- [x] You can use Node.js on GCP and access TPU instances
- [ ] You can't

### Question 4
Which of the following lines of code will correctly add a single dense layer containing a single neuron that takes a numeric input to a model using JavaScript?
- [ ] ``model.add(tf.layers.dense({units: 1, inputShape:= [1]}))``;
- [ ] ``model.add(tf.layers.dense({units= 1, inputShape: [1]}));``
- [x] ``model.add(tf.layers.dense({units: 1, inputShape: [1]}));``
- [ ] ``model.add(tf.layers({units: 1, inputShape: [1,1]}));``

### Question 5
When creating data to input to a model using Python you could use a numpy array. How would you do it in JavaScript?
- [ ] Use a numpyjs array
- [ ] Use a tensor2d containing the data
- [x] Use a tensor2d containing the data and the shape of the data
- [ ] Use a tensor2d contining a numpyjs array

### Question 6
If I train a model to detect a linear relationship (i.e. Y=2X-1), what line of code would output a prediction from that model for Y where X=10?
- [x] ``alert(model.predict(tf.tensor2d([10], [1,1])));`` 
- [ ] ``alert(model.predict(tf.tensor2d([10], [1,1])));`` 
- [ ] ``alert(model.predict(10));``
- [ ] ``alert(model.predict([10], [1,1]));``

### Question 7
When training a model, if I want to log training status at the end of an epoch, what is the name of the callback event you want to capture?
- [ ] EpochEnd
- [ ] EpochEnded
- [ ] OnEpochEnded
- [x] onEpochEnd
