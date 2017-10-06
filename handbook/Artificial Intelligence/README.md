## [Artificial Intelligence](https://en.wikipedia.org/wiki/Artificial_intelligence)
* [Machine Learning](https://en.wikipedia.org/wiki/Machine_learning)
  * Courses
    * [Machine Learning](https://www.cs.ox.ac.uk/people/nando.defreitas/machinelearning/) [www.cs.ox.ac.uk]
    * [Coursera: Machine Learning](https://www.coursera.org/learn/machine-learning) [www.coursera.org]
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
  * [Regression](https://en.wikipedia.org/wiki/Regression_analysis)
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
