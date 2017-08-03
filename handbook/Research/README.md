## Research
  * [Geographic Information Systems](https://en.wikipedia.org/wiki/Geographic_information_system) (GIS)
    * Geoinformation: where, what, how much, how, why
      * Categories
        * Entities: things (discrete objects) e.g. cities, roads, rivers
        * Phenomena: dynamic things (temporal continuity) e.g. fires, floods, urban growth
        * Fields: functions (spatially continuity) e.g. elevation, temperature, soil moisture
      * 7 Dimensions
        * 3 Space: coordinates, address
        * Time: time
        * Themematic Layers
          * Settlement
          * Water
          * Boundaries
          * Vegetation
          * Human e.g. Yelp
        * Scale/Resolution: level of detail
          * Spatial resolution: minimum size of an object that is discernable
            * Sampling rate: how often we sample when moving over the area
          * Temporal resolution: minimum duration of event that is discernable
            * Temporal sampling rate: how often we sample in time
          * Thematic resolution: e.g. building / non building versus restaurant/park/grocery store/school/etc; greyscale/color
        * Quality: difference from reality
          * Accuracy: discrepancy between data and reality
            * Spatial accuracy: positional accuracy
            * Temporal accuracy: currentness
            * Thematic accuracy
              * Quantitative: mismeasurement
              * Errors of omission: missing from a class
              * Errors of comission: assigned to wrong class
        * Data Quality
          * often provided by a specification including format and metadata
          * Quality
          * Scale/Resolution
          * Consistency: free from conflict
            * Spatial consistency e.g. only one road can be along one line
            * Temporal consistency e.g. only one thing can happen at a time
            * Thematic consistency e.g. population where there are no houses
          * Completeness
            * Data completeness: between data and specificationn
            * Model completeness: does it work well enough for the use case
            * Attribute completeness: are attributes all encoded?
            * Value completeness: are values all there?
      * Properties of Geoinformation
        * [First Law of Geography](https://en.wikipedia.org/wiki/Tobler%27s_first_law_of_geography): "everything is related to everything else, but near things are more related than distant things" (autocorrelation)
          * applies spatially and temporally
        * spatial heterogeneity: conditions in one place are not the same other places
        * thematic dependence: thematic layers in an area may be correlated
        * localization: information in a place is of greater importance to people in that place
          * [Friction of Distance](https://en.wikipedia.org/wiki/Friction_of_distance)
      * Views
        * Mathematical
          * [Euclidean Space](https://en.wikipedia.org/wiki/Euclidean_geometry)
            * distance = sqrt((x₁ - x₂)²) + (y₁ - y₂)²) 
          * [Gridded Space](https://en.wikipedia.org/wiki/Grid_plan) (Manhattan or [Taxicab](https://en.wikipedia.org/wiki/Taxicab_geometry))
            * distance = |xi - xj| + |yi - yj|
        * Ontological: We focus on mesoscopic.
        * Physical - Real World
        * Philosophical
        * Cognitive and Socio-Cultural: We each form our own mental map. e.g. bike lanes, freeways, public transit, localized to our home
      * Spatial Representation
        * [Georeferenced](https://en.wikipedia.org/wiki/Georeferencing)
        * Nodes (0D), Lines (1D), and Polygons (2D)
        * Raster (Pixels or [Voxels](https://en.wikipedia.org/wiki/Voxel), Vector
        * Process Modeling
          * [Finite Difference Model](https://en.wikipedia.org/wiki/Finite_difference_method)
          * [Finite Element Model](https://en.wikipedia.org/wiki/Finite_element_method)
            * gives finite number of closed areas (usually triangles)
            * usually use average of nodes (or can use node value)
          * provides iso-lines
        * [Spatial Realtions](https://en.wikipedia.org/wiki/Spatial_relation)
          * Distance
            * Measured
            * Near, Far
          * Direction
            * Degrees
            * North, South, East, West
          * 8 Topological relations between two polygons
            * disjoint
            * meet
            * contains
            * covers
            * overlap
            * equal
            * inside
            * coveredBy
          * 9 Intersections: A-interior, A-boundary, A-exterior Union B-interior, B-boundary, B-exterior
      * Temporal Representation
        * Things change over time.
        * Branching: we can predict the past and the future, but only the present is known now.
        * Patterns: random, monotonic, periodic, deteriorate, expand/shrink, deform, split/merge
        * Characteristics
          * Rate: fast/slow, sudden/gradual
          * Frequency: periodic, majorative, sporatic, once
          * Amplitude: large/small
        * Units: [chronons](https://en.wikipedia.org/wiki/Chronon), seconds, minutes, days, seasons
        * Associations: before, equals, meets, overlaps, during, starts, ends
        * Combinations: binary relations e.g. union
        * Transformations
        * Methods
          * Location-based
            * snapshots
            * temporal grid
          * Entity-based: record any time an entity is created or destroyed
          * Time-based: record all events occuring between certain times
      * Data Structures
        * Array
        * Stack (LIFO) and Queue (FIFO)
        * Linked List
          * Single Linked List: A -> B
          * Double Linked List: A <=> B
          * Circularly Linked List: A -> B -> A
        * Tree
          * height: max measure going down
          * depth: max measure going up
        * Graph (Network): vertices (nodes) are connected by edges (links)
      * Index Methods
        * Unordered O(n)
        * Index O(log n)
          * [B-tree](https://en.wikipedia.org/wiki/B-tree)
            * [R-tree](https://en.wikipedia.org/wiki/R-tree)
          * [Space-filling Curves](https://en.wikipedia.org/wiki/Space-filling_curve):
            * row
            * row-prime
            * [morton](https://en.wikipedia.org/wiki/Z-order_curve): nearby objects are located closer to each other
              * Procedure for (10,7)
                * Write coordinates in binary form. 10 => 1010, 7 => 0111
                * Interleave the digits => 10011101
                * Convert to base 10 => 157
          * [k-d tree](https://en.wikipedia.org/wiki/K-d_tree)
    * [Geoinformatics](https://en.wikipedia.org/wiki/Geoinformatics): art, science, engineering, techonogy of geoinformation
      * Purpose: determine relationships between spatial observations
      * Pitfalls
        * First Law of Geography / Autocorrelation
        * Modifiable Areal Unit Problem: we group things in unnatural ways e.g. census blocks
        * The Ecological Fallacy: judge all individuals based on groupings e.g. if high crime occurs in low income areas, this does not mean low income people are more likely to commit crime
        * Scale: scale changes how we see things
        * Nonuniformity: clusters change how we see things
        * Edge effects at artificial boundaries
      * Workflow
        * Spatial Data Modeling
          * Acquisition
            * Satellite
              * Camera
                * [Landsat 8](https://en.wikipedia.org/wiki/Landsat_8) (USA: NASA/USGS)
                * [IKONOS](https://en.wikipedia.org/wiki/Ikonos) (USA: DigitalGlobe)
                * [QuickBird](https://en.wikipedia.org/wiki/QuickBird) (USA)
                * [SPOT](https://en.wikipedia.org/wiki/SPOT_(satellite)) (FR)
                * [RapidEye](https://en.wikipedia.org/wiki/RapidEye) (DE)
                * [TanDEM-X](https://en.wikipedia.org/wiki/TanDEM-X) (DE: DLR)
              * [Geodesy](https://en.wikipedia.org/wiki/Geodesy)
                * [Global Positioning System](https://en.wikipedia.org/wiki/Global_Positioning_System) (GPS)
                * [Galielo](https://en.wikipedia.org/wiki/Galileo_(satellite_navigation))
                * [GLONASS](https://en.wikipedia.org/wiki/GLONASS)
                * [BeiDou Navigation Satellite System](https://en.wikipedia.org/wiki/BeiDou_Navigation_Satellite_System)
                * [Indian Regional Navigation Satellite System](https://en.wikipedia.org/wiki/Indian_Regional_Navigation_Satellite_System)
          * Integration
          * Updating
        * Spatial Data Handling
          * Visualization
          * [Analysis](https://en.wikipedia.org/wiki/Spatial_analysis#Spatial_dependency_or_auto-correlation)
            * Analysis of Point Patterns
              * Distance
                * Adjacency: share a boundary or w/in a distance
                * Interaction: similar to a gravity function (See Trip Distribution)
                * Neighborhood
              * Spatial Autocorrelation Measures
                * [Moran's I](https://en.wikipedia.org/wiki/Moran%27s_I)
                  * I = 0 => independent
                  * I > 0 => positive autocorrelation
                  * I < 0 => negative autocorrelation
                * [Geary's C](https://en.wikipedia.org/wiki/Geary%27s_C)
                  * C = 1 => independent
                  * C < 1 => positive autocorrelation
                  * C > 1 => negative autocorrelation
            * Geostatistics
              * [Variograms](https://en.wikipedia.org/wiki/Variogram): shows the threshold where there is autocorrelation
                * Semivariogram
                * Covariogram
              * Interpolation Methods
                * Local
                  * [Thiessen Polygons](https://en.wikipedia.org/wiki/Voronoi_diagram): each new point gets the value of the nearest sample point
                  * [Inverse Distance Weighting](https://en.wikipedia.org/wiki/Inverse_distance_weighting): new point gets a value based on its neighbors and their distance
                * Global
                  * Density Maps: [Kernel Density Estimation](https://en.wikipedia.org/wiki/Kernel_density_estimation)
                  * [Trend Surfaces](https://en.wikipedia.org/wiki/Trend_surface_analysis)
                  * [Regression Analysis](https://en.wikipedia.org/wiki/Regression_analysis) e.g. Linear Regression y = mx + b
                  * [Kriging](https://en.wikipedia.org/wiki/Kriging): fit within a confidence interval assuming autocorrelation
            * Vertical Analysis
              * Map Algebra (on multiple layers)
                * Boolean Operators e.g. AND, OR, NOT
                * Algebraic Operators e.g. +, -, *, /, log, etc.
              * Slope and Aspect e.g. Does the terrain slope north, south, etc?
                * Gradiant: each cell has 8 neighbors (n, s, e, w, ne, nw, se, sw)
                * Flow Analysis for Hydrology
                  * Assumptions
                    * water flows follow topology
                    * water is evenly distributed
                    * inflitration is zero
                    * evaporation is zero
                    * surface is bare
                  * Process
                    * Find the hightes point
                    * Fout = Fin + Flocal, Fin = from other cells, Flocal = rain
                    * Send the flow to the neighboring cell based on slope gradiant
                    * Repeat
              * Line of Sight
            * Network Analysis
              * [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm) (See Routing)
              * [Minimum Spanning Tree](https://en.wikipedia.org/wiki/Minimum_spanning_tree)
              * Least Cost Path
              * Cellular Models e.g. [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)
        * Quality Assessment
    * [Geographic Information System](https://en.wikipedia.org/wiki/Geographic_information_system): tools + display + database
      * [GIS Software](https://en.wikipedia.org/wiki/List_of_geographic_information_systems_software)
    * Cartography Design
      * https://blogs.esri.com/esri/arcgis/2011/10/28/design-principles-for-cartography/
  * [Probability](https://en.wikipedia.org/wiki/Probability) and [Statistics](https://en.wikipedia.org/wiki/Statistics)
    * Definations
      * Probability: likelihood an event will occur, 0 -> 1, deductive, Population -> Sample
      * Statistics: data analysis, inductive, Sample -> Population
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
      * [Uncertainty](https://en.wikipedia.org/wiki/Uncertainty)
        * [Wait/Walk Dilemma](https://en.wikipedia.org/wiki/Wait/walk_dilemma)
    * Descriptive Statistics: summary and description
      * Visual Data Analysis
        * Good Practices
          * Clear Labels
            * Title
            * Variables
            * Axes
            * Units
          * Identify Sources and Dates of Data
        * Keep in Mind
          * May be printed in black and white and people are colorblind
          * Projectors are not good 
          * Less is more
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
        * [Parallel Coordinates](https://en.wikipedia.org/wiki/Parallel_coordinates)
        * [Heatmaps](https://en.wikipedia.org/wiki/Heat_map)
        * [Dendrogram](https://en.wikipedia.org/wiki/Dendrogram)
            * [Summary Measures](https://en.wikipedia.org/wiki/Summary_statistics)
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
        * Variation ([Statistical Dispersion](https://en.wikipedia.org/wiki/Statistical_dispersion)
          * [Range](https://en.wikipedia.org/wiki/Range_(statistics)) = xmax - xmin
          * [Deviation](https://en.wikipedia.org/wiki/Deviation_(statistics)) from Mean = mean - xi
          * [Unbiased Sample Variance](https://en.wikipedia.org/wiki/Variance) s = 1 / (N - 1) * Σ(( Deviation from the Mean of xi )²)
            * [Standard Deviation](https://en.wikipedia.org/wiki/Standard_deviation) = sqrt(variance)
              * Add c to all values, same standard deviation
              * Multiply all values by c, new standard deviation = old standard deviation * c²
          * Population Variance = σ² = Σ(( Deviation from the Mean of xi )²) / N
            * Coefficient of Variation = Variance / Population Mean
              * Estimated Coefficient of Variation = Sample Variance / Sample Mean
        * Shape
          * [Skewness](https://en.wikipedia.org/wiki/Skewness)
          * [Kurtosis](https://en.wikipedia.org/wiki/Kurtosis)
        * Moments
          1. Sample Mean
          2. Variance
          3. Skewness
          4. Kurtosis
          * Inferential Statistics: generalizing from a sample to a population
      * Probability
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
      * [Analysis of Variance](https://en.wikipedia.org/wiki/Analysis_of_variance) [ANOVA]
      * [Hypothesis Testing](https://en.wikipedia.org/wiki/Statistical_hypothesis_testing): is the difference by chance or not?
        * [Null Hypothesis](https://en.wikipedia.org/wiki/Null_hypothesis) (H₀): no relationship between the two
        * Process
          * Choose a null hypothesis and an alternate hypothesis.
            * e.g. H₀ = there has been no chnage in speeds as a result of a new law. H₁ = there has been a change.
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
        * Random Variables
        * Probability Distribution (Probability Mass Function)
        * Cummulative Distribution Function
        * Expected Value = Mean Value
          * Discrete = Σ(xi * p(x))
          * Expected Value(h(X)) = Σ(h(x) * p(x))
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
            * [Standard Error](https://en.wikipedia.org/wiki/Sampling_error) = sqrt((Population Size - Sample Size) * (Sample Variance)² / (Population Size * Sample Size))
              * Estimate = Sample Variance / sqrt(Sample Size) => we want a big sample size if possible
              * Depends on Sample Variance which we known only after we collect the data
              * When the measure is a percent > 10%, Standard Error = sqrt(Percentage Obtained from Measurement * (1 - Percentage Obtained from Measurement) / Sample Size)
      * [Confidence Interval](https://en.wikipedia.org/wiki/Confidence_interval) = Sample Mean ± Confidence Interval Coefficient * Standard Error
        * Confidence Interval Coefficient for 2-sided test and confidence level 90%: 1.65, 95%: 1.96, 98%: 2.33, 99%: 2.58
      * [Central Limit Theorem](https://en.wikipedia.org/wiki/Central_limit_theorem): means of samples tend to be distributed according to a normal distribution when n > 30
      * Comparing Two Samples
        * Standard Error of the Distribution of the Difference of the Two Averages = sqrt((Variance₁ / Sample Size₁) + (Variance₂ / Sample Size₂))
      * [Student's t-test](https://en.wikipedia.org/wiki/Student%27s_t-test)
        * Degrees of Freedom = Sample Size - 1
      * [Monte Carlo Method](https://en.wikipedia.org/wiki/Monte_Carlo_method)
    * [(Big)](https://en.wikipedia.org/wiki/Big_data) [Data Science](https://en.wikipedia.org/wiki/Data_science)
      * Workflow
        * http://datascience.la/data-science-toolbox-survey-results-surprise-r-and-python-win/
        ![pafka2014](http://datascience.la/wp-content/uploads/2014/09/data-science-workflow-szilard.png)
        * [Sample, Explore, Modify, Model, Assess](https://en.wikipedia.org/wiki/SEMMA) (SEMMA)
      * Volume, Velocity, Variety
      * [Machine Learning](https://en.wikipedia.org/wiki/Machine_learning)
        * [Neural Networks](https://en.wikipedia.org/wiki/Artificial_neural_network)
      * Data Sources
        * Surveys
          * Observations are usually more accurate
          * Helps understand why, not just what
          * Often miss special cases
        * Environmental Sensors (See Environmental Sensors)
        * Traffic Counts (See Traffic Counts)
        * (Autonomous) Vehicles
        * Social Media
          * Twitter
        * Energy Data
        * Communication Data
        * Activity Data
        * Production and Consumption Data
        * Census Data
        * Safety Data
      * http://trec.pdx.edu/events/professional-development/big-data-and-future-travel-modeling
  * [Traffic](https://en.wikipedia.org/wiki/Traffic)
    * [Induced Demand](https://en.wikipedia.org/wiki/Induced_demand) (Latent Demand)
      * Road Supply -> Travel Demand -> Road Supply... (positive feedback loop is controlled by congestion)
      * http://www.accessmagazine.org/articles/spring-2003/induced-travel-studies-inducing-bad-investments/
      * http://trec.pdx.edu/events/professional-development/friday-transportation-seminar-topic-tba-0
    * [Rush Hour](https://en.wikipedia.org/wiki/Rush_hour)
    * [Braess' Paradox](https://en.wikipedia.org/wiki/Braess%27_paradox)
    * [Traffic Models](https://en.wikipedia.org/wiki/Traffic_model)
      * Requirements for Models
        * sensativity: as close to reality as necessary
        * logical consistancy: makes sense
        * operability: easy and cheap to use
        * transparency: clear and understandable
        * reliability: same result with the same external conditions
        * validity: suitable for representation and analysis
      * Model error is based on data error and specification error
        * Data error increases w/ complexity
        * Specification error decreases w/ complexity
      * Types
        * Relationship Model e.g. function w/ inputs and outputs
        * Process Model e.g. complex system w/ many relationships, interfaces (input/output), and feedback loops
        * Modelling Platform e.g. a tool
      * Objectives
        * Visualize/analyze/understand today
        * Predict the future w/ and w/o implementing changes to make a better decision today
      * Method
        * [Microsimulation](https://en.wikipedia.org/wiki/Microscopic_traffic_flow_model)
          * Purpose
            * car-following behavior
            * lane change behavior
            * merge behavior
            * driver-infrastructure interaction behavior
            * driver-vehicle interaction behavior
          * Definations
            * Net Distance = Time Gap = Back of 1st car to Front of 2nd car => Distance necessary to drive perpendicular across the direction of traffic
            * Gross Distance = Headway = Front of 1st car to Front of 2nd car => For measuring vehicles/hour
            * Braking Distance
              * Absolute = minimum distance to stop before hitting a stopped object in front of you
              * Relative = minimum distance to stop before hitting a moving object in front of you
            * Time-to-crash: seconds until a vehicle hits the vehicle in front if neither speed changes
            * Post-encroachment Time: seconds between perpindicular vehicles occupying the same point
          * Variables
            * Temporal Distance = headway = seconds
            * Spatial Distance = meters
            * Velocity = kilometers / hour = meters / seconds
          * [Mass Point Model](https://en.wikipedia.org/wiki/Mass_point_geometry)
            * with constant velocity
              * a = 0
              * v = constant
              * s = s₀ + v * t
              * Centrifugal Force = (m*v²)/R
            * with constant acceleration
              * a = constant
              * v = v₀ + a * t
              * s = ½ * a * t² + v₀*t
              * F = m * a
            * [Weight](https://en.wikipedia.org/wiki/Weight) = m*g
            * [Friction Force](https://en.wikipedia.org/wiki/Friction) = µ * Normal Force
              * Dry Concrete and Rubber: µ = 1.0
              * Lubricated Steel and Steel: µ = 0.16
          * Car-Following Model
            * [Gipps' model](https://en.wikipedia.org/wiki/Gipps%27_model) (1970s)
            * [Intelligent Driver Model](https://en.wikipedia.org/wiki/Intelligent_driver_model) (2000)
            * [Newell's car-following model](https://en.wikipedia.org/wiki/Newell%27s_car-following_model) (2002)
            * Psycho-physical car-following model
              * incorporates the driver - following distance is not fixed, but oscillates
              * drivers cannot judge the speed of a car in front of them well -> design roads like ~~~~~~~ not -------
          * Lane Changing Model
            * to change or not
          * Cellular Automation Model
            * discrete car on discrete road
            * fast to compute
          * Fundamental Equation of Traffic Flow (Greenshields, 1935)
            * Volume = Density * Velocity (momentary, not local)
              * q = k * v
              * cars/hr = cars/km * km/hr
            * [Fundamental Diagram of Traffic Flow](https://en.wikipedia.org/wiki/Fundamental_diagram_of_traffic_flow)
            ![schick2003](https://github.com/davidbailey/tum/raw/master/handbook/Research/schick2003.png)

            |   | Density (k) | Volume (q) | Velocity (v) |
            | - | ----------- | ---------- | ------------ |
            | Free Flow | Low | Low | High |
            | Partially Dense | Medium | High | Medium-High |
            | Dense | High | Low | Low |

            * Two Areas of Traffic
              * Free flow (stable)
              * Transitional (unstable)
              * Congested (stable)
            * [Three Phases of Traffic](https://en.wikipedia.org/wiki/Three-phase_traffic_theory) (Kerner 2003)
              * Free flow
              * Synchronized flow
              * Wide moving jam
            * Van Aerde Model
            * Uses
              * design capacity determination
              * probablilty of congestion / level of service prediction
          * Continuum Theory and Dynamic Modeling
            * [Kinematic Wave](https://en.wikipedia.org/wiki/Kinematic_wave)
              * q = v * k => q = f(k) = q(k(x)) => k = f(x - c * t), c = speed of the wave
              * [shock waves](https://en.wikipedia.org/wiki/Shock_wave) occur where two waves meet
                * shock wave velocity, u = (q₂ – q₁) / (k₂ – k₁)
                  * positive: downstream, no effect on congestion
                  * negative: upstream, causes congestion
        * [Macrosimulation](https://en.wikipedia.org/wiki/Macroscopic_traffic_flow_model)
          * Definations
            * Passenger Car Unit = [Passenger Car Equivalent](https://en.wikipedia.org/wiki/Passenger_car_equivalent)
              * Car = 1
              * Motorcycle = .5
              * Bus = 2-4
              * Truck = 2-4
            * Homogeneous = gradiant at point in time is constant
            * [Stationary](https://en.wikipedia.org/wiki/Stationary_state) = gradiant at point in space is constant
          * Variables
            * Traffic Volume = q = vehicles / hour
              * Max capacity per lane = 1800 vehicles per hour = 1 vehicle every 2 seconds
            * Traffic Density = k = vehicles / km
              * Max density per lane = 150 vehicles per kilometer in congestions = 7 meters per vehicle
            * Average velocity = v = km / hour
              * Local = space is constant, time is variable overcounts fast vehicles = higher than momentary
              * Momentary = time is constant, space is variable
          * Four-step Model
            * Purpose
              * [Transportation Forcasting](https://en.wikipedia.org/wiki/Transportation_forecasting)
            * Assumptions / Recommendations
              * Zones (and traffic to/from a zone) is consolidated into one point via a connector. Lot of calibration needed here.
              * Create single-use zones. e.g. all residential, all commercial, etc.
              * Use natural and political boundaries if appropriate.
              * Create smaller zones in more dense areas
              * Create a study area bigger than the planning area
              * Does not consider feedback between land use and transportation
              * Does not consider feedback between the four stages.
              * Mode choice is done after destination choice
              * Ignores internal trips and through trips (to/from outside the region)
              * Ignores trip chaining
            * Required Information
              * Links: speeds, capacity (number of lanes), congestion, permissible transport modes, public transport lines
              * Nodes: capacity, turn restrictions, mean delay time for each traffic stream, public transport stops
            * Steps
              * Trip Generation
                * Number of person/vehicle trips entering or leaving a zone.
                * Structural data (population, jobs, square feet of retail space, number of seats, etc.) * Mobility rate for that data
                * Hopefully this is symmetric. e.g. number of people who leave for work = number of people who arrive at work.
              * Trip Distribution
                * Based on a gravity function Tij = Oi * Dj * f(cij)
                  * Tij = trips from i to j
                  * Oi = trips w/ origin i
                  * Dj = trips w/ destination j
                  * cij = resistance based on distance, travel time, costs, etc.
                  * f() = deterrence function e.g. power function or exponential function
                * Not necessarily symmetric.
                * Big problem is a lack of understanding of spacial decision making. E.g. what if you visit a friend across town?
              * Mode Choice
                * Generalized cost term (utility) = (time + cost + comfort) * perception of each
                * Based on the person (income, car availability, etc.) and the mode (travel time, comfort, etc.)
                * Public transport times from timetable/reality
                * Time includes wait time, access time (walk to car or public tranportation)
                * Comfort includes stress, reliability, safety, etc.
                * Captive riders must use public transportation (no car). Captive drivers must drive (no public tranportation).
                * Methods
                  * [Kirchhoff's Law](https://en.wikipedia.org/wiki/Kirchhoff%27s_circuit_laws)
                  * [Binary Logit Model](https://en.wikipedia.org/wiki/Logistic_regression)
                  * [Nested Logit Model](https://en.wikipedia.org/wiki/Discrete_choice#nested_logit)
              * Route Assignment
                * Car: which roads to take
                * Public transportation: which lines, which transfers
                * Inputs are travel demands (O/D Matrix, mode choice), transportation network with qualities for each mode, and a methodology for route choice and assignment
                * Convert from input (people) to output (vehicles) by dividing by an occupancy rate e.g. 1.1 people/vehicle for commuting
                * Outputs are impacts: traffic, congestion, noise, air pollution, loads on nodes and links
                * Methods
                  * All or nothing
                    1. Route identification for each O/D pair
                    2. Route choice
                    3. Load routes onto the network
                    4. Evaluate the effects of congestion on 1.
                  * Capacity-restraint function
                    * t = t0 * (1 + a * (V / C) ^ b
                      * t = congested travel time
                      * t0 = free flow travel time
                      * V = traffic volume on the link
                      * C = capacity of the link
                      * a,b = parameters
                    * Iterative method. e.g. add 50%, then 30%, then 20%
                * Limitations
                  * Drivers do not assign themselves logically and change assignments over time
                  * Congestion affects destination choice, mode choice, whether to take the trip at all
            * [John Glen Wardrop](https://en.wikipedia.org/wiki/John_Glen_Wardrop)
        * [Queuing Theory](https://en.wikipedia.org/wiki/Queueing_theory)
          * e.g. intersections, toll plazas, merging at bottlenecks, loading and unloading boats, planes, buses, trains
          * Arriaval Process ([FIFO](https://en.wikipedia.org/wiki/First-come,_first-served), LIFO, Service in Random Order) -> Queuing Order -> Service Process
          * [Kendall's notation](https://en.wikipedia.org/wiki/Kendall%27s_notation)
            * A/B/m/n
              * A = arrival time distribution (often stochastic)
              * B = service time distribution (often deterministic)
              * m = number of service points
              * n = number of waiting places before entering the system
              * e.g. One Lane @ Traffic Signal = A/B/1/1; Two Lanes @ Traffic Signal = A/B/1/2; Toll Plaza w/ 3 approaching lanes and 5 gates = A/B/5/3
          * ~ 2 seconds / vehicle to leave the queue
          * [Degree of Saturation](https://en.wikipedia.org/wiki/Degree_of_saturation_(traffic)) 
            * Deterministic Degree of Saturation = r = Arrival Volume / Capacity e.g. Traffic Signal
              * r > 1 = oversaturated (realistic here)
              * at a traffic signal r = Arrival Rate / (Service Rate * α) where α = Effective Greentime / Cycle Length
            * Stochastic Degree of Saturation = ρ = Arrival Rate / Service Rate e.g. Toll Gate
              * ρ < 1 = undersaturation (realistic here)
              * mean waiting time = 1 / (Service Rate - Arrival Rate)
              * mean queue length = Arrival Rate / (Service Rate - Arrival Rate)
            * Use Stochastic for ρ < 1 and Deterministic for r > 1. Problem at 1.
              * Webster Formula - useful for Traffic Signals
              * Kimber/Hollis Model
    * [Simulation](https://en.wikipedia.org/wiki/Traffic_simulation)
      * Model -> Simulation, replace physical systems w/ mathmatical models
      * Purpose
        * Study things too expensive, too dangerous, not possible
        * Compare multiple options
      * Benefits
        * Less cost, less time, less risk
        * Detailed data about all components
        * Reproducible, modifiable
      * Be careful what you define as the system. E.g. if you only consider current drivers, induced demand doesn't exist, but we know it does... In reality, the transportation system is global (or greater)
      * Inputs
        * Network Model: Links, Nodes, Rules
        * Traffic Demand: O/D Matrix
        * Behavioral Models: Car-following Model, Lane Changing Model, Route Choice Model
        * Driver and Vehicle Parameters
      * Workflow
        * Preperation
        * Initialization
        * Calibration and Validation
        * Simulation
        * Documentation      
      * Sub-Microscopic
        * PELOPS - Program for the dEvelopment of Longitudinal micrOscopic traffic Processes in a Systemrelevant environment
          * Driver Model
          * Environment Model
          * Vehicle Model
        * Driving Simulaton
      * Microscopic
        * PTV VISSIM
          * https://www.youtube.com/watch?v=PDSpKTZrE8g
        * Paramics
          * http://www.paramics-online.com
        * http://www.traffic-simulation.de
        * https://www.youtube.com/watch?v=Suugn-p5C1M
        * Pedestrian Simulation
          * Purpose: building design, station design, emergency evacuation
          * [Social Force Model](https://en.wikipedia.org/wiki/Social_force_model)
        * Bicycle Simulation
          * Traditional Microscopic Simulation e.g. small, slow cars
          * [Cellular Automation](https://en.wikipedia.org/wiki/Cellular_automaton)
          * [Social Force Model](https://en.wikipedia.org/wiki/Social_force_model)
          * [Fuzzy Logic](https://en.wikipedia.org/wiki/Fuzzy_logic)
          * [Game Theory](https://en.wikipedia.org/wiki/Game_theory)
      * Mesoscopic
        * Aimsun
          * https://www.aimsun.com
        * DYNEMO
          * https://trid.trb.org/view.aspx?id=210825
        * [Agent-based Model](https://en.wikipedia.org/wiki/Agent-based_model)
          * [MATSim](https://en.wikipedia.org/wiki/MATSim)
            * http://matsim.org/docs/extensions/matsim4urbansim
          * [UrbanSim](https://en.wikipedia.org/wiki/UrbanSim)
            * https://www.urbansim.com
        * Dynamic Traffic Assignment
          * http://dynust.net
          * http://trec.pdx.edu/events/professional-development/friday-transportation-seminar-topic-tbd-3
        * http://opentrafficsim.org
      * Macroscopic
        * PTV VISUM
        * Emme
          * https://www.inrosoftware.com/en/products/emme/
        * METANET
        * SiMoNe
        * https://github.com/jfietkau/Streets4MPI
        * http://bit-player.org/extras/traffic/
	* TransCAD
	  * http://www.caliper.com/tcovu.htm
	* Citilabs Cube
	  * http://www.citilabs.com/software/cube/
    * [Traffic Counts](https://en.wikipedia.org/wiki/Traffic_count) and (Speed Surveys)
      * Subjects
        * Pedestrians
        * Bicycles
        * Cars
          * [Vehicle Miles Traveled](https://en.wikipedia.org/wiki/Vehicle_miles_of_travel)
      * Types
        * Local: constant space, variable time
        * Momentary: constant time, variable space
        * Time-space measurement: measurement across space and time
        * Moving observer: one measurement with variable space and time
      * Methods
        * Manual
          * https://davidbailey.github.io/counter
          * https://github.com/davidbailey/js/blob/master/trafficcounter-index.ios.js
        * Automated
          * [Loop Detector](https://en.wikipedia.org/wiki/Induction_loop)
          * [Automatic Number Plate Recognition](https://en.wikipedia.org/wiki/Automatic_number_plate_recognition)
          * [Bluetooth](https://en.wikipedia.org/wiki/Bluetooth)
          * [Radar](https://en.wikipedia.org/wiki/Radar)
          * [Lidar](https://en.wikipedia.org/wiki/Lidar)
          * Photography
          * Video
          * Audio
          * Apps / [Floating Car Data](https://en.wikipedia.org/wiki/Floating_car_data)
            * [Navigation](https://en.wikipedia.org/wiki/Turn-by-turn_navigation)
            * [Strava](https://en.wikipedia.org/wiki/Strava)
              * http://metro.strava.com
            * [Uber](https://en.wikipedia.org/wiki/Uber_(company))
              * https://movement.uber.com/cities
            * Process
              * Map Matching
              * Route Reconstruction
              * Estimate
              * Display
        * Surveys
        * Traffic Count Estimation
          * Models w/o a Traffic Model
            * Neural Networks
            * Pattern Matching
            * Regression
          * Models w/ a Traffic Model
            * PTV Optima
              * http://vision-traffic.ptvgroup.com/en-us/products/ptv-optima/
      * Duration
        * Long Term - to research temporal variances
        * Short Term - to research spacial variances
      * http://nitc.trec.pdx.edu/events/professional-development/webinar-state-wide-pedestrian-and-bicycle-miles-traveled-can-we
      * https://www.pdx.edu/ibpi/count
      * https://www.fhwa.dot.gov/policyinformation/tmguide/
      * http://bikepeddocumentation.org
      * *be aware of selection biases*
  * Routing
    * [Shortest Path](https://en.wikipedia.org/wiki/Shortest_path_problem)
      * [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)
      * [A* Search Algorithm](https://en.wikipedia.org/wiki/A*_search_algorithm)
      * [Vehicle Routing Problem](https://en.wikipedia.org/wiki/Vehicle_routing_problem)
        * [Traveling Salesman Problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem)
  * Travel Behavior Analysis
    * Why Travel?
      * Activities at Destination
      * [Recreation](https://en.wikipedia.org/wiki/Recreation)
    * 
    * Influences
      * Environment: noise, air, water, safety
      * Technology: ITS, phone, GPS, telework, teleconference
      * Space
        * Hagerstrand Diagram
	* cities have more activities within a surrounding area than suburbs
      * Performance, comfort, convenience
      * Available vehicle types: car, car share, bike, bike share, public transportation
      * Cost/price: money and time; perception matters more than actual cost
      * Home/work locations: average travel time ~ 30 minutes each way
    * Maslow's Heierarchy of Needs
      1. Physiological: breathing, sleeping (food)
      2. Saety: security of the body, family, property (work)
      3. Love/belonging: friends, family, sex, intamacy (socializing)
      4. Esteem: respect
      5. Self-actualization: morality, creativity, problem solving (recreation)
    * Scheduling
      1. Mandatory things
      2. Discretionary things
    * Travel Budgets
    * Mode Choice
      * [Discrete Choice](https://en.wikipedia.org/wiki/Discrete_choice)
        * [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression)
      * [Red Bus / Blue Bus Problem](https://en.wikipedia.org/wiki/Independence_of_irrelevant_alternatives#Criticism_of_IIA)
