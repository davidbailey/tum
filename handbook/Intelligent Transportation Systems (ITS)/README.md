## [Intelligent Transportation Systems](https://en.wikipedia.org/wiki/Intelligent_transportation_system) (ITS)
* Objective: Sustainable Transportation
  * environmental
  * economic
  * social
    * safe
    * efficient
    * comfortable
* [Control Theory](https://en.wikipedia.org/wiki/Control_theory)
    * [Open Loop](https://en.wikipedia.org/wiki/Open-loop_controller)
    * Open Loop [Feedforward](https://en.wikipedia.org/wiki/Feed_forward_(control))
    * Closed Loop w/ [Feedback](https://en.wikipedia.org/wiki/Feedback)
    ![A block diagram of a negative feedback control system.](https://upload.wikimedia.org/wikipedia/commons/2/24/Feedback_loop_with_descriptions.svg)
    * [PID Controller](https://en.wikipedia.org/wiki/PID_controller)
        * P: Present Values (Proportional Term)
        * I: Past Values (Integral Term)
        * D: Future Values (Derivative Term)
    ![A block diagram of a PID controller in a feedback loop.](https://upload.wikimedia.org/wikipedia/commons/4/43/PID_en.svg)
    * [Model Predictive Control](https://en.wikipedia.org/wiki/Model_predictive_control)
* [State Machine](https://en.wikipedia.org/wiki/Finite-state_machine)
    * Stability
    * Controlability
    * Ovservability
    * [State Space](https://en.wikipedia.org/wiki/State_space)
        * [State Space Representation](https://en.wikipedia.org/wiki/State-space_representation)
* [Signal Processing](https://en.wikipedia.org/wiki/Signal_processing)
    * [Kalman Filter](https://en.wikipedia.org/wiki/Kalman_filter)
* Telematics (Telecommunications and Informatics)
  * Acquisition
  * Transmission
  * Storage
  * Processing
* Levels
  * Framework Architecture
    * US: http://www.its.dot.gov/research_archives/arch/
    * EU: http://frame-online.eu
  * Reference Architecture
  * Implementation
* Viewpoints
  * Functional: What?
  * Technical: How?
  * Organizational: Who?
* [Traffic Control](https://en.wikipedia.org/wiki/Road_traffic_control)
  * Outputs
    * Information (voluntary)
      * Radio / Digital Radio
      * [Variable Message Signs](https://en.wikipedia.org/wiki/Variable-message_sign)
        * http://www.daktronics.com/en-us/products/its-dynamic-message-signs
      * Apps (See Apps)
    * Recommendations and Guidance (voluntary)
    * Regulation and Control (mandatory)
    * Static (e.g. Yield Sign) or Dynamic (e.g. Traffic Signal)
    * Global (e.g. Yield Sign) or Individual (e.g. GPS)
  * Components
    * Central Systems
      * Human-Machine Interface
    * Distributed Systems
    * Communication Network
      * Wired
      * Wireless
        * V2X
          * [802.11p](https://en.wikipedia.org/wiki/IEEE_802.11p)
      * TCP/IP
      * Preserve Project
        * https://www.preserve-project.eu
    * Signs and Actuators
    * Detection
      * Vehicle (See Traffic Counts)
      * Environmental Sensors
        * Weather
          * air temperature
          * humidity
          * visability (fog)
          * wind speed
          * precipitation
          * road surface temperature
          * road surface condition
        * Light
        * Noise
        * Air Pollution
          * Examples
            * https://www.arb.ca.gov/adam/index.html
            * https://airnow.gov
            * http://www.umweltbundesamt.de/en/data/current-concentrations-of-air-pollutants-in-germany
          * carbon dioxide
          * sulfur oxides
          * nitrogen oxides
          * carbon monoxide
          * volatile organic compounds
          * particulates
          * ozone
    * Software
      * Data Processing
        * Aggregation
        * Filtering
        * Plausibility Checks
      * [National Transportation Communications for Intelligent Transportation System Protocol](https://en.wikipedia.org/wiki/National_Transportation_Communications_for_Intelligent_Transportation_System_Protocol)
        * http://www.ntcip.org
  * Urban
    * [Intersections](https://en.wikipedia.org/wiki/Intersection_(road)) / [Junctions](https://en.wikipedia.org/wiki/Junction_(road))
      * Types
        * Non-Signalized
          * Priortiy Intersection
            * [Priority to the Right](https://en.wikipedia.org/wiki/Priority_to_the_right)
            * [Yield Sign](https://en.wikipedia.org/wiki/Yield_sign) / [Stop Sign](https://en.wikipedia.org/wiki/Stop_sign)
              * [Level of Service](https://en.wikipedia.org/wiki/Level_of_service) Procedure
                1. Determine ranks of different streams
                2. Determine design hour traffic volume
                3. Determine basic capacity of subordinate streams
                4. Determine maximum effective capacity
                5. Consider influence of mixed lanes
                6. Assess level of service
                * Ground Capacity = number of vehicles that can cross superordinate stream in 1 hour. Depends on rank of the stream, type and location of intersection, and volume of superordinate streams
                * Effective Capacity = number of vehicles that can cross superordinate stream in 1 hour, including effects of queuing. Depends on ground capacity and probability of queues in superordinate streams
          * [Roundabout](https://en.wikipedia.org/wiki/Roundabout)
            * http://www.wimp.com/mythbusters-test-a-four-way-stop-vs-a-roundabout/
              * 4-way Roundabout averages 460 crossings in 15 minutes (+20% vs. Stop)
              * 4-way Stop: 378 crossings in 15 minutes; 391 crossings in 15 minutes; averages 384.5 crossings
              * Traffic Cop: 289 crossings
            * https://www.youtube.com/watch?v=ONacAiKXe-8
        * Signalized
          * [Traffic Signals](https://en.wikipedia.org/wiki/Traffic_light)
            * [Signal Timing](https://en.wikipedia.org/wiki/Signal_timing)
              * Signalized Intersection Design Process
                1. Find complementary signals: analyze the intersection geometry and determine conflict points (conflicting signals).
                2. Define which signal belong to which phases and choose an appropriate sequence of phases.
                3. Determine inter-green times based conflict mode, type, geometry, and speed.
                4. Determine saturation flow based on number of lanes * adjustment factors
                5. Determine traffic volumes per stream
                6. Determine cycle time between 60 and 120 seconds
                7. Calculate necessary green times including minimum green times.
                8. Calculate available green time = cycle time - sum of intergreen times
                9. Determine capacity of the intersection = sum of all capacities = green time for each flow * saturation flow for each flow from 4.
                10. Determine degree of saturation (highest of all flows) for all movements and assign a quality.
                11. Set the signal plan.
              * (See Traffic Signal Timing Manual)
              * [Traffic Signal Control and Coordination](https://en.wikipedia.org/wiki/Traffic_light_control_and_coordination#Traffic_controller_systems)
                * Requirements for Coordination
                  * Distance between intersections < 750-1000m
                  * Coordinated cycle time across all intersections
                  * Progresssion speed = 0.85 * speed limit to speed limit => offset time
                  * Level of saturation < 0.85 for coordinated stream and < 0.9 for other streams
                  * More than one lane for through traffic
                  * Dedicated left turn lanes
                  * No non-signalized pedestrian crossings
                  * Limited parking
                  * Fixed distance between intersections (for 2-way coordination). Otherwise coordinate 1-way in AM and other way in PM
                * Procedure
                  1. Define a cyce time for coordination, highest wins
                  2. Calculate signal timing plans for intersections
                  3. Define schedule of green periods based on progression speed and offset. Add 4.5 seconds the beginning of the phase to disolve queues but not more so you don't encourage speeding.
                  4. Assess quality
                    * number of vehicles that do not have to stop / total number of vehicles >= 65% is good
              * [Pedestrian Scramble](https://en.wikipedia.org/wiki/Pedestrian_scramble)
              * Leading Pedestrian Interval
              * [Green Wave](https://en.wikipedia.org/wiki/Green_wave) (DE: Grüne Welle)
            * [Turn on Red](https://en.wikipedia.org/wiki/Turn_on_red)
        * [Grade Seperation](https://en.wikipedia.org/wiki/Grade_separation)
      * Turns
        * Types (varies across the USA, even within a city)
          * Permissive (green/red circle)
            * Shorter delay for all users
            * Typical in Germany
          * Protected (green/red arrow)
            * Longer delay for all users
            * Typical in The Netherlands
        * [Hook Turn](https://en.wikipedia.org/wiki/Hook_turn)
        * [Pittsburgh Left](https://en.wikipedia.org/wiki/Pittsburgh_left)
        * [Michigan Left](https://en.wikipedia.org/wiki/Michigan_left)
        * [Jughandle](https://en.wikipedia.org/wiki/Jughandle)
    * Adaptive Traffic Control
      * Inputs (excluding Vehicle and Environment (See Detection))
        * time of day
        * day of week
        * season of year
        * special events
        * incidents
        * traffic management
      * Coverage
        * Local
        * Line (e.g. coordinated signals)
        * Network
          * Types
            * Centralized
            * Central-Decentralized (German Philosophy)
              * Central controller sets bounds every 5-15 minutes
              * Local controllers act within those bounds.
            * Decentralized
          * Procedure
            1. Inputs
            2. Traffic Demand Model
            3. Traffic Flow Model
            4. Traffic Impact Model
            5. Control Model
            6. Signal Program
            7. Repeat from 3. until optimized
            8. Outputs
          * Examples
            * Los Angeles Automated Traffic Surveillance and Control
              * http://www.trafficinfo.lacity.org/about-atsac.php
            * SCOOT (Split Cycle Offset Optimisation Technique)
              * http://www.scoot-utc.com
              * small steps every 5 minutes
      * Levels
        * Strategic - long-term
        * Tactical - mid-term
        * Operational - short-term
      * Online Modifications
        * cycle time
        * offset
        * phase sequence
        * number of phases
        * split
      * Types
        * rule-based e.g. end a green phase early if queue on other stream builds up
          * good local for a few critical intersections
        * model-based
          * good network for network w/ complex cause-effect relationships
      * Public Transportation Prioritization (Signal Preemption)
        1. detect vehicle / request signal
        2. end current phase (or extend current phase)
        3. begin public transportation phase
        4. detect vehicle / release signal
        5. resume normal operations
  * [Freeway / Motorway](https://en.wikipedia.org/wiki/Controlled-access_highway)
    * Objectives
      * increase traffic flow
      * increase safety
      * reduce emissions
    * Classification
      * Network Control Systems e.g. rerouting for major events, traffic
        * [Variable Message Signs](https://en.wikipedia.org/wiki/Variable-message_sign)
        * [Navigation System](https://en.wikipedia.org/wiki/Automotive_navigation_system)
        * addative: recommend a new route or substantiative: change the route
        * manual or automatic control
        * Variable Lane Allocation e.g. Northbound I-110 at I-5
      * Section Control Systems
        * [Variable Message Signs](https://en.wikipedia.org/wiki/Variable-message_sign)
          * Text
            * Traffic Dependent (automatic)
              * Congestion
                * Depends on traffic flow, density, and velocity
              * Crash
              * Hard Shoulder Use
              * Truck Passing Ban
            * Environmental (automatic): Ice, Rain, Snow, Fog
            * Other: Construction
          * Image
          * Dynamnic Speed Limit
            * Purpose: allows more people ot travel closer to the free flow speed, reduces critical braking that causes brakeing shock waves
            * Pick lowest speed for the conditions
          * Procedure
            * Identify Situation
              * Data Acquisition
              * Data Validation
            * Determine Priority
              * Build Speed Funnels
            * Display Message
      * Intersection Control Systems
        * [Ramp Metering](https://en.wikipedia.org/wiki/Ramp_meter)
        * Purpose
          * Reduce congestion on freeway by temporarly reducing demand
          * Break up entering [Platoons](https://en.wikipedia.org/wiki/Platoon_(automobile))
        * Local or Coordinated
    * [Interchange](https://en.wikipedia.org/wiki/Interchange_(road))
        * https://ops.fhwa.dot.gov/publications/fhwahop12032/
* Automatic Incident Detection
  * Incident: drop in speed/safety or any deviation from the norm
    * Characteristics
      * Severity
      * Length
      * Location
  * Methods
    * Compare w/ Norm
    * [Kalman Filter](https://en.wikipedia.org/wiki/Kalman_filter)
    * Video Image Processing
    * ...
  * Examples
    * [Motorway Incident Detection and Automatic Signalling](https://en.wikipedia.org/wiki/Motorway_Incident_Detection_and_Automatic_Signalling) (MIDAS) (UK)
    * [Expressway Monitoring and Advisory System](https://en.wikipedia.org/wiki/Expressway_Monitoring_and_Advisory_System) (SG)
    * [Freeway Traffic Management System](https://en.wikipedia.org/wiki/Freeway_Traffic_Management_System) COMPASS (CA)
