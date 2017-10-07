## [Artificial Intelligence](https://en.wikipedia.org/wiki/Artificial_intelligence) ([Machine Learning](https://en.wikipedia.org/wiki/Machine_learning))
### Courses
* [Machine Learning](https://www.cs.ox.ac.uk/people/nando.defreitas/machinelearning/) [www.cs.ox.ac.uk]
* [Coursera: Machine Learning](https://www.coursera.org/learn/machine-learning) [www.coursera.org]
### Tasks
* Formal Tasks e.g. board games
* Expert Tasks e.g. engineering design
* Mundane Tasks e.g. walking
### Driving Tasks
* Localization and Mapping - Where am I?
  * [Six Degrees of Freedom](https://en.wikipedia.org/wiki/Six_degrees_of_freedom)
  
![Six Degrees of Freedom](https://upload.wikimedia.org/wikipedia/commons/f/fa/6DOF_en.jpg)
  
  * [Simultaneous localization and mapping](https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping)
  * [Object Detection](https://en.wikipedia.org/wiki/Object_detection)
    * [Scale-invariant feature transform](https://en.wikipedia.org/wiki/Scale-invariant_feature_transform)
      * [Kanade–Lucas–Tomasi feature tracker](https://en.wikipedia.org/wiki/Kanade–Lucas–Tomasi_feature_tracker)
* Scene Understanding - Where is everyone else?
  * [Object Detection](https://en.wikipedia.org/wiki/Object_detection)
    * [Cascading Classifiers](https://en.wikipedia.org/wiki/Cascading_classifiers)
      * [Haar-like Features](https://en.wikipedia.org/wiki/Haar-like_feature)
    * [Convolutional Neural Networks](https://en.wikipedia.org/wiki/Convolutional_neural_network)
      * [SegNet](https://github.com/tkuanlun350/Tensorflow-SegNet) [github.com]
  * [Recurrent Neural Networks](https://en.wikipedia.org/wiki/Recurrent_neural_network)
    * temporal data e.g. sound of wet road vs. dry road
* Movement Planning - Where am I going?
* Driver State
  * Gaze: head and eyes
### Learning Types
* Supervised: provide large sample of training data (ground truth: inputs and outputs)
  * Humans can learn from much less data, simple instructions.
* [Reinforcement Learning](https://en.wikipedia.org/wiki/Reinforcement_learning): reward or punish based on just outcome, ground truth is scarce
  * [Markov Decision Model](https://en.wikipedia.org/wiki/Markov_decision_process): state, action, reward -> state, action, reward -> ...
  * maximize sum of future rewards (discounted because future rewards may not be realized)
  * [Q-Learning](https://en.wikipedia.org/wiki/Q-learning)
    * Exploration (try something new, see if it's fun; a random action) vs. Exploitation (keep doing what you enjoy)
      * Controlled by ε
    * [Bellman Equation](https://en.wikipedia.org/wiki/Bellman_equation)
* Unsupervised: no information about outputs
### Neural Networks (Deep Learning)
* Universality - can approximate any function e.g. driving
* Courses
  * [MIT 6.S094: Deep Learning for Self-Driving Cars](http://selfdrivingcars.mit.edu) [selfdrivingcars.mit.edu]
  * [Deep Learning](http://www.deeplearningbook.org) [www.deeplearningbook.org]
  * [Practical Deep Learning For Coders, Part 1](http://course.fast.ai) [course.fast.ai]
* Libraries
  * [TensorFlow](https://www.tensorflow.org) [www.tensorflow.org]
  * [Keras](https://keras.io) [keras.io] / [keras.js](https://github.com/transcranial/keras-js) [github.com]
  * [Torch](http://torch.ch) [torch.ch] / [PyTorch](http://pytorch.org) [pytorch.org]
  * [Theano](http://www.deeplearning.net/software/theano/) [www.deeplearning.net]
  * [mxnet](https://mxnet.incubator.apache.org) [mxnet.incubator.apache.org]
  * [neon](https://www.intelnervana.com/neon/) [www.intelnervana.com]
  * [ConvNetJS](http://cs.stanford.edu/people/karpathy/convnetjs/) [cs.stanford.edu]
* Types
  * Multilayer Perceptron (MLP) / Deep Feedforward Networks / FeedForward Neural Networks: information only travels forward
  * [Convolutional Neural Networks](https://en.wikipedia.org/wiki/Convolutional_neural_network) (CNN, ConvNet)
    * inputs have spacial (height, width, and depth (color depth, number of frames)) information e.g. image, video
    * filter that slides around the image => convolution
      * can find the feature anywhere in the image
    * allows you to find small objects in larger images
    * number of filters, stride (speed you move the filter), padding around the edges
    * pooling: downsampling
    * network architecture: input -> conv -> pooling -> conf -> pooling -> ... -> fully-connected layer -> output
    * network architecture (heatmap): input -> conv -> pooling -> conf -> pooling -> ... -> output
  * [Recurrent Neural Networks](https://en.wikipedia.org/wiki/Recurrent_neural_network) (RNN)
    * have memory (state)
    * 1-many, many-many, many-1 (versus 1-to-1 for other types of neural networks)
    * variable input/output lengths
    * speech, video, audio
    * Long Short-Term Memory (LSTM) e.g. Video Caption Generation
  * [Deep Neural Networks](https://en.wikipedia.org/wiki/Deep_learning#Deep_neural_networks) (DNN)
  * [Deep Belief Networks](https://en.wikipedia.org/wiki/Deep_belief_network) (DBN)
* Operations
  * Convolution
  * Pooling
  * Activation Function
  * Backpropagation
* Components
  * Neurons w/ Synapses
    * [Perceptron](https://en.wikipedia.org/wiki/Perceptron)
      * Process
        1. input (1 or 0)
        1. multiply by weight
        2. sum + bias
        3. activate (output 0 or 1)
      * can form a NAND Gate
        * logically complete (can build any function from just NAND gates)
      * activation function is a step function -> not smooth => sigmoid
  * Input
    * [ImageNet](http://www.image-net.org) [www.image-net.org]: labeled images
    * [MNIST](https://en.wikipedia.org/wiki/MNIST_database): handwritten digits
    * CIFAR-10: small labeled images
  * Output
    * Class e.g. Cat, Dog
    * Probability
    * Segmentation => Heatmap of probabilities
* Other
  * Sliding image approach (versus Convolutional Neural Networks)
    1. Create a detector for the object of interest
    2. Slide that detector around the image and look for the objects
### [Regression](https://en.wikipedia.org/wiki/Regression_analysis)
* Purpose: explain the relationship between two variables, predict 
* [Linear Regression](https://en.wikipedia.org/wiki/Linear_regression)
  * y = ax + c (+ ε)
  * [Least Squares](https://en.wikipedia.org/wiki/Least_squares)
    * [Residual Sum of Squares](https://en.wikipedia.org/wiki/Residual_sum_of_squares)
  * [Coefficient of Determination](https://en.wikipedia.org/wiki/Coefficient_of_determination) R² = 1 - Residual Sum of Squares / Total Sum of Squares, better fit = closer to 1
* [p-value](https://en.wikipedia.org/wiki/P-value) lower is better
* [Cross Validation](https://en.wikipedia.org/wiki/Cross-validation_(statistics)): split data into training and test sets. compare mean square error of test set w/ training set. they should be about the same.
  * [Correlation](https://en.wikipedia.org/wiki/Correlation_and_dependence): two things that happen or change together
    * 1 = correlated, -1 = inversely correlated, 0 = uncorrelated
    * [Causation](https://en.wikipedia.org/wiki/Causality): something causes something else
      * [Bradford-Hill criteria](https://en.wikipedia.org/wiki/Bradford_Hill_criteria)
        * Strength
        * Consistency
        * Specificity
        * Temporality
        * Biological gradient
        * Plausibility
        * Coherence
        * Experiment
        * Analogy
  * [Gauss-Markov Theorem](https://en.wikipedia.org/wiki/Gauss–Markov_theorem): if linear (expected value of ε = 0), [homoscedastic](https://en.wikipedia.org/wiki/Homoscedasticity) (constant error variance), independent (covariance between εi and εj = 0), then least squares gives the best linear unbiased estimator (BLUE)
  * Process
    * Choose independent variables.
    * Analyse the relationship between independent variable and the dependent variable.
      * If the relationship is non-linear, apply a suitable transformation. e.g. log()
    * Calculate the correlation table for all possible variable pairs.
      * If two variables are collinear, choose the one wit the hightest correlation.
    * Add variables to the model depending on if they improve model accuracy. Otherwise, reject them.
    * Finalize statistical indices of the model.
      * Coefficient of Determination
      * Standard Error of the Estimate
        * ± 1 Standard Error => 68% Confidence Interval
        * ± 2 Standard Errors => 95% Confidence Interval
    * T-Ratio compared against t-Student distribution with (Sample Size - Number of Variables) degrees of freedom
### [Pattern Recognition](https://en.wikipedia.org/wiki/Pattern_recognition)
* [K-nearest neighbors](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)
  * L1 diff |image1 - image2| to find the closest match (if k=1)
  * if k=2+, find the closest matches, but there are gaps
