### [Traffic](https://en.wikipedia.org/wiki/Traffic)
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
    * Physical Models
    * Mathmatical (Relationship) Model e.g. function w/ inputs and outputs
      * Numerical and Analytical
    * Process Model e.g. complex system w/ many relationships, interfaces (input/output), and feedback loops
    * Modelling Platform e.g. a tool
    * Static and Dynamic
    * Deterministic and Stochastic
    * Continuous and Discrete
  * Objectives
    * Visualize/analyze/understand today
    * Predict the future w/ and w/o implementing changes to make a better decision today
  * Method
    * [Microscopic Traffic Flow Models](https://en.wikipedia.org/wiki/Microscopic_traffic_flow_model)
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
          * s = s₀ + v × t
          * Centrifugal Force = (m × v²)/R
        * with constant acceleration
          * a = constant
          * v = v₀ + a × t
          * s = ½ × a × t² + v₀ × t
          * F = m × a
        * [Weight](https://en.wikipedia.org/wiki/Weight) = m × g
        * [Friction Force](https://en.wikipedia.org/wiki/Friction) = µ × Normal Force
          * Dry Concrete and Rubber: µ = 1.0
          * Lubricated Steel and Steel: µ = 0.16
      * Car-Following Model
        * [Gipps' model](https://en.wikipedia.org/wiki/Gipps%27_model) (1970s)
        * [Intelligent Driver Model](https://en.wikipedia.org/wiki/Intelligent_driver_model) (2000)
        * [Newell's car-following model](https://en.wikipedia.org/wiki/Newell%27s_car-following_model) (2002)
        * Psycho-physical car-following model
          * incorporates the driver - following distance is not fixed, but oscillates
          * drivers cannot judge the speed of a car in front of them well -> design roads like ~~~~~~~ not -------
        * https://www.desmos.com/calculator/aqfmizrvdo
        * Cellular Automation Model
          * discrete car on discrete road
          * fast to compute
      * Lane Changing Model
        * to change or not
        * Mandatory versus Discretionary
      * Fundamental Equation of Traffic Flow (Greenshields, 1935)
        * Volume = Density × Velocity (momentary, not local)
          * q = k × v
          * cars/hr = cars/km × km/hr
        * [Fundamental Diagram of Traffic Flow](https://en.wikipedia.org/wiki/Fundamental_diagram_of_traffic_flow)
        ![schick2003](https://github.com/davidbailey/tum/raw/master/handbook/Traffic/schick2003.png)

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
          * q = v × k => q = f(k) = q(k(x)) => k = f(x - c × t), c = speed of the wave
          * [shock waves](https://en.wikipedia.org/wiki/Shock_wave) occur where two waves meet
            * shock wave velocity, u = (q₂ – q₁) / (k₂ – k₁)
              * positive: downstream, no effect on congestion
              * negative: upstream, causes congestion
    * [Macroscopic Traffic Flow Models](https://en.wikipedia.org/wiki/Macroscopic_traffic_flow_model)
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
            * Based on a gravity function Tij = Oi × Dj × f(cij)
              * Tij = trips from i to j
              * Oi = trips w/ origin i
              * Dj = trips w/ destination j
              * cij = resistance based on distance, travel time, costs, etc.
              * f() = deterrence function e.g. power function or exponential function
            * Not necessarily symmetric.
            * Big problem is a lack of understanding of spacial decision making. E.g. what if you visit a friend across town?
          * Mode Choice
            * Generalized cost term (utility) = (time + cost + comfort) × perception of each
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
                * t = t0 × (1 + a × (V / C) ^ b
                  * t = congested travel time
                  * t0 = free flow travel time
                  * V = traffic volume on the link
                  * C = capacity of the link
                  * a,b = parameters
                * Iterative method. e.g. add 50%, then 30%, then 20%
		* User Equilibrium / System Optimum Method
		  * Minimize Sum of Travel Time
		  * Deterministic or Stochastic (Percieved Best Route)
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
    * DYNAanimation
      * https://www.tesis-dynaware.com/en/products/dynaanimation-3/overview-benefits.html
  * Microscopic
    * MITSIMLab
      * https://its.mit.edu/software/mitsimlab
    * DynaMIT
      * https://its.mit.edu/software/dynamit
    * DRACULA
      * www.its.leeds.ac.uk/software/dracula/
    * Dynameq
      * www.inrosoftware.com/en/products/dynameq/
    * PTV VISSIM
      * https://www.youtube.com/watch?v=PDSpKTZrE8g
      * VisVAP
        * .vap file (VisVAP) + .pua file (Vissig)
    * Paramics
      * http://www.paramics-online.com
    * SUMO
      * http://sumo.dlr.de/wiki/
      * http://www.dlr.de/ts/en/desktopdefault.aspx/tabid-9883/16931_read-41000/
      * Network File .net
        * netedit
        * http://sumo.dlr.de/wiki/NETCONVERT Convert OSM, VISUM, VISSIM, etc.
        * http://sumo.dlr.de/wiki/NETGENERATE Generic Network
      * Traffic Demand .rou
        * DUAROUTER
        * JTRROUTER
        * OD2TRIPS
        * DFROUTER
      * Configuration File .sumocfg
    * http://www.traffic-simulation.de
    * https://www.youtube.com/watch?v=Suugn-p5C1M
    * Pedestrian Simulation
      * Purpose: capacity analysis, building design, station design, emergency evacuation
      * Grid-based Methods (Cellular Automata) e.g F.A.S.T. - Floor field- and Agent-based Simulation
      * Discrete Choice Models e.g. Speed and Direction
      * [Social Force Model](https://en.wikipedia.org/wiki/Social_force_model)
    * Bicycle Simulation
      * Traditional Microscopic Simulation e.g. small, slow cars
      * Continuous lateral movement model: maximize minimum Time to Collision, diamond shape
      * [Cellular Automation](https://en.wikipedia.org/wiki/Cellular_automaton)
      * [Social Force Model](https://en.wikipedia.org/wiki/Social_force_model)
      * [Fuzzy Logic](https://en.wikipedia.org/wiki/Fuzzy_logic)
      * [Game Theory](https://en.wikipedia.org/wiki/Game_theory)
    * Public Transportation Simulation
      * Examples: Stop Locations, Signalization, ROW C -> ROW B, Interaction w/ Others, Bus Bunching, Travel Times
      * Dwell Times
        1. Pedestrian Simulation
	2. Dwell Time = Clearance Time + Alighting Time + Boarding Time
	  * Alighting/Boarding Times = Number Alighting/Boarding * Average Alighting/Boarding Time
	  * Clearance Time = Stop, Open Doors, Go
	3. Distribution e.g. Normal Distribution
      * Outputs: travel time, delay time, speeds, speed differential, flows, densities, capacities, number of stops, queue length, fuel consumption, emissions (PHEM), ...
      * Safety Outputs: Minimum Time to Collision, Minimum Post-Encroachment Time, Initial Deceleration Rate, Maximum Speed, Maximum Relative Speed Difference
        * Surrogate Safety Assessment Model
	  * https://www.fhwa.dot.gov/publications/research/safety/08049/
      * Calibration and Validation
        * Traffic Analysis Toolbox Volume III: Guidelines for Applying Traffic Microsimulation Modeling Software
          * https://ops.fhwa.dot.gov/trafficanalysistools/tat_vol3/vol3_guidelines.pdf
  * Mesoscopic
    * Aimsun
      * https://www.aimsun.com
    * DYNEMO
      * https://trid.trb.org/view.aspx?id=210825
    * [Agent-based Model](https://en.wikipedia.org/wiki/Agent-based_model)
      * [MATSim](https://en.wikipedia.org/wiki/MATSim)
        * http://matsim.org/docs/extensions/matsim4urbansim
	* plans -> scoring -> global optimization
	* roads as queues
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
