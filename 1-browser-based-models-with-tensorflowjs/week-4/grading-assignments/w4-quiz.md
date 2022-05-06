# Week 4 - Quiz

### Question 1
What HTML5 tag is used to show the contents of a webcam?
* [ ] <webcam>
* [ ] <pre>
* [ ] <div>
* [x] <video>

### Question 2
If I initialize a webcam object like this:
```javascript
const webcam = new Webcam(document.getElementById('wc'));
```
* [ ] ``async function init(){await webcam.initialize();}``
* [ ] ``async function init(){await webcam.go();}async function init(){await webcam.go();}``
* [x] ``async function init(){await webcam.setup();}``
* [ ] ``async function init(){await webcam.start();}``

### Question 3
If I want to create a model that uses transfer learning, with everything in mobilenet up to layer ‘foo’, and my layers afterwards, how do I do it? Assume this code was used to find layer ‘foo’
```javascript
const layer = mobilenet.getLayer('foo');
```
* [ ] ``return tf.model({inputs: mobilenet.inputs, outputs: layer.outputs});``
* [x] ``return tf.model({inputs: mobilenet.inputs, outputs: layer.output});``
* [ ] ``return tf.model({inputs: mobilenet, outputs: layer});``
* [ ] ``return tf.model({inputs: mobilenet.input, outputs: layer.outputs});``

### Question 4
If I am transfer learning from a mobilenet, and I want to use my own dense layers after the mobilenet ones, what is the correct syntax to use at <INSERT CODE HERE>
```javascript
model = tf.sequential({
    layers: [
      tf.layers.flatten(<INSERT CODE HERE>),
      tf.layers.flatten({inputShape: mobilenet.outputs[0].shape.slice(1)}),
      tf.layers.dense({ units: 100, activation: 'relu'}),
      tf.layers.dense({ units: 3, activation: 'softmax'})
    ]
  });
```
* [ ] ``{inputShape: mobilenet.outputs[1].shape.slice(0)}``
* [ ] ``{inputShape: mobilenet.outputs[0].slice(1)}``
* [ ] ``{inputShape: mobilenet.outputs[1].slice(0)}``
* [x] ``{inputShape: mobilenet.outputs[0].shape.slice(1)}``

### Question 5
If I am using a mobilenet with my own DNN for transfer learning in TensorFLow.js, how do I get a prediction for an image?
* [x] Get a set of prediction embeddings from mobilenet and pass them to your model
* [ ] Just pass the prediction to your own model, it already includes the mobilenet layers
* [ ] Just pass the prediction to mobilenet, because you’ve already added your layers to it
* [ ] Get a set of prediction embeddings from your model and pass them to mobilenet

### Question 6
If you have a set of predictions returned from model.predict(something) and you want to take the one with the largest probability, how do you do it?
* [ ] ``predictions.sort()`` then look at the 0th element
* [ ] ``predictions[0]`` contains the one with the largest probability
* [ ] ``predictions.argMax()`` then look at the 0th element
* [x] ``predictions.as1D().argMax()``, then look at the 0th element

### Question 7
If you already have a function called predict() in a class called ‘foo’  which captures a frame from the webcam and predicts it, what’s the best way to call it, particularly if you plan to do continuous predictions?
* [ ] ``foo.predict(tf.tidy());``
* [x] ``tf.tidy(() => foo.predict());``
* [ ] ``foo.predict(); tf.tidy();``
* [ ] ``tf.tidy(foo.predict());``

### Question 8
Why is transfer learning a huge advantage, particularly when training in the browser?
* [x] It allows you to use already-learned convolutions for distinguishing features, saving training tim
* [ ] It allows you to use already-learned convolutions for distinguishing features, saving space
* [ ] It lets you skip training altogether
* [ ] It gives you a smaller model