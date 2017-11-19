## [Mathematics](https://en.wikipedia.org/wiki/Mathematics)

### [Linear Algebra](https://en.wikipedia.org/wiki/Linear_algebra)

* [Scalar](https://en.wikipedia.org/wiki/Scalar_(mathematics)) a, [Vector](https://en.wikipedia.org/wiki/Vector_(mathematics_and_physics)) **a**, [Matrix](https://en.wikipedia.org/wiki/Matrix_(mathematics)) **A**
* [Matrix Multiplication](https://en.wikipedia.org/wiki/Matrix_multiplication)

![Schematic depiction of the matrix product AB of two matrices A and B.](https://upload.wikimedia.org/wikipedia/commons/e/eb/Matrix_multiplication_diagram_2.svg)

* [Principal component analysis](https://en.wikipedia.org/wiki/Principal_component_analysis)
* [Norm](https://en.wikipedia.org/wiki/Norm_(mathematics))
  * L1 Norm: red line
  * L2 Norm: green line

![Taxicab geometry versus Euclidean distance: In taxicab geometry, the red, yellow, and blue paths all have the shortest length of 12. In Euclidean geometry, the green line has length , and is the unique shortest path.](https://upload.wikimedia.org/wikipedia/commons/0/08/Manhattan_distance.svg)

### [Calculus](https://en.wikipedia.org/wiki/Calculus)
* [Derivitave](https://en.wikipedia.org/wiki/Derivative)
  * [Partial Derivitave](https://en.wikipedia.org/wiki/Partial_derivative)
  * [Gradient](https://en.wikipedia.org/wiki/Gradient)
    * [numpy.gradient](https://docs.scipy.org/doc/numpy/reference/generated/numpy.gradient.html) [docs.scipy.org])
  * [Jacobian](https://en.wikipedia.org/wiki/Jacobian_matrix_and_determinant)
  * [Hessian](https://en.wikipedia.org/wiki/Hessian_matrix): Second Derivitave
  * [Directional Derivitave](https://en.wikipedia.org/wiki/Directional_derivative)
  * [Matrix Calculus](http://www.matrixcalculus.org) [www.matrixcalculus.org]
* [Integral](https://en.wikipedia.org/wiki/Integral)

### [Graphs](https://en.wikipedia.org/wiki/Graph_(discrete_mathematics))
* [Degree distribution](https://en.wikipedia.org/wiki/Degree_distribution)

### [Statistics](https://en.wikipedia.org/wiki/Statistics)

* Definations
  * Probability: likelihood an event will occur, 0 -> 1, deductive, Population -> Sample, small -> big
  * Statistics: data analysis, inductive, Sample -> Population, big -> small
  * [Population](https://en.wikipedia.org/wiki/Statistical_population): collection of objects or units of interest
  * [Sample](https://en.wikipedia.org/wiki/Sample_(statistics)): subset of a population - easier, cheaper, more practical than whole population
  * [Primary Source](https://en.wikipedia.org/wiki/Primary_source)
    * Observation
    * Experimentation
    * Survey
  * [Secondary Source](https://en.wikipedia.org/wiki/Secondary_source)
    * Previous Studies
  * [Qualitative](https://en.wikipedia.org/wiki/Qualitative_property): groups, categories
  * [Quantitative](https://en.wikipedia.org/wiki/Quantity): numerical
    * [Discrete](https://en.wikipedia.org/wiki/Discrete-time_signal) e.g. number of passengers in a vehicle
    * [Continious](https://en.wikipedia.org/wiki/Continuous_signal) e.g. velocity of a vehicle
  * [Deterministic](https://en.wikipedia.org/wiki/Deterministic_system) =  no randomness
  * [Stochastic](https://en.wikipedia.org/wiki/Stochastic) = randomly determined
* Descriptive Statistics: summary and description
  * Visual Data Analysis
    * Good Practices
      * Clear Labels: Title, Variables, Axes, Units, Legends
        * drive the reader’s focus, less is more, gray > black
      * Identify Sources and Dates of Data
      * Color
        * [Adobe Color](https://color.adobe.com) [color.adobe.com]
        * [Hue](https://en.wikipedia.org/wiki/Hue) is important
        * May be printed in [black and white](https://en.wikipedia.org/wiki/Black_and_white)
        * people are [colorblind](https://en.wikipedia.org/wiki/Color_blindness)
        * [Projectors](https://en.wikipedia.org/wiki/Projector) are not good
        * Less is more, limit to 5-7 colors
      * Scale: start bar (and area) charts at 0, use round numbers
    * Tables
    * [Stem-and-leaf Displays](https://en.wikipedia.org/wiki/Stem-and-leaf_display)
      * 8 | 00 15 30 45
      * 9 | 00 30
    * [Dot Plots](https://en.wikipedia.org/wiki/Dot_plot_(statistics))
      * 8 | \*\*\*\*
      * 9 | \*\*
    * [Histograms](https://en.wikipedia.org/wiki/Histogram)
      * Determine Class/Bin Size: Number of Classes ≈ sqrt(number of observations)
      * Determine Frequency or Relative Frequency (normalized)
    * [Box Plot](https://en.wikipedia.org/wiki/Box_plot)
      * min \*-----[ | ]-----\* max
      * box is lower quarter (median of lower half), median, upper quarter (median of upper half)
    * [Parallel Coordinates](https://en.wikipedia.org/wiki/Parallel_coordinates) (and slope graphs)
    * [Heatmaps](https://en.wikipedia.org/wiki/Heat_map)
    * [Dendrogram](https://en.wikipedia.org/wiki/Dendrogram)
    * [Bar chart](https://en.wikipedia.org/wiki/Bar_chart)
    * [Line chart](https://en.wikipedia.org/wiki/Line_chart): data over time
    * Examples
      * [D3 Gallery](https://github.com/d3/d3/wiki/Gallery) [github.com]
      * [Matplotlib Examples](http://matplotlib.org/examples/index.html) [matplotlib.org]
      * [The Python Graph Gallery](https://python-graph-gallery.com) [python-graph-gallery]
      * [Awesome dataviz](https://github.com/fasouto/awesome-dataviz) [github.com]
  * [Summary Measures](https://en.wikipedia.org/wiki/Summary_statistics)
    * [Anscombe's quartet](https://en.wikipedia.org/wiki/Anscombe%27s_quartet)
    
    ![All four sets are identical when examined using simple summary statistics, but vary considerably when graphed
](https://upload.wikimedia.org/wikipedia/commons/e/ec/Anscombe%27s_quartet_3.svg)
    
    * Location [Central Tendency](https://en.wikipedia.org/wiki/Central_tendency))
      * [Mean](https://en.wikipedia.org/wiki/Mean) (Average) = (x₁ + x₂) / n
        * sensative to [Outliers](https://en.wikipedia.org/wiki/Outlier) (observations w/ extreme values)
        * will generally larger than median because of outliers, but not always
          * [Trimmed Mean](https://en.wikipedia.org/wiki/Truncated_mean) = eliminate the smallest 10% and the largest 10%
      * [Median](https://en.wikipedia.org/wiki/Median) Half the date on either side
        * not sensative to outliers
        * [Quartiles](https://en.wikipedia.org/wiki/Quartile) divide data into four equal parts
        * [Percentiles](https://en.wikipedia.org/wiki/Percentile) divide the data into 100 equal parts e.g. 99%
      * [Mode](https://en.wikipedia.org/wiki/Mode_(statistics))
    * Variation ([Statistical Dispersion](https://en.wikipedia.org/wiki/Statistical_dispersion))
      * [Range](https://en.wikipedia.org/wiki/Range_(statistics)) = xmax - xmin
      * [Deviation](https://en.wikipedia.org/wiki/Deviation_(statistics)) from Mean = mean - xi
      * [Unbiased Sample Variance](https://en.wikipedia.org/wiki/Variance) s = 1 / (N - 1) × Σ(( Deviation from the Mean of xi )²)
        * [Standard Deviation](https://en.wikipedia.org/wiki/Standard_deviation) = sqrt(variance)
          * Add c to all values, same standard deviation
          * Multiply all values by c, new standard deviation = old standard deviation × c²
      * Population Variance = σ² = Σ(( Deviation from the Mean of xi )²) / N
        * Coefficient of Variation = Variance / Population Mean
          * Estimated Coefficient of Variation = Sample Variance / Sample Mean
    * Shape
      * [Skewness](https://en.wikipedia.org/wiki/Skewness)
      * [Kurtosis](https://en.wikipedia.org/wiki/Kurtosis)
    * Moments
      * Sample Mean
      * Variance
      * Skewness
      * Kurtosis
* Inferential Statistics: generalizing from a sample to a population
* [Likelihood function](https://en.wikipedia.org/wiki/Likelihood_function)
  * [Likelihood principle](https://en.wikipedia.org/wiki/Likelihood_principle)
* [Simpson's_paradox](https://en.wikipedia.org/wiki/Simpson%27s_paradox)

![Simpson's paradox for quantitative data: a positive trend appears for two separate groups, whereas a negative trend appears when the groups are combined.](https://upload.wikimedia.org/wikipedia/commons/4/47/Simpson%27s_paradox_continuous.svg)

* References
  * [NIST/SEMATECH e-Handbook of Statistical Methods](http://www.itl.nist.gov/div898/handbook/index.htm) [www.itl.nist.gov]

### [Probability](https://en.wikipedia.org/wiki/Probability)
* Definations
    * [Experiment](https://en.wikipedia.org/wiki/Experiment_(probability_theory)): a process that generates well-defined [outcomes](https://en.wikipedia.org/wiki/Outcome_(probability))
    * [Sample Space](https://en.wikipedia.org/wiki/Sample_space): the set of all possible outcomes e.g. Heads/Tails, 6 Sides of a Die
    * Sample Point: a single outcome
    * [Event](https://en.wikipedia.org/wiki/Event_(probability_theory)): Collection of Sample Points
      * Simple: one outcome
      * Compound: more than one outcome
      * Events are Sets => [Set Theory](https://en.wikipedia.org/wiki/Set_theory)
        * [Complement](https://en.wikipedia.org/wiki/Complement_(set_theory)) = not A
        * [Union](https://en.wikipedia.org/wiki/Union_(set_theory)) = A or B
        * [Intersection](https://en.wikipedia.org/wiki/Intersection_(set_theory)) A and B
        * Mutually Exclusive (Disjoint) = have no intersection
        * Collectively Exhaustive = covers the whole sample space
      * Null Event (Impossible Event) p = 0
      * Certain Event p = 1
      * Equally Likely Outcomes
    * [Permutations](https://en.wikipedia.org/wiki/Permutation) order matters
      * permutations of n ojects = n!
      * k permutations of n objects = n!/((n - k)!)
    * [Combinations](https://en.wikipedia.org/wiki/Combination) order doesn't matter
      * combinations of k out of n objects = n!/(k! * (n - k)!)
      * e.g. poker hand = 52 choose 5 = 2,598,960 combinations
  * Visualizations
    * [Tree Diagrams](https://en.wikipedia.org/wiki/Tree_diagram_(probability_theory))
    * X-Y Plots
  * [Uncertainty](https://en.wikipedia.org/wiki/Uncertainty)
    * [Wait/Walk Dilemma](https://en.wikipedia.org/wiki/Wait/walk_dilemma)
    * Sources of Uncertainty
      * Inherent stochasticity
      * Incomplete observability
      * Incomplete modeling
* [Analysis of Variance](https://en.wikipedia.org/wiki/Analysis_of_variance) [ANOVA]
* [Hypothesis Testing](https://en.wikipedia.org/wiki/Statistical_hypothesis_testing): is the difference by chance or not?
  * [Null Hypothesis](https://en.wikipedia.org/wiki/Null_hypothesis) (H₀): no relationship between the two
  * Process
    * Choose a null hypothesis and an alternate hypothesis.
      * e.g. H₀ = there has been no change in speeds as a result of a new law. H₁ = there has been a change.
    * Calculate the appropriate test statistic.
      * (Sample Estimate - Hypothesised Value) / Standard Error of Sample Estimate
    * Refer this statistic to a known distribution if the null hypothesis were true.
    * Select a significance level. e.g. 5%
    * Calculate the probability if the null hypothesis were true = Critial Value
  * Reject or not the null hypothesis.
    * e.g if |test statistic| > critical value, reject null hypothesis
      * [Errors](https://en.wikipedia.org/wiki/Type_I_and_type_II_errors)
        * Type I: incorrect rejection of a true null hypothesis (false positive)
        * Type II: incorrectly retaining a false null hypothesis (false negative)
* [Nonparametric Tests](https://en.wikipedia.org/wiki/Nonparametric_statistics)
* Distributions
  * Properties
    * [Efficiency](https://en.wikipedia.org/wiki/Efficiency_(statistics))
    * [Consistency](https://en.wikipedia.org/wiki/Consistency_(statistics))
  * Random Variables
  * Probability Distribution (Probability Mass Function)
  * Cummulative Distribution Function
  * Expected Value = Mean Value
    * Discrete = Σ(xi × p(x))
    * Expected Value(h(X)) = Σ(h(x) × p(x))
  * Discrete Distributions
    * [Bernoulli](https://en.wikipedia.org/wiki/Bernoulli_distribution)
      * 1 = success, 0 = failure
    * [Binomial](https://en.wikipedia.org/wiki/Binomial_distribution)
      * e.g. arrival of vehicles in free flow, low density, small random sample
    * [Poisson](https://en.wikipedia.org/wiki/Poisson_distribution)
      * e.g. arrival of vehicles in free flow, low density, medium random sample
  * Continuous Distributions
    * [Uniform Distribution](https://en.wikipedia.org/wiki/Uniform_distribution)
      * e.g. arrival of vehicles in a platoon
    * [Normal](https://en.wikipedia.org/wiki/Normal_distribution)
      * Standard Normal
        * μ=0 and σ=1
      * e.g. arrival of vehicles in free flow, low density, large random sample; speed of vehicles
    * [Shifted Negative Exponential Distribution](https://en.wikipedia.org/wiki/Exponential_distribution)
      * e.g. arrival of vehicles in free flow, low density, medium random sample
    * [Logarithmic Normal Distribution](https://en.wikipedia.org/wiki/Log-normal_distribution)
      * e.g. arrival of vehicles in free flow, low density, medium random sample
  * Jointly Distributed Random Variables
    * [Sampling](https://en.wikipedia.org/wiki/Sampling_%28statistics%29)
      * Methods
        * Random Sampling - impossible
        * Systematic Sampling - e.g. pick every 10th
        * Stratified Sampling - group the population and sample from the groups at a ratio equal to their representation
        * Enriched Sampling - stratified, but seek out people you need
      * [Standard Error](https://en.wikipedia.org/wiki/Sampling_error) = sqrt((Population Size - Sample Size) × (Sample Variance)² / (Population Size × Sample Size))
        * Estimate = Sample Variance / sqrt(Sample Size) => we want a big sample size if possible
        * Depends on Sample Variance which we known only after we collect the data
        * When the measure is a percent > 10%, Standard Error = sqrt(Percentage Obtained from Measurement × (1 - Percentage Obtained from Measurement) / Sample Size)
* [Confidence Interval](https://en.wikipedia.org/wiki/Confidence_interval) = Sample Mean ± Confidence Interval Coefficient × Standard Error
  * Confidence Interval Coefficient for 2-sided test and confidence level 90%: 1.65, 95%: 1.96, 98%: 2.33, 99%: 2.58
* [Central Limit Theorem](https://en.wikipedia.org/wiki/Central_limit_theorem): means of samples tend to be distributed according to a normal distribution when n > 30
* Comparing Two Samples
  * Standard Error of the Distribution of the Difference of the Two Averages = sqrt((Variance₁ / Sample Size₁) + (Variance₂ / Sample Size₂))
* [Student's t-test](https://en.wikipedia.org/wiki/Student%27s_t-test)
  * Degrees of Freedom = Sample Size - 1
* [Monte Carlo Method](https://en.wikipedia.org/wiki/Monte_Carlo_method)
* [Bayes' theorem](https://en.wikipedia.org/wiki/Bayes%27_theorem)
  * P(A|B) = P(B|A) × P(A) / P(B)
* [Frequentist probability](https://en.wikipedia.org/wiki/Frequentist_probability)
* [Bayesian probability](https://en.wikipedia.org/wiki/Bayesian_probability)
