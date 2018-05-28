## [Research Methods](https://en.wikipedia.org/wiki/Research#Research_methods)

### [Research Design](https://en.wikipedia.org/wiki/Research_design)

* Types of Studies
  * [Case-control study](https://en.wikipedia.org/wiki/Case-control_study)
  * Before/After Study
  * [Cross-sectional study](https://en.wikipedia.org/wiki/Cross-sectional_study)
  * [Meta-analysis](https://en.wikipedia.org/wiki/Meta-analysis)
  
### [Experimental design](https://en.wikipedia.org/wiki/Design_of_experiments)
* Full [factorial design](https://en.wikipedia.org/wiki/Factorial_experiment)
* [Fractional factorial design](https://en.wikipedia.org/wiki/Fractional_factorial_design)
* [Robust parameter design](https://en.wikipedia.org/wiki/Robust_parameter_design)
* [Sparsity-of-effects principle](https://en.wikipedia.org/wiki/Sparsity-of-effects_principle)
* [Indicator function](https://en.wikipedia.org/wiki/Indicator_function) e.g. 1 if male, 0 if female
* [Latent class model](https://en.wikipedia.org/wiki/Latent_class_model)
  * Latent variable: a variable we cannot directly observe: Observable variables -> Latent variable -> Observable outputs

### [Sensitivity analysis](https://en.wikipedia.org/wiki/Sensitivity_analysis)

### High [Dimensional](https://en.wikipedia.org/wiki/Dimension) Space

* [Curse of dimensionality](https://en.wikipedia.org/wiki/Curse_of_dimensionality)

### Communicating Information

* Principles
  * Figure/ground: one thing in the foreground and one thing in the background; bottom thing is always foreground
  * Proximity: we see things near each other as together
  * Similarity: things that look similar go together
  * Parallelism: parallel lines go together
  * Common Fate: things that move together go together
  * Closure: our brain completes the picture / sees what isn’t there
  * Continuity: our brain fills gaps
* Visualizations
  * Tell a story. Start with a big header, then some introduction, then a bold call to action, then the data. Maybe add a little conclusion in a text box in the data. 
  * Headline: communicates the key idea of the story
  * Story: think of the story, then the data, then the visualization
* Presentations / Lectures
  * Types
    * Monologue: the presenter speaks the entire time
    * Guided Monlogue: the presenter acts as a guide and prompts the audience to provide the material
    * Seminar: the audience guides the discussion, may not cover all the material desired to be covered by the presenter
  * Multimedia: slides, pictures, video, posters, handouts
  * Questions: are good, allow for them
  * Exercises: can be good
* [Design Principles](https://principles.design/examples/) [principles.design]
* Remove to improve
  * [the data-ink ratio](https://www.darkhorseanalytics.com/blog/data-looks-better-naked) [www.darkhorseanalytics.com]
![the data-ink ratio](https://static1.squarespace.com/static/56713bf4dc5cb41142f28d1f/t/5671eae2816924fc2265189a/1454121618204/data-ink.gif)
  * [the data tables edition](https://www.darkhorseanalytics.com/blog/clear-off-the-table) [www.darkhorseanalytics.com]
![the data tables edition](https://static1.squarespace.com/static/56713bf4dc5cb41142f28d1f/t/5671eb1e816924fc2265196e/1454121002571/ClearOffTheTableMd.gif)
  * [the map edition](https://www.darkhorseanalytics.com/blog/data-looks-better-naked-maps-edition) [www.darkhorseanalytics.com]
![the map edition](https://static1.squarespace.com/static/56713bf4dc5cb41142f28d1f/t/5810e4186a4963ac4defc76b/1481623134192/map_reduce2.gif)
* [SSAC18: Talk Data to your Organization Part 1](https://www.youtube.com/watch?v=txrOQ2p7xK8) [www.youtube.com]

### Models

* Requirements for Models
  * sensativity: as close to reality as necessary
  * logical consistancy: makes sense
  * operability: easy and cheap to use 
  * transparency: clear and understandable
  * reliability: same result with the same external conditions
  * validity: suitable for representation and analysis
* Model error is based on data error (measurement error) and specification error
  * Data error increases w/ complexity
  * Specification error decreases w/ complexity
* Types
  * Physical Models
  * Mathmatical (Relationship) Model e.g. function w/ inputs and outputs
    * Numerical and Analytical
  * Process Model e.g. complex system w/ many relationships, interfaces (input/output), and feedback loops
  * Modelling Platform e.g. a tool
* Properties
  * Static and Dynamic
  * Deterministic and Stochastic
  * Continuous and Discrete
* Objectives
  * Visualize/analyze/understand today
  * Predict the future w/ and w/o implementing changes to make a better decision today
* Calibration and Validation
  * Minimize the Mean Square Error - always a good thing to try
  * Number of runs determined by mean square error deviation and confidence interval


### [(Big)](https://en.wikipedia.org/wiki/Big_data) [Data Science](https://en.wikipedia.org/wiki/Data_science)

* Workflow
  * http://datascience.la/data-science-toolbox-survey-results-surprise-r-and-python-win/
  ![pafka2014](http://datascience.la/wp-content/uploads/2014/09/data-science-workflow-szilard.png)
  * [Sample, Explore, Modify, Model, Assess](https://en.wikipedia.org/wiki/SEMMA) (SEMMA)
  * [Cross-industry standard process for data mining](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining)
* Volume, Velocity, Variety
* [Databases](https://en.wikipedia.org/wiki/Database)
  * [Data Warehouse](https://en.wikipedia.org/wiki/Data_warehouse) vs. [Data Lake](https://en.wikipedia.org/wiki/Data_lake) vs. Data Swamp
  * [Extract, transform, load (ETL)](https://en.wikipedia.org/wiki/Extract,_transform,_load)
  * [Data cleaning](https://en.wikipedia.org/wiki/Data_cleansing)
  * [ACID (Atomicity, Consistency, Isolation, Durability)](https://en.wikipedia.org/wiki/ACID)
  * [CAP theorem](https://en.wikipedia.org/wiki/CAP_theorem): Consistency,	Availability,	Partition tolerance - Pick 2 of 3
* Data Sources
  * Driving Simulators
  * Field studies: expensive and difficult
  * Surveys: cheap, detailed, easy, flexible, biased
    * [Survey Design](https://en.wikiversity.org/wiki/Survey_design) [en.wikiversity.org]
    * [Travel Survey Manual](http://www.travelsurveymanual.org) [www.travelsurveymanual.org]
    * [Panel data](https://en.wikipedia.org/wiki/Panel_data) repeated data from the same source
    * Self-administered (questionnaire, inventories, travel diaries)
      * Online / App
      * Mail
    * Interview
      * In-person / focus groups
      * Telephone
    * Observations are usually more accurate
    * Helps understand why, not just what
    * Often miss special cases
    * Reasonableness check: ask for individual satisfaction and overall satisfaction. they should match.
    Order of questions matters.
    * Provide Other, N/A, etc.
  * Environmental Sensors (See Environmental Sensors)
  * Traffic Counts (See Traffic Counts)
  * (Autonomous) Vehicles
  * Crash Reports
  * Social Media
    * Twitter
  * Energy Data
  * Communication Data
  * Activity Data
  * Production and Consumption Data
  * Census Data
  * Safety Data
* http://trec.pdx.edu/events/professional-development/big-data-and-future-travel-modeling

### [Randomness](https://en.wikipedia.org/wiki/Randomness)

* [Random number generator](https://en.wikipedia.org/wiki/Random_number_generation)
  * [Pseudorandom number generator](https://en.wikipedia.org/wiki/Pseudorandom_number_generator)
    * [Halton sequence](https://en.wikipedia.org/wiki/Halton_sequence)
    
    
