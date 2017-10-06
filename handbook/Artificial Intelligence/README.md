## [Artificial Intelligence](https://en.wikipedia.org/wiki/Artificial_intelligence)
* [Machine Learning](https://en.wikipedia.org/wiki/Machine_learning)
  * Courses
    * [Machine Learning](https://www.cs.ox.ac.uk/people/nando.defreitas/machinelearning/) [www.cs.ox.ac.uk]
    * [Coursera: Machine Learning](https://www.coursera.org/learn/machine-learning) [www.coursera.org]
    * [MIT 6.S094: Deep Learning for Self-Driving Cars](http://selfdrivingcars.mit.edu) [selfdrivingcars.mit.edu]
    * [Deep Learning](http://www.deeplearningbook.org) (www.deeplearningbook.org)
  * Tasks
    * Formal Tasks e.g. board games
    * Expert Tasks e.g. engineering design
    * Mundane Tasks e.g. walking
  * Driving Tasks
    * Localization and Mapping - Where am I?
    * Scene Understanding - Where is everyone else?
    * Movement Planning - Where am I going?
    * Driver State
  * Neural Networks (Deep Learning)
    * Universality - can approximate any function e.g. driving
    * Libraries
      * [TensorFlow](https://www.tensorflow.org) [www.tensorflow.org]
      * [Keras](https://keras.io) [keras.io] / [keras.js](https://github.com/transcranial/keras-js) [github.com]
      * [Torch](http://torch.ch) [torch.ch] / [PyTorch](http://pytorch.org) [pytorch.org]
      * [Theano](http://www.deeplearning.net/software/theano/) [www.deeplearning.net]
      * [mxnet](https://mxnet.incubator.apache.org) [mxnet.incubator.apache.org]
      * [neon](https://www.intelnervana.com/neon/) [www.intelnervana.com]
      * [ConvNetJS](http://cs.stanford.edu/people/karpathy/convnetjs/) [cs.stanford.edu]
    * Types
      * Multilayer Perception (MLP)
      * Deep Neural Networks (DNN)
      * Recurrent Neural Networks (RNN): map a sequence to another sequence (versus 1-to-1)
        * Long Short-Term Memory (LSTM) e.g. Video Caption Generation
      * Convolutional Neural Networks (CNN, ConvNet)
      * Deep Belief Networks (DBN)
    * Operations
      * Convolution
      * Pooling
      * Activation Function
      * Backpropagation
    * Components
      * Neurons
      * Synapses
      * [Perceptron](https://en.wikipedia.org/wiki/Perceptron)
        1. weight
        2. sum
        3. activate
      * Input
        * [ImageNet](http://www.image-net.org) [www.image-net.org]
      * Output
        * Class e.g. Cat, Dog
        * Probability
        * Segmentation => Heatmap of probabilities
    * Learning Types
      * Supervised: provide large sample of training data (ground truth: inputs and outputs)
        * Humans can learn from much less data, simple instructions.
      * Reinforcement Learning: reward or punish based on just outcome, ground truth is scarce
      * Unsupervised: no information about outputs
    * Other
      * Sliding image approach (versus Convolutional Neural Networks)
        1. Create a detector for the object of interest
        2. Slide that detector around the image and look for the objects
