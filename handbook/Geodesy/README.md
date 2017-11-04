## Geodesy

### Geoinformation: where, what, how much, how, why

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

### [Geoinformatics](https://en.wikipedia.org/wiki/Geoinformatics): art, science, engineering, techonogy of geoinformation

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
    * Integration
    * Updating
  * Spatial Data Handling
    * Visualization
    * [Analysis](https://en.wikipedia.org/wiki/Spatial_analysis)
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
  * Quality Assessment
* Cellular Models e.g. [Conway's Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life)

### [Geographic Information System](https://en.wikipedia.org/wiki/Geographic_information_system): tools + display + database

* [GIS Software](https://en.wikipedia.org/wiki/List_of_geographic_information_systems_software)

### Global Navigation Satellite System (GNSS)

* Systems
  * [Global Positioning System](https://en.wikipedia.org/wiki/Global_Positioning_System) (GPS)
    * Uplink: Colorado Springs
    * Downlink
    * 24 Satellites / 6 Orbital Planes
    * 4 Unknowns: X, Y, Z, Receiver Clock Error = 4 Satellites
    * 5-20m accuracy
    * [Differential_GPS](https://en.wikipedia.org/wiki/Differential_GPS): 1m accuracy
  * [Galielo](https://en.wikipedia.org/wiki/Galileo_(satellite_navigation))
  * [GLONASS](https://en.wikipedia.org/wiki/GLONASS)
  * [BeiDou Navigation Satellite System](https://en.wikipedia.org/wiki/BeiDou_Navigation_Satellite_System)
  * [Indian Regional Navigation Satellite System](https://en.wikipedia.org/wiki/Indian_Regional_Navigation_Satellite_System)
* [GNSS augmentation](https://en.wikipedia.org/wiki/GNSS_augmentation)
  * Satellite-based augmentation systems
    * Wide Area Augmentation System
    * European Geostationary Navigation Overlay Service
* Theory
  * Earth is an Ellipsoid: semi-major axis, semi-minor axis, flattening, eccentricity
  * Levels of Maps
    * Global
    * National
    * Transformations between levels
      * 3 Translations, 3 Roataions, 1 Scale
      * Preserve Angles: UTM or Preserve Areas

### Design

* Maps > Reports (people don't read reports)
* Clear
* High Resolution
* Title, Legend, Compass Rose, Scale
* Symbols - clear and precise
* No purposeless details
* [Design principles for cartography](https://blogs.esri.com/esri/arcgis/2011/10/28/design-principles-for-cartography/) [blogs.esri.com]

