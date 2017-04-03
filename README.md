# api documentation for  [brain (v0.7.0)](https://github.com/harthur/brain)  [![npm package](https://img.shields.io/npm/v/npmdoc-brain.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-brain) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-brain.svg)](https://travis-ci.org/npmdoc/node-npmdoc-brain)
#### Neural network library

[![NPM](https://nodei.co/npm/brain.png?downloads=true)](https://www.npmjs.com/package/brain)

[![apidoc](https://npmdoc.github.io/node-npmdoc-brain/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-brain_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-brain/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-brain/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-brain/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Heather Arthur",
        "email": "fayearthur@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/harthur/brain/issues"
    },
    "dependencies": {
        "inherits": "~2.0.1",
        "underscore": ">=1.5.1"
    },
    "description": "Neural network library",
    "devDependencies": {
        "browserify": "~3.32.0",
        "canvas": ">=0.10.0",
        "grunt": "~0.4.3",
        "grunt-contrib-uglify": "~0.2.0",
        "mocha": ">=1.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a6d0718c064a9d50d9bff39f38557b6b94d4466c",
        "tarball": "https://registry.npmjs.org/brain/-/brain-0.7.0.tgz"
    },
    "homepage": "https://github.com/harthur/brain",
    "keywords": [
        "neural network",
        "classifier",
        "machine learning"
    ],
    "main": "./lib/brain",
    "maintainers": [
        {
            "name": "harth",
            "email": "fayearthur@gmail.com"
        }
    ],
    "name": "brain",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/harthur/brain.git"
    },
    "version": "0.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module brain](#apidoc.module.brain)
1.  [function <span class="apidocSignatureSpan">brain.</span>NeuralNetwork (options)](#apidoc.element.brain.NeuralNetwork)
1.  [function <span class="apidocSignatureSpan">brain.</span>crossValidate (classifierConst, data, opts, trainOpts, k)](#apidoc.element.brain.crossValidate)
1.  object <span class="apidocSignatureSpan">brain.</span>NeuralNetwork.prototype
1.  object <span class="apidocSignatureSpan">brain.</span>lookup
1.  object <span class="apidocSignatureSpan">brain.</span>neuralnetwork

#### [module brain.NeuralNetwork](#apidoc.module.brain.NeuralNetwork)
1.  [function <span class="apidocSignatureSpan">brain.</span>NeuralNetwork (options)](#apidoc.element.brain.NeuralNetwork.NeuralNetwork)

#### [module brain.NeuralNetwork.prototype](#apidoc.module.brain.NeuralNetwork.prototype)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>adjustWeights (learningRate)](#apidoc.element.brain.NeuralNetwork.prototype.adjustWeights)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>calculateDeltas (target)](#apidoc.element.brain.NeuralNetwork.prototype.calculateDeltas)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>createTrainStream (opts)](#apidoc.element.brain.NeuralNetwork.prototype.createTrainStream)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>formatData (data)](#apidoc.element.brain.NeuralNetwork.prototype.formatData)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>fromJSON (json)](#apidoc.element.brain.NeuralNetwork.prototype.fromJSON)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>initialize (sizes)](#apidoc.element.brain.NeuralNetwork.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>run (input)](#apidoc.element.brain.NeuralNetwork.prototype.run)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>runInput (input)](#apidoc.element.brain.NeuralNetwork.prototype.runInput)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>test (data)](#apidoc.element.brain.NeuralNetwork.prototype.test)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>toFunction ()](#apidoc.element.brain.NeuralNetwork.prototype.toFunction)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>toJSON ()](#apidoc.element.brain.NeuralNetwork.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>train (data, options)](#apidoc.element.brain.NeuralNetwork.prototype.train)
1.  [function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>trainPattern (input, target, learningRate)](#apidoc.element.brain.NeuralNetwork.prototype.trainPattern)

#### [module brain.lookup](#apidoc.module.brain.lookup)
1.  [function <span class="apidocSignatureSpan">brain.lookup.</span>buildLookup (hashes)](#apidoc.element.brain.lookup.buildLookup)
1.  [function <span class="apidocSignatureSpan">brain.lookup.</span>lookupFromArray (array)](#apidoc.element.brain.lookup.lookupFromArray)
1.  [function <span class="apidocSignatureSpan">brain.lookup.</span>lookupFromHash (hash)](#apidoc.element.brain.lookup.lookupFromHash)
1.  [function <span class="apidocSignatureSpan">brain.lookup.</span>toArray (lookup, hash)](#apidoc.element.brain.lookup.toArray)
1.  [function <span class="apidocSignatureSpan">brain.lookup.</span>toHash (lookup, array)](#apidoc.element.brain.lookup.toHash)

#### [module brain.neuralnetwork](#apidoc.module.brain.neuralnetwork)
1.  [function <span class="apidocSignatureSpan">brain.neuralnetwork.</span>NeuralNetwork (options)](#apidoc.element.brain.neuralnetwork.NeuralNetwork)



# <a name="apidoc.module.brain"></a>[module brain](#apidoc.module.brain)

#### <a name="apidoc.element.brain.NeuralNetwork"></a>[function <span class="apidocSignatureSpan">brain.</span>NeuralNetwork (options)](#apidoc.element.brain.NeuralNetwork)
- description and source-code
```javascript
NeuralNetwork = function (options) {
  options = options || {};
  this.learningRate = options.learningRate || 0.3;
  this.momentum = options.momentum || 0.1;
  this.hiddenSizes = options.hiddenLayers;

  this.binaryThresh = options.binaryThresh || 0.5;
}
```
- example usage
```shell
...



# brain
'brain' is a JavaScript [neural network](http://en.wikipedia.org/wiki/Artificial_neural_network) library. Here's an example of using
 it to approximate the XOR function:

'''javascript
var net = new brain.NeuralNetwork();

net.train([{input: [0, 0], output: [0]},
           {input: [0, 1], output: [1]},
           {input: [1, 0], output: [1]},
           {input: [1, 1], output: [0]}]);

var output = net.run([1, 0]);  // [0.987]
...
```

#### <a name="apidoc.element.brain.crossValidate"></a>[function <span class="apidocSignatureSpan">brain.</span>crossValidate (classifierConst, data, opts, trainOpts, k)](#apidoc.element.brain.crossValidate)
- description and source-code
```javascript
function crossValidate(classifierConst, data, opts, trainOpts, k) {
  k = k || 4;
  var size = data.length / k;

  data = _(data).sortBy(function() {
    return Math.random();
  });

  var avgs = {
    error : 0,
    trainTime : 0,
    testTime : 0,
    iterations: 0,
    trainError: 0
  };

  var stats = {
    truePos: 0,
    trueNeg: 0,
    falsePos: 0,
    falseNeg: 0,
    total: 0
  };

  var misclasses = [];

  var results = _.range(k).map(function(i) {
    var dclone = _(data).clone();
    var testSet = dclone.splice(i * size, size);
    var trainSet = dclone;

    var result = testPartition(classifierConst, opts, trainOpts, trainSet, testSet);

    _(avgs).each(function(sum, stat) {
      avgs[stat] = sum + result[stat];
    });

    _(stats).each(function(sum, stat) {
      stats[stat] = sum + result[stat];
    })

    misclasses.push(result.misclasses);

    return result;
  });

  _(avgs).each(function(sum, i) {
    avgs[i] = sum / k;
  });

  stats.precision = stats.truePos / (stats.truePos + stats.falsePos);
  stats.recall = stats.truePos / (stats.truePos + stats.falseNeg);
  stats.accuracy = (stats.trueNeg + stats.truePos) / stats.total;

  stats.testSize = size;
  stats.trainSize = data.length - size;

  return {
    avgs: avgs,
    stats: stats,
    sets: results,
    misclasses: _(misclasses).flatten()
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.brain.NeuralNetwork"></a>[module brain.NeuralNetwork](#apidoc.module.brain.NeuralNetwork)

#### <a name="apidoc.element.brain.NeuralNetwork.NeuralNetwork"></a>[function <span class="apidocSignatureSpan">brain.</span>NeuralNetwork (options)](#apidoc.element.brain.NeuralNetwork.NeuralNetwork)
- description and source-code
```javascript
NeuralNetwork = function (options) {
  options = options || {};
  this.learningRate = options.learningRate || 0.3;
  this.momentum = options.momentum || 0.1;
  this.hiddenSizes = options.hiddenLayers;

  this.binaryThresh = options.binaryThresh || 0.5;
}
```
- example usage
```shell
...



# brain
'brain' is a JavaScript [neural network](http://en.wikipedia.org/wiki/Artificial_neural_network) library. Here's an example of using
 it to approximate the XOR function:

'''javascript
var net = new brain.NeuralNetwork();

net.train([{input: [0, 0], output: [0]},
           {input: [0, 1], output: [1]},
           {input: [1, 0], output: [1]},
           {input: [1, 1], output: [0]}]);

var output = net.run([1, 0]);  // [0.987]
...
```



# <a name="apidoc.module.brain.NeuralNetwork.prototype"></a>[module brain.NeuralNetwork.prototype](#apidoc.module.brain.NeuralNetwork.prototype)

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.adjustWeights"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>adjustWeights (learningRate)](#apidoc.element.brain.NeuralNetwork.prototype.adjustWeights)
- description and source-code
```javascript
adjustWeights = function (learningRate) {
  for (var layer = 1; layer <= this.outputLayer; layer++) {
    var incoming = this.outputs[layer - 1];

    for (var node = 0; node < this.sizes[layer]; node++) {
      var delta = this.deltas[layer][node];

      for (var k = 0; k < incoming.length; k++) {
        var change = this.changes[layer][node][k];

        change = (learningRate * delta * incoming[k])
                 + (this.momentum * change);

        this.changes[layer][node][k] = change;
        this.weights[layer][node][k] += change;
      }
      this.biases[layer][node] += learningRate * delta;
    }
  }
}
```
- example usage
```shell
...

trainPattern : function(input, target) {
  // forward propogate
  this.runInput(input);

  // back propogate
  this.calculateDeltas(target);
  this.adjustWeights();

  var error = mse(this.errors[this.outputLayer]);
  return error;
},

calculateDeltas: function(target) {
  for (var layer = this.outputLayer; layer >= 0; layer--) {
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.calculateDeltas"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>calculateDeltas (target)](#apidoc.element.brain.NeuralNetwork.prototype.calculateDeltas)
- description and source-code
```javascript
calculateDeltas = function (target) {
  for (var layer = this.outputLayer; layer >= 0; layer--) {
    for (var node = 0; node < this.sizes[layer]; node++) {
      var output = this.outputs[layer][node];

      var error = 0;
      if (layer == this.outputLayer) {
        error = target[node] - output;
      }
      else {
        var deltas = this.deltas[layer + 1];
        for (var k = 0; k < deltas.length; k++) {
          error += deltas[k] * this.weights[layer + 1][k][node];
        }
      }
      this.errors[layer][node] = error;
      this.deltas[layer][node] = error * output * (1 - output);
    }
  }
}
```
- example usage
```shell
...
},

trainPattern : function(input, target) {
  // forward propogate
  this.runInput(input);

  // back propogate
  this.calculateDeltas(target);
  this.adjustWeights();

  var error = mse(this.errors[this.outputLayer]);
  return error;
},

calculateDeltas: function(target) {
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.createTrainStream"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>createTrainStream (opts)](#apidoc.element.brain.NeuralNetwork.prototype.createTrainStream)
- description and source-code
```javascript
createTrainStream = function (opts) {
  opts = opts || {};
  opts.neuralNetwork = this;
  this.trainStream = new TrainStream(opts);
  return this.trainStream;
}
```
- example usage
```shell
...
## Streams
The network now has a [WriteStream](http://nodejs.org/api/stream.html#stream_class_stream_writable). You can train the network by
 using 'pipe()' to send the training data to the network.

#### Example
Refer to 'stream-example.js' for an example on how to train the network with a stream.

#### Initialization
To train the network using a stream you must first create the stream by calling 'net.createTrainStream()' which takes the following
 options:

* 'floodCallback()' - the callback function to re-populate the stream. This gets called on every training iteration.
* 'doneTrainingCallback(info)' - the callback function to execute when the network is done training. The 'info' param will contain
 a hash of information about how the training went:

'''javascript
{
error: 0.0039139985510105032,  // training error
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.formatData"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>formatData (data)](#apidoc.element.brain.NeuralNetwork.prototype.formatData)
- description and source-code
```javascript
formatData = function (data) {
  if (!_.isArray(data)) { // turn stream datum into array
    var tmp = [];
    tmp.push(data);
    data = tmp;
  }
  // turn sparse hash input into arrays with 0s as filler
  var datum = data[0].input;
  if (!_(datum).isArray() && !(datum instanceof Float64Array)) {
    if (!this.inputLookup) {
      this.inputLookup = lookup.buildLookup(_(data).pluck("input"));
    }
    data = data.map(function(datum) {
      var array = lookup.toArray(this.inputLookup, datum.input)
      return _(_(datum).clone()).extend({ input: array });
    }, this);
  }

  if (!_(data[0].output).isArray()) {
    if (!this.outputLookup) {
      this.outputLookup = lookup.buildLookup(_(data).pluck("output"));
    }
    data = data.map(function(datum) {
      var array = lookup.toArray(this.outputLookup, datum.output);
      return _(_(datum).clone()).extend({ output: array });
    }, this);
  }
  return data;
}
```
- example usage
```shell
...
  }
  var output = input = this.outputs[layer];
}
return output;
  },

  train: function(data, errorThresh, iterations) {
data = this.formatData(data);
iterations = iterations || 20000;
errorThresh = errorThresh || 0.004;

var inputSize = data[0].input.length;
var outputSize = data[0].output.length;

var hiddenSizes = this.hiddenSizes;
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.fromJSON"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>fromJSON (json)](#apidoc.element.brain.NeuralNetwork.prototype.fromJSON)
- description and source-code
```javascript
fromJSON = function (json) {
  var size = json.layers.length;
  this.outputLayer = size - 1;

  this.sizes = new Array(size);
  this.weights = new Array(size);
  this.biases = new Array(size);
  this.outputs = new Array(size);

  for (var i = 0; i <= this.outputLayer; i++) {
    var layer = json.layers[i];
    if (i == 0 && (!layer[0] || json.inputLookup)) {
      this.inputLookup = lookup.lookupFromHash(layer);
    }
    else if (i == this.outputLayer && (!layer[0] || json.outputLookup)) {
      this.outputLookup = lookup.lookupFromHash(layer);
    }

    var nodes = _(layer).keys();
    this.sizes[i] = nodes.length;
    this.weights[i] = [];
    this.biases[i] = [];
    this.outputs[i] = [];

    for (var j in nodes) {
      var node = nodes[j];
      this.biases[i][j] = layer[node].bias;
      this.weights[i][j] = _(layer[node].weights).toArray();
    }
  }
  return this;
}
```
- example usage
```shell
...

## JSON
Serialize or load in the state of a trained network with JSON:

'''javascript
var json = net.toJSON();

net.fromJSON(json);
'''

You can also get a custom standalone function from a trained network that acts just like 'run()':

'''javascript
var run = net.toFunction();
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.initialize"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>initialize (sizes)](#apidoc.element.brain.NeuralNetwork.prototype.initialize)
- description and source-code
```javascript
initialize = function (sizes) {
  this.sizes = sizes;
  this.outputLayer = this.sizes.length - 1;

  this.biases = []; // weights for bias nodes
  this.weights = [];
  this.outputs = [];

  // state for training
  this.deltas = [];
  this.changes = []; // for momentum
  this.errors = [];

  for (var layer = 0; layer <= this.outputLayer; layer++) {
    var size = this.sizes[layer];
    this.deltas[layer] = zeros(size);
    this.errors[layer] = zeros(size);
    this.outputs[layer] = zeros(size);

    if (layer > 0) {
      this.biases[layer] = randos(size);
      this.weights[layer] = new Array(size);
      this.changes[layer] = new Array(size);

      for (var node = 0; node < size; node++) {
        var prevSize = this.sizes[layer - 1];
        this.weights[layer][node] = randos(prevSize);
        this.changes[layer][node] = zeros(prevSize);
      }
    }
  }
}
```
- example usage
```shell
...
var outputSize = data[0].output.length;

var hiddenSizes = this.hiddenSizes;
if (!hiddenSizes) {
  hiddenSizes = [Math.max(3, inputSize)];
}
var sizes = _([inputSize, hiddenSizes, outputSize]).flatten();
this.initialize(sizes);

var error = 1;
for (var i = 0; i < iterations && error > errorThresh; i++) {
  var sum = 0;
  for (var j = 0; j < data.length; j++) {
    sum += this.trainPattern(data[j].input, data[j].output);
  }
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.run"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>run (input)](#apidoc.element.brain.NeuralNetwork.prototype.run)
- description and source-code
```javascript
run = function (input) {
  if (this.inputLookup) {
    input = lookup.toArray(this.inputLookup, input);
  }

  var output = this.runInput(input);

  if (this.outputLookup) {
    output = lookup.toHash(this.outputLookup, output);
  }
  return output;
}
```
- example usage
```shell
...
var net = new brain.NeuralNetwork();

net.train([{input: [0, 0], output: [0]},
           {input: [0, 1], output: [1]},
           {input: [1, 0], output: [1]},
           {input: [1, 1], output: [0]}]);

var output = net.run([1, 0]);  // [0.987]
'''

There's no reason to use a neural network to figure out XOR however (-: so here's a more involved, realistic example:
[Demo: training a neural network to recognize color contrast](http://harthur.github.com/brain/)

## Using in node
If you have [node](http://nodejs.org/) you can install with [npm](http://github.com/isaacs/npm):
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.runInput"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>runInput (input)](#apidoc.element.brain.NeuralNetwork.prototype.runInput)
- description and source-code
```javascript
runInput = function (input) {
  this.outputs[0] = input;  // set output state of input layer

  for (var layer = 1; layer <= this.outputLayer; layer++) {
    for (var node = 0; node < this.sizes[layer]; node++) {
      var weights = this.weights[layer][node];

      var sum = this.biases[layer][node];
      for (var k = 0; k < weights.length; k++) {
        sum += weights[k] * input[k];
      }
      this.outputs[layer][node] = 1 / (1 + Math.exp(-sum));
    }
    var output = input = this.outputs[layer];
  }
  return output;
}
```
- example usage
```shell
...
},

run: function(input) {
  if (this.inputLookup) {
    input = lookup.toArray(this.inputLookup, input);
  }

  var output = this.runInput(input);

  if (this.outputLookup) {
    output = lookup.toHash(this.outputLookup, output);
  }
  return output;
},
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.test"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>test (data)](#apidoc.element.brain.NeuralNetwork.prototype.test)
- description and source-code
```javascript
test = function (data) {
  data = this.formatData(data);

  // for binary classification problems with one output node
  var isBinary = data[0].output.length == 1;
  var falsePos = 0,
      falseNeg = 0,
      truePos = 0,
      trueNeg = 0;

  // for classification problems
  var misclasses = [];

  // run each pattern through the trained network and collect
  // error and misclassification statistics
  var sum = 0;
  for (var i = 0; i < data.length; i++) {
    var output = this.runInput(data[i].input);
    var target = data[i].output;

    var actual, expected;
    if (isBinary) {
      actual = output[0] > this.binaryThresh ? 1 : 0;
      expected = target[0];
    }
    else {
      actual = output.indexOf(_(output).max());
      expected = target.indexOf(_(target).max());
    }

    if (actual != expected) {
      var misclass = data[i];
      _(misclass).extend({
        actual: actual,
        expected: expected
      })
      misclasses.push(misclass);
    }

    if (isBinary) {
      if (actual == 0 && expected == 0) {
        trueNeg++;
      }
      else if (actual == 1 && expected == 1) {
        truePos++;
      }
      else if (actual == 0 && expected == 1) {
        falseNeg++;
      }
      else if (actual == 1 && expected == 0) {
        falsePos++;
      }
    }

    var errors = output.map(function(value, i) {
      return target[i] - value;
    });
    sum += mse(errors);
  }
  var error = sum / data.length;

  var stats = {
    error: error,
    misclasses: misclasses
  };

  if (isBinary) {
    _(stats).extend({
      trueNeg: trueNeg,
      truePos: truePos,
      falseNeg: falseNeg,
      falsePos: falsePos,
      total: data.length,
      precision: truePos / (truePos + falsePos),
      recall: truePos / (truePos + falseNeg),
      accuracy: (trueNeg + truePos) / data.length
    })
  }
  return stats;
}
```
- example usage
```shell
...

var beginTrain = Date.now();

var trainingStats = classifier.train(trainSet);

var beginTest = Date.now();

var testStats = classifier.test(testSet);

var endTest = Date.now();

return {
  error : testStats.error,
  misclasses: testStats.misclasses,
  trainTime : beginTest - beginTrain,
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.toFunction"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>toFunction ()](#apidoc.element.brain.NeuralNetwork.prototype.toFunction)
- description and source-code
```javascript
toFunction = function () {
  var json = this.toJSON();
  // return standalone function that mimics run()
  return new Function("input",
'  var net = ' + JSON.stringify(json) + ';\n\n\
for (var i = 1; i < net.layers.length; i++) {\n\
  var layer = net.layers[i];\n\
  var output = {};\n\
  \n\
  for (var id in layer) {\n\
    var node = layer[id];\n\
    var sum = node.bias;\n\
    \n\
    for (var iid in node.weights) {\n\
      sum += node.weights[iid] * input[iid];\n\
    }\n\
    output[id] = (1 / (1 + Math.exp(-sum)));\n\
  }\n\
  input = output;\n\
}\n\
return output;');
}
```
- example usage
```shell
...

net.fromJSON(json);
'''

You can also get a custom standalone function from a trained network that acts just like 'run()':

'''javascript
var run = net.toFunction();

var output = run({ r: 1, g: 0.4, b: 0 });

console.log(run.toString()); // copy and paste! no need to import brain.js
'''
## Streams
The network now has a [WriteStream](http://nodejs.org/api/stream.html#stream_class_stream_writable). You can train the network by
 using 'pipe()' to send the training data to the network.
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>toJSON ()](#apidoc.element.brain.NeuralNetwork.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
<span class="apidocCodeCommentSpan">  /* make json look like:
    {
      layers: [
        { x: {},
          y: {}},
        {'0': {bias: -0.98771313, weights: {x: 0.8374838, y: 1.245858},
         '1': {bias: 3.48192004, weights: {x: 1.7825821, y: -2.67899}}},
        { f: {bias: 0.27205739, weights: {'0': 1.3161821, '1': 2.00436}}}
      ]
    }
  */
</span>  var layers = [];
  for (var layer = 0; layer <= this.outputLayer; layer++) {
    layers[layer] = {};

    var nodes;
    // turn any internal arrays back into hashes for readable json
    if (layer == 0 && this.inputLookup) {
      nodes = _(this.inputLookup).keys();
    }
    else if (layer == this.outputLayer && this.outputLookup) {
      nodes = _(this.outputLookup).keys();
    }
    else {
      nodes = _.range(0, this.sizes[layer]);
    }

    for (var j = 0; j < nodes.length; j++) {
      var node = nodes[j];
      layers[layer][node] = {};

      if (layer > 0) {
        layers[layer][node].bias = this.biases[layer][j];
        layers[layer][node].weights = {};
        for (var k in layers[layer - 1]) {
          var index = k;
          if (layer == 1 && this.inputLookup) {
            index = this.inputLookup[k];
          }
          layers[layer][node].weights[k] = this.weights[layer][j][index];
        }
      }
    }
  }
  return { layers: layers, outputLookup:!!this.outputLookup, inputLookup:!!this.inputLookup };
}
```
- example usage
```shell
...

If the training error is still something huge like '0.4' after 20000 iterations, it's a good sign that the network can't make sense
 of the data you're giving it.

## JSON
Serialize or load in the state of a trained network with JSON:

'''javascript
var json = net.toJSON();

net.fromJSON(json);
'''

You can also get a custom standalone function from a trained network that acts just like 'run()':

'''javascript
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.train"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>train (data, options)](#apidoc.element.brain.NeuralNetwork.prototype.train)
- description and source-code
```javascript
train = function (data, options) {
  data = this.formatData(data);

  options = options || {};
  var iterations = options.iterations || 20000;
  var errorThresh = options.errorThresh || 0.005;
  var log = options.log || false;
  var logPeriod = options.logPeriod || 10;
  var learningRate = options.learningRate || this.learningRate || 0.3;
  var callback = options.callback;
  var callbackPeriod = options.callbackPeriod || 10;

  var inputSize = data[0].input.length;
  var outputSize = data[0].output.length;

  var hiddenSizes = this.hiddenSizes;
  if (!hiddenSizes) {
    hiddenSizes = [Math.max(3, Math.floor(inputSize / 2))];
  }
  var sizes = _([inputSize, hiddenSizes, outputSize]).flatten();
  this.initialize(sizes);

  var error = 1;
  for (var i = 0; i < iterations && error > errorThresh; i++) {
    var sum = 0;
    for (var j = 0; j < data.length; j++) {
      var err = this.trainPattern(data[j].input, data[j].output, learningRate);
      sum += err;
    }
    error = sum / data.length;

    if (log && (i % logPeriod == 0)) {
      console.log("iterations:", i, "training error:", error);
    }
    if (callback && (i % callbackPeriod == 0)) {
      callback({ error: error, iterations: i });
    }
  }

  return {
    error: error,
    iterations: i
  };
}
```
- example usage
```shell
...

# brain
'brain' is a JavaScript [neural network](http://en.wikipedia.org/wiki/Artificial_neural_network) library. Here's an example of using
 it to approximate the XOR function:

'''javascript
var net = new brain.NeuralNetwork();

net.train([{input: [0, 0], output: [0]},
           {input: [0, 1], output: [1]},
           {input: [1, 0], output: [1]},
           {input: [1, 1], output: [0]}]);

var output = net.run([1, 0]);  // [0.987]
'''
...
```

#### <a name="apidoc.element.brain.NeuralNetwork.prototype.trainPattern"></a>[function <span class="apidocSignatureSpan">brain.NeuralNetwork.prototype.</span>trainPattern (input, target, learningRate)](#apidoc.element.brain.NeuralNetwork.prototype.trainPattern)
- description and source-code
```javascript
trainPattern = function (input, target, learningRate) {
  learningRate = learningRate || this.learningRate;

  // forward propogate
  this.runInput(input);

  // back propogate
  this.calculateDeltas(target);
  this.adjustWeights(learningRate);

  var error = mse(this.errors[this.outputLayer]);
  return error;
}
```
- example usage
```shell
...
var sizes = _([inputSize, hiddenSizes, outputSize]).flatten();
this.initialize(sizes);

var error = 1;
for (var i = 0; i < iterations && error > errorThresh; i++) {
  var sum = 0;
  for (var j = 0; j < data.length; j++) {
    sum += this.trainPattern(data[j].input, data[j].output);
  }
  error = sum / data.length;
}

return {
  error: error,
  iterations: i
...
```



# <a name="apidoc.module.brain.lookup"></a>[module brain.lookup](#apidoc.module.brain.lookup)

#### <a name="apidoc.element.brain.lookup.buildLookup"></a>[function <span class="apidocSignatureSpan">brain.lookup.</span>buildLookup (hashes)](#apidoc.element.brain.lookup.buildLookup)
- description and source-code
```javascript
function buildLookup(hashes) {
  // [{a: 1}, {b: 6, c: 7}] -> {a: 0, b: 1, c: 2}
  var hash = _(hashes).reduce(function(memo, hash) {
    return _(memo).extend(hash);
  }, {});
  return lookupFromHash(hash);
}
```
- example usage
```shell
...
  }
},

formatData: function(data) {
  // turn sparse hash input into arrays with 0s as filler
  if (!_(data[0].input).isArray()) {
    if (!this.inputLookup) {
      this.inputLookup = lookup.buildLookup(_(data).pluck("input"));
    }
    data = data.map(function(datum) {
      var array = lookup.toArray(this.inputLookup, datum.input)
      return {input: array, output: datum.output};
    }, this);
  }
...
```

#### <a name="apidoc.element.brain.lookup.lookupFromArray"></a>[function <span class="apidocSignatureSpan">brain.lookup.</span>lookupFromArray (array)](#apidoc.element.brain.lookup.lookupFromArray)
- description and source-code
```javascript
function lookupFromArray(array) {
  var lookup = {};
  // super fast loop
  var z = 0;
  var i = array.length;
  while (i-- > 0) {
    lookup[array[i]] = z++;
  };
  return lookup;
}
```
- example usage
```shell
...
TrainStream.prototype.finishStreamIteration = function() {
  if (this.dataFormatDetermined && this.size !== this.count) {
console.log("This iteration's data length was different from the first.");
  }

  if (!this.dataFormatDetermined) {
// create the lookup
this.neuralNetwork.inputLookup = lookup.lookupFromArray(this.inputKeys);
this.neuralNetwork.outputLookup = lookup.lookupFromArray(this.outputKeys);

var data = this.neuralNetwork.formatData(this.firstDatum);
var inputSize = data[0].input.length;
var outputSize = data[0].output.length;

var hiddenSizes = this.hiddenSizes;
...
```

#### <a name="apidoc.element.brain.lookup.lookupFromHash"></a>[function <span class="apidocSignatureSpan">brain.lookup.</span>lookupFromHash (hash)](#apidoc.element.brain.lookup.lookupFromHash)
- description and source-code
```javascript
function lookupFromHash(hash) {
  // {a: 6, b: 7} -> {a: 0, b: 1}
  var lookup = {};
  var index = 0;
  for (var i in hash) {
    lookup[i] = index++;
  }
  return lookup;
}
```
- example usage
```shell
...
    this.weights = new Array(size);
    this.biases = new Array(size);
    this.outputs = new Array(size);

    for (var i = 0; i <= this.outputLayer; i++) {
var layer = json.layers[i];
if (i == 0 && !layer[0]) {
  this.inputLookup = lookup.lookupFromHash(layer);
}
else if (i == this.outputLayer && !layer[0]) {
  this.outputLookup = lookup.lookupFromHash(layer);
}

var nodes = _(layer).keys();
this.sizes[i] = nodes.length;
...
```

#### <a name="apidoc.element.brain.lookup.toArray"></a>[function <span class="apidocSignatureSpan">brain.lookup.</span>toArray (lookup, hash)](#apidoc.element.brain.lookup.toArray)
- description and source-code
```javascript
function toArray(lookup, hash) {
  // {a: 0, b: 1}, {a: 6} -> [6, 0]
  var array = [];
  for (var i in lookup) {
    array[lookup[i]] = hash[i] || 0;
  }
  return array;
}
```
- example usage
```shell
...
    }
  }
}
  },

  run: function(input) {
if (this.inputLookup) {
  input = lookup.toArray(this.inputLookup, input);
}

var output = this.runInput(input);

if (this.outputLookup) {
  output = lookup.toHash(this.outputLookup, output);
}
...
```

#### <a name="apidoc.element.brain.lookup.toHash"></a>[function <span class="apidocSignatureSpan">brain.lookup.</span>toHash (lookup, array)](#apidoc.element.brain.lookup.toHash)
- description and source-code
```javascript
function toHash(lookup, array) {
  // {a: 0, b: 1}, [6, 7] -> {a: 6, b: 7}
  var hash = {};
  for (var i in lookup) {
    hash[i] = array[lookup[i]];
  }
  return hash;
}
```
- example usage
```shell
...
  if (this.inputLookup) {
    input = lookup.toArray(this.inputLookup, input);
  }

  var output = this.runInput(input);

  if (this.outputLookup) {
    output = lookup.toHash(this.outputLookup, output);
  }
  return output;
},

runInput: function(input) {
  this.outputs[0] = input;  // set output state of input layer
...
```



# <a name="apidoc.module.brain.neuralnetwork"></a>[module brain.neuralnetwork](#apidoc.module.brain.neuralnetwork)

#### <a name="apidoc.element.brain.neuralnetwork.NeuralNetwork"></a>[function <span class="apidocSignatureSpan">brain.neuralnetwork.</span>NeuralNetwork (options)](#apidoc.element.brain.neuralnetwork.NeuralNetwork)
- description and source-code
```javascript
NeuralNetwork = function (options) {
  options = options || {};
  this.learningRate = options.learningRate || 0.3;
  this.momentum = options.momentum || 0.1;
  this.hiddenSizes = options.hiddenLayers;

  this.binaryThresh = options.binaryThresh || 0.5;
}
```
- example usage
```shell
...



# brain
'brain' is a JavaScript [neural network](http://en.wikipedia.org/wiki/Artificial_neural_network) library. Here's an example of using
 it to approximate the XOR function:

'''javascript
var net = new brain.NeuralNetwork();

net.train([{input: [0, 0], output: [0]},
           {input: [0, 1], output: [1]},
           {input: [1, 0], output: [1]},
           {input: [1, 1], output: [0]}]);

var output = net.run([1, 0]);  // [0.987]
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
