## [Artificial Intelligence](https://en.wikipedia.org/wiki/Artificial_intelligence) - [Machine Learning](https://en.wikipedia.org/wiki/Machine_learning)

### [Occam's Razor](https://en.wikipedia.org/wiki/Occam%27s_razor)
* (all else equal) simplest is best

### Courses

* [Machine Learning](https://www.cs.ox.ac.uk/people/nando.defreitas/machinelearning/) [www.cs.ox.ac.uk]
* [Coursera: Machine Learning](https://www.coursera.org/learn/machine-learning) [www.coursera.org]

### Competitions

* [Kaggle](https://www.kaggle.com) [www.kaggle.com]

### Tasks

* Formal Tasks e.g. board games
* Expert Tasks e.g. engineering design
* Mundane Tasks e.g. walking
* More Tasks: Classification, Classification with missing inputs, Regression, Transcription (OCR, Speech Recognition), Machine translation, Structured output, Anomaly detection, Synthesis and Sampling, Filling missing values, Noise removal, Density estimation, …

### Learning Types

* Supervised: provide large sample of labeled training data (ground truth: inputs and outputs); e.g. regression, classification, structured data
  * Humans can learn from much less data, simple instructions.
* [Reinforcement Learning](https://en.wikipedia.org/wiki/Reinforcement_learning): reward or punish based on just outcome, ground truth is scarce
  * [agent](https://en.wikipedia.org/wiki/Intelligent_agent) acts (decision) on environment, environment rewards or punishes agent
  
  ![Simple reflex agent](https://upload.wikimedia.org/wikipedia/commons/3/3f/IntelligentAgent-SimpleReflex.png)
  
  * End-to-end learning: combine perceptiona and decision and optimize both together
  * supervised learning -> reinforcement learning - inputs: observations; output: actions; reward: loss function
  * Model-based reinforcement learning
  * [Policy Gradient Method](https://en.wikipedia.org/wiki/Reinforcement_learning#Direct_policy_search): increase log probability when 'good' actions occur, decrease log probabilities when 'bad' actions occur
    * [Policy gradient methods](http://www.scholarpedia.org/article/Policy_gradient_methods) [www.scholarpedia.org]
  * [Markov Decision Model](https://en.wikipedia.org/wiki/Markov_decision_process): state, action, reward -> state, action, reward -> ...
  * maximize sum of future rewards (discounted because future rewards may not be realized)
  * [Q-Learning](https://en.wikipedia.org/wiki/Q-learning)
    * Exploration (try something new, see if it's fun; a random action) vs. Exploitation (keep doing what you enjoy)
      * Controlled by ε
    * [Bellman Equation](https://en.wikipedia.org/wiki/Bellman_equation)
  * Problems: Trail and Error Learning, Delayed Reward, No Specified Instructions
* Unsupervised: unlabled data; e.g. clustering, density estimation
* [Competitive Self-Play](https://blog.openai.com/competitive-self-play) [blog.openai.com]
* [Transfer Learning](https://en.wikipedia.org/wiki/Transfer_learning): use a pre-trained model as part of a new model in a different domain
* [Autoencoder](https://en.wikipedia.org/wiki/Autoencoder)
* other types of learning: demonstrations, observations

### Neural Networks (Deep Learning)

* Universality - can approximate any function e.g. driving
* Courses
  * [MIT 6.S094: Deep Learning for Self-Driving Cars](http://selfdrivingcars.mit.edu) [selfdrivingcars.mit.edu]
  * [Deep Learning](http://www.deeplearningbook.org) [www.deeplearningbook.org]
  * [Practical Deep Learning For Coders, Part 1](http://course.fast.ai) [course.fast.ai]
  * [Hacker's guide to Neural Networks](http://karpathy.github.io/neuralnets/) [karpathy.github.io]
  * [CS 294: Deep Reinforcement Learning, Fall 2017](http://rll.berkeley.edu/deeprlcourse/) [rll.berkeley.edu]
  * [Deep RL Bootcamp](https://sites.google.com/view/deep-rl-bootcamp/lectures) [sites.google.com]
  * [6.S191: Introduction to Deep Learning](http://introtodeeplearning.com) [introtodeeplearning.com]
  * [Stanford Computer Vision](https://www.youtube.com/playlist?list=PLf7L7Kg8_FNxHATtLwDceyh72QQL9pvpQ) [www.youtube.com]
  * [3Blue1Brown - Neural Networks](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) [www.youtube.com]
  * [Theories of Deep Learning (STATS 385)](https://stats385.github.io) [stats385.github.io]
  * Non-free
    * [Neural Networks and Deep Learning](https://www.coursera.org/learn/neural-networks-deep-learning) [www.coursera.org]
* Reading Lists
  * [Awesome - Most Cited Deep Learning Papers](https://github.com/terryum/awesome-deep-learning-papers) [github.com]
  * [Deep Learning Reading List](http://deeplearning.net/reading-list/) [deeplearning.net]
* Libraries
  * [TensorFlow](https://www.tensorflow.org) [www.tensorflow.org]
    * Symbol-to-symbol differientation - Can compute higher order derivatives 
  * [Keras](https://keras.io) [keras.io] / [keras.js](https://github.com/transcranial/keras-js) [github.com]
  * [Torch](http://torch.ch) [torch.ch] / [PyTorch](http://pytorch.org) [pytorch.org]
    * Symbol-to-number differentiation: Torch
  * [Theano](http://www.deeplearning.net/software/theano/) [www.deeplearning.net]
  * [mxnet](https://mxnet.incubator.apache.org) [mxnet.incubator.apache.org]
  * [neon](https://www.intelnervana.com/neon/) [www.intelnervana.com]
  * [ConvNetJS](http://cs.stanford.edu/people/karpathy/convnetjs/) [cs.stanford.edu]
  * [Caffe2](https://caffe2.ai) [caffe2.ai]
    * [Model Zoo](https://github.com/caffe2/caffe2/wiki/Model-Zoo) [github.com]
* Formats
  * [Open Neural Network Exchange](https://github.com/onnx/onnx) [github.com/onnx/onnx]
* Example Networks
  * [AlexNet](https://en.wikipedia.org/wiki/AlexNet)
  * [VGG](http://www.robots.ox.ac.uk/%7Evgg/research/very_deep/) [www.robots.ox.ac.uk]
  * ResNet
  * GoogLeNet
  * [CS231n Convolutional Neural Networks for Visual Recognition: Course Project Reports](http://cs231n.stanford.edu/reports.html) [cs231n.stanford.edu]
* Example Implementations
  * [Training a Neural Network ATARI Pong agent with Policy Gradients from raw pixels](https://gist.github.com/karpathy/a4166c7fe253700972fcbc77e4ea32c5) [gist.github.com]
  * [Demo of running NNs across different frameworks](https://github.com/ilkarman/DeepLearningFrameworks) [github.com]
  * [PyTorch implementation of Advantage Actor Critic (A2C), Proximal Policy Optimization (PPO) and Scalable trust-region method for deep reinforcement learning using Kronecker-factored approximation (ACKTR).](https://github.com/ikostrikov/pytorch-a2c-ppo-acktr) [github.com]
  * [A Neural Network Playground](http://playground.tensorflow.org) [playground.tensorflow.org]
  * [Boltzmann Machines in TensorFlow with examples](https://github.com/monsta-hd/boltzmann-machines) [github.com]
* Types
  * Multilayer Perceptron (MLP) / Deep Feedforward Networks / FeedForward Neural Networks
    * basic neural networks
    * information only travels forward = no feedback
  * [Convolutional Neural Networks](https://en.wikipedia.org/wiki/Convolutional_neural_network) (CNN, ConvNet)
    * Additional Operations
      * [Convolution](https://en.wikipedia.org/wiki/Convolution): s(t) = (x * w)(t) = Σ x(a) × w(t − a)
        * inputs -> Fourier transformation -> multiplication -> Fourier transformation -> outputs
      * Pooling (downsampling)
    * Example Input Data Types

    X | Single channel | Multichannel
    --- | --- | ---
    1-D | Audio waveform |
    2-D | Greyscale image, Audio pre-processed with Fourier transofrm | Color image
    3-D | Greyscale video, Volumetric data | Color video

    * Humans
      * light -> eye -> retina -> optic nerve -> brain -> primary visual cortex -> medial temporal lobe -> inferotemporal cortex
      * reverse correlation reveals Gabor functions -> edge detection
    * inputs have spacial (height, width, and depth (color depth, number of frames)) information e.g. image, video
    * filter that slides around the image => convolution
      * can find the feature anywhere in the image
    * allows you to find small objects in larger images
    * number of filters, stride (speed you move the filter), padding around the edges
    * pooling: downsampling
    * network architecture: input -> conv -> pooling -> conf -> pooling -> ... -> fully-connected layer -> output
    * network architecture (heatmap): input -> conv -> pooling -> conf -> pooling -> ... -> output
    * Time-delay Neural Networks
  * [Recurrent Neural Networks](https://en.wikipedia.org/wiki/Recurrent_neural_network) (RNN)
    * derived from parameter sharing
    * unfolding a state function s(t) = f(s(t−1); θ) to remove recurrance -> create a neural network from this unfolded function
    * most useful architecture (most data is time-series data)
    * have memory (state)
    * good short-term memory, but not great long-term memory
    * 1-many, many-many, many-1 (versus 1-to-1 for other types of neural networks)
    * variable input/output lengths
    * speech, video, audio
    * [Long Short-Term Memory](https://en.wikipedia.org/wiki/Long_short-term_memory) (LSTM) e.g. Video Caption Generation
      * Previous State (Data) and New Data
        * Decide what to forget (from the Previous State)
        * Decide what to remember (from the Previous State and/or New Data)
        * Decide what to output (if anything)
      * Uses: machine translation, handwriting recogntion, character-level text generation, image/video caption generation, steer sliding window, add audio to silent video, medical diagnosis, audio classification (wet road/dry road)
      * [Understanding LSTM and its diagrams](https://medium.com/mlreview/understanding-lstm-and-its-diagrams-37e2f46f1714) [medium.com]
  * [Deep Neural Networks](https://en.wikipedia.org/wiki/Deep_learning#Deep_neural_networks) (DNN)
  * [Deep Belief Networks](https://en.wikipedia.org/wiki/Deep_belief_network) (DBN)
* Components
  * Network (Directed Graph of a Depth): Inputs -> Hidden Layers -> Output Function -> Outputs
  * Neurons w/ Synapses
    * [Perceptron](https://en.wikipedia.org/wiki/Perceptron)
      * Process
        * input (1 or 0)
        * multiply by weight
        * sum + bias
        * activate (output 0 or 1)
      * can form a NAND Gate
        * logically complete (can build any function from just NAND gates)
      * activation function is a step function -> not smooth => sigmoid
  * Operations
    * [Dropout](https://en.wikipedia.org/wiki/Dropout_(neural_networks))
  * Input
    * [ImageNet](http://www.image-net.org) [www.image-net.org]: labeled images
    * [MNIST](https://en.wikipedia.org/wiki/MNIST_database): handwritten digits
    * CIFAR-10: small labeled images
    * [UCI Machine Learning Repository: Data Sets](https://archive.ics.uci.edu/ml/datasets.html) [archive.ics.uci.edu]
  * Output
    * Linear Units for [Gaussian](https://en.wikipedia.org/wiki/Normal_distribution) Output Distributions y = mx + b | h = Wᵀx + b
    * Sigmoid Units for [Bernoulli](https://en.wikipedia.org/wiki/Bernoulli_distribution) Output Distributions
    * Softmax Units for [Multinoulli](https://en.wikipedia.org/wiki/Categorical_distribution) Output Distributions
    * Class e.g. Cat, Dog
    * Probability
    * Segmentation => Heatmap of probabilities
* Training Process
  * Forward pass (compute the outputs)
    * Linear Function
    * Nonlinear Function (Activation Function)
      * [Softmax Function](https://en.wikipedia.org/wiki/Softmax_function)
      * [Rectified Linear Unit (ReLU)](https://en.wikipedia.org/wiki/Rectifier_(neural_networks)) g(z) = max{0, z}
        * Maxout Unit
      * Logistic Sigmoid discourged because gradient-based learning is difficult on the sides
      * Hyperbolic Tangent
      * radial basis function
      * softplus
      * hard tanh
  * Compute the Loss Function
  * Find the Gradient of the loss function
    * [Vanishing Gradient Problem](https://en.wikipedia.org/wiki/Vanishing_gradient_problem)
      * [Untersuchungen zu dynamischen neuronalen Netzen](http://www.bioinf.jku.at/publications/older/3804.pdf) [www.bioinf.jku.at]
  * [Backpropigate](https://en.wikipedia.org/wiki/Backpropagation
) (backward pass)
    * [A Step by Step Backpropagation Example](https://mattmazur.com/2015/03/17/a-step-by-step-backpropagation-example/) [mattmazur.com]
    * [Hebbian Theory](https://en.wikipedia.org/wiki/Hebbian_theory)
      * "Cells that fire together wire together."
  * Run the Optimization algorythm to minimize the loss function by updating weights and biases
    * Optimization algorithms
      * [Gradient Descent](https://en.wikipedia.org/wiki/Gradient_descent)
      * [Stochastic Gradient Descent](https://en.wikipedia.org/wiki/Stochastic_gradient_descent)
        * with Momentum
        * with [Nesterov's](https://en.wikipedia.org/wiki/Yurii_Nesterov) Momentum
        * with an Adaptive [Learning Rate](https://en.wikipedia.org/wiki/Learning_curve)
          * Adagrad
          * Adadelta
          * RMSProp
          * Adam
      * [An overview of gradient descent optimization algorithms](http://ruder.io/optimizing-gradient-descent/) [ruder.io]
  * Repeat if desired
* Performance
  * [Bayes Error Rate](https://en.wikipedia.org/wiki/Bayes_error_rate)
  * Underfitting
  * Overfitting
    * How to avoid overfitting:
      * Add more data
      * Data augmentation e.g. flip (usually horizontal, not vertical), stretch/compress, change the color/brightness a bit, etc.
      * Normalization e.g. Batch normalization
      * Reudce complexity e.g. Dropout
  * Capacity (e.g. polinomial degree for least squares)
    * [VC dimension](https://en.wikipedia.org/wiki/VC_dimension)
* Other
  * Sliding image approach (versus Convolutional Neural Networks)
    * Create a detector for the object of interest
    * Slide that detector around the image and look for the objects

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

### [Discrete Choice](https://en.wikipedia.org/wiki/Discrete_choice) [Modelling](https://en.wikipedia.org/wiki/Choice_modelling)
* [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression)
  * [Independence of Irrelevant Alternatives](https://en.wikipedia.org/wiki/Independence_of_irrelevant_alternatives)
  * [Independent and Identically Distributed Random Variables](https://en.wikipedia.org/wiki/Independent_and_identically_distributed_random_variables)
  * [Logit](https://en.wikipedia.org/wiki/Logit)
    * [Sigmoid](https://en.wikipedia.org/wiki/Sigmoid_function) [Logistic Function](https://en.wikipedia.org/wiki/Logistic_function)
  * [Mixed Logit](https://en.wikipedia.org/wiki/Mixed_logit)
  * [Generalized Extreme Value Distribution](https://en.wikipedia.org/wiki/Generalized_extreme_value_distribution)
  * [Maximum Likelihood Estimation](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation)
* [Probit Model](https://en.wikipedia.org/wiki/Probit_model)
  * No [Closed-form Expression](https://en.wikipedia.org/wiki/Closed-form_expression)
* References
  * [Discrete Choice Methods with Simulation](https://eml.berkeley.edu/books/choice2.html) [eml.berkeley.edu]
  * [Discrete Dependent Variable Models](http://onlinepubs.trb.org/Onlinepubs/nchrp/cd-22/v2chapter5.html) [onlinepubs.trb.org]


### [Pattern Recognition](https://en.wikipedia.org/wiki/Pattern_recognition)

* [K-nearest neighbors](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)
  * L1 diff |image1 - image2| to find the closest match (if k=1)
  * if k=2+, find the closest matches, but there are gaps
* [Kernel methods](https://en.wikipedia.org/wiki/Kernel_method)
  * [Support vector machine](https://en.wikipedia.org/wiki/Support_vector_machine)

