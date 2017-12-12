## [Intelligent Transportation Systems](https://en.wikipedia.org/wiki/Intelligent_transportation_system) (ITS)

### Objective

* Save lives, time, money, energy, the environment
* Promote all modes
* [Sustainable Transportation Systems](https://github.com/davidbailey/tum/blob/master/handbook/Sustainable%20Transportation%20Systems/) [self]

### [Control Theory](https://en.wikipedia.org/wiki/Control_theory)

* [Open Loop](https://en.wikipedia.org/wiki/Open-loop_controller)
* [Feed Forward](https://en.wikipedia.org/wiki/Feed_forward_(control))
* Closed Loop w/ [Feedback](https://en.wikipedia.org/wiki/Feedback)

![A block diagram of a negative feedback control system.](https://upload.wikimedia.org/wikipedia/commons/2/24/Feedback_loop_with_descriptions.svg)

* [PID Controller](https://en.wikipedia.org/wiki/PID_controller)
  * P: Present Values (Proportional Term)
  * I: Past Values (Integral Term)
  * D: Future Values (Derivative Term)

![A block diagram of a PID controller in a feedback loop.](https://upload.wikimedia.org/wikipedia/commons/4/43/PID_en.svg)

* [Model Predictive Control](https://en.wikipedia.org/wiki/Model_predictive_control)

### [State Machine](https://en.wikipedia.org/wiki/Finite-state_machine)

* Stability
* Controlability
* Ovservability
* [State Space](https://en.wikipedia.org/wiki/State_space)
  * [State Space Representation](https://en.wikipedia.org/wiki/State-space_representation)

### [Signal Processing](https://en.wikipedia.org/wiki/Signal_processing)

* [Kalman Filter](https://en.wikipedia.org/wiki/Kalman_filter)

### Telematics (Telecommunications and Informatics)

* Acquisition
* Transmission
* Storage
* Processing

### Networking

* Destination
  * Unicast
  * Multicast
  * Broadcast
* Latency
* Bandwidth
* OSI Model
  * Physical
  * Data Link
  * Network
  * Transport
  * Session
  * Presentation
  * Application

### Levels

* Framework Architecture
  * US: http://www.its.dot.gov/research_archives/arch/
  * EU: http://frame-online.eu
  * 2010 directive 2010/40/EU of European Parliament on ITS: Framework for the deployment of Intelligent Transport Systems in the field of road transportation and for interfaces with other modes of transport
* Reference Architecture
* Implementation

### Viewpoints

* Functional: What?
* Technical: How?
* Organizational: Who?

### Autonomous Driving

* History
  * [Navlab](https://en.wikipedia.org/wiki/Navlab)
  * [Eureka Prometheus Project](https://en.wikipedia.org/wiki/Eureka_Prometheus_Project)
* SAE Levels of Automation:
  * Human monitors the driving environment
    * No Automation
    * Driver Assistance
      * Self Parking
    * Partial Automation
  * Car monitors the driving environment
    * Conditional Automation: need a process to bring the driver back into the loop
    * High Automation
    * Full Automation
* Driving Tasks
  * Localization and Mapping - Where am I?
    * [Six Degrees of Freedom](https://en.wikipedia.org/wiki/Six_degrees_of_freedom)

    ![Six Degrees of Freedom](https://upload.wikimedia.org/wikipedia/commons/f/fa/6DOF_en.jpg)

    * [Simultaneous localization and mapping](https://en.wikipedia.org/wiki/Simultaneous_localization_and_mapping)
      * [GraphSLAM](https://en.wikipedia.org/wiki/GraphSLAM)
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
    * [Pose](https://en.wikipedia.org/wiki/Pose_(computer_vision))
      * [3D Pose Estimation](https://en.wikipedia.org/wiki/3D_pose_estimation)

* Inputs (Sensors)
  * Internal
    * Car Area Network (CAN)
      * Wheel Speed
      * Yaw Rate
      * Steering Angle
      * Acceleration/Brake Pedal
      * Accelerometer
      * Roll Angle
      * Pitch Angle
      * Rain/Temperature Sensor
    * Cabin
      * Cameras
      * Internal Audio
    * [Inertial Measurement Unit](https://en.wikipedia.org/wiki/Inertial_measurement_unit)
  * External
    * Ultrasonic
    * Radar
    * LIDAR
    * Optical Camera (Stereo)
    * Infrared Camera
    * Satellite Navigation
    * Audio e.g. wet road
  * [Microelectromechanical systems](https://en.wikipedia.org/wiki/Microelectromechanical_systems)
* Outputs
  * Steering Angle (Steer By Wire)
  * Brakes
    * Pressure
    * Modulation
  * Engine (Drive By Wire)
  * Driver Feedback
    * Visual
    * Haptic
    * Acoustic
* Functions (Computers)
  * Fusion of Sensor Data
  * Object Detection
  * Object Identification (Classification)
  * Route Planning
  * Lateral Control
    * Lane Selection (for route, safety, and speed)
  * Longitudinal Control
* Challenges
  * Snow / Rain
  * Open Spaces
  * Indoors (Parking Structure)
  * Pedestrian/Bicycle Behavior
    * Communication with Pedestrians/Cyclists
  * Reflections
  * Merging
  * initial decrease in road capacity followed by possible increase in capacity if high adoption rate

### [Advanced Driver Assistance Systems (ADAS)](https://en.wikipedia.org/wiki/Advanced_driver-assistance_systems)

* Anti-lock Braking System (ABS)
* [Electronic Stability Control](https://en.wikipedia.org/wiki/Electronic_stability_control)
  * Traction Control System (TCS)
* [Adaptive Cruise Control](https://en.wikipedia.org/wiki/Autonomous_cruise_control_system)
* [Navigation](https://en.wikipedia.org/wiki/Automotive_navigation_system) = Positioning x Guidance
  * Positioning
    * Dead Reckoning = Velocity * Time + Last Known Location
      * Can have high error propagation
    * [Global Navigation Satellite System (GNSS)]() [self]

### Vehicle Efficency/Convinence Improvements

* Regenerative Braking
* Automatic Engine Stop / Start
* Cooperative Traffic Signal Communication with Vehicles (Speed for Green)
    * Dynamic Speed Limit on Motorways

### Cooperative Intelligent Transport Systems (C-ITS)

* [Cooperative ITS Corridor](http://www.c-its-korridor.de/?menuId=1&sp=en) [www.c-its-korridor.de]
* [Vehicular_communication_systems](https://en.wikipedia.org/wiki/Vehicular_communication_systems)
  * [simTD](http://www.simtd.de/index.dhtml/enEN/index.html) [www.simtd.de]
  * [Vehicle to Everything (V2X)](https://en.wikipedia.org/wiki/Vehicle-to-everything)
  * [Vehicle to Vehicle (V2V)](https://en.wikipedia.org/wiki/Vehicle-to-vehicle)
  * [Vehicle to Grid (V2G)](https://en.wikipedia.org/wiki/Vehicle-to-grid)
  * [Vehicle to Device (V2D)](https://en.wikipedia.org/wiki/Vehicle-to-device)
  * Vehicle to Pedestrian (V2P)
  * Vehicle to Infrastructure (V2I)

### Vehicle Safety

* Active: avoid crashes
  * Blind Spot Warning
  * Lane Keeping
  * Emergency Braking
  * Emergency Lane Change
  * Car Preconditioning
  * Pedestrian Warning
  * Cyclist Warning
  * Collision Warning / Prevention
* Passive: reduce effects of crashes
  * During Crash
    * Seat Belts (Lap Belt -> 3-point Belt)
      * Belt Tensioners
    * Head Restraint
    * Crumple Zones
      * High [g-forces](https://en.wikipedia.org/wiki/G-force) in a short time period are very bad.
      * Smaller vehicles need stiffer crumple zones because they have less mass so they need to absorb more impact.
    * Child Restraint Systems
    * [Crash Tests](https://en.wikipedia.org/wiki/Crash_test)
      * Standards
        * https://en.wikipedia.org/wiki/Federal_Motor_Vehicle_Safety_Standards
        * http://www.unece.org/trans/main/welcwp29.html
        * https://en.wikipedia.org/wiki/Euro_NCAP
        * https://en.wikipedia.org/wiki/Insurance_Institute_for_Highway_Safety
      * Types: Single Wall vs. Car to Car
        * Front Impact
        * Side Impact
          * Pole
          * Moveable Barrier
        * Rear Impact: Fuel and Whiplash are often biggest problems.
      * Crash Test Dummies
        * 50% Male
        * THOR
        * THUMS
  * Airbags (Front, Side, Head)
* After Crash
  * Automatic Emergency Call
  * V2V/I Collision Notifications
* "Night Vision" Systems

### [Traffic Control](https://en.wikipedia.org/wiki/Road_traffic_control)

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
              * Determine ranks of different streams
              * Determine design hour traffic volume
              * Determine basic capacity of subordinate streams
              * Determine maximum effective capacity
              * Consider influence of mixed lanes
              * Assess level of service
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
            * [Traffic Signal Timing Manual](https://ops.fhwa.dot.gov/publications/fhwahop08024/) [ops.fhwa.dot.gov]
            * Signalized Intersection Design Process
              * Find complementary signals: analyze the intersection geometry and determine conflict points (conflicting signals).
              * Define which signal belong to which phases and choose an appropriate sequence of phases.
              * Determine inter-green times based conflict mode, type, geometry, and speed.
              * Determine saturation flow based on number of lanes * adjustment factors
              * Determine traffic volumes per stream
              * Determine cycle time between 60 and 120 seconds
              * Calculate necessary green times including minimum green times.
              * Calculate available green time = cycle time - sum of intergreen times
              * Determine capacity of the intersection = sum of all capacities = green time for each flow * saturation flow for each flow from 4.
              * Determine degree of saturation (highest of all flows) for all movements and assign a quality.
              * Set the signal plan.
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
                * Define a cyce time for coordination, highest wins
                * Calculate signal timing plans for intersections
                * Define schedule of green periods based on progression speed and offset. Add 4.5 seconds the beginning of the phase to disolve queues but not more so you don't encourage speeding.
                * Assess quality
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
        * EPICS
      * Line (e.g. coordinated signals)
      * Network
        * Types
          * Centralized
          * Central-Decentralized (German Philosophy)
            * Central controller sets bounds every 5-15 minutes
            * Local controllers act within those bounds.
          * Decentralized
        * Procedure
          * Inputs
          * Traffic Demand Model
          * Traffic Flow Model
          * Traffic Impact Model
          * Control Model
          * Signal Program
          * Repeat from 3. until optimized
          * Outputs
        * Examples
          * Los Angeles Automated Traffic Surveillance and Control
            * http://www.trafficinfo.lacity.org/about-atsac.php
          * SCOOT (Split Cycle Offset Optimisation Technique)
            * http://www.scoot-utc.com
            * small steps every 5 minutes
          * MOTION
          * TRANSYT
          * BALANCE
          * Sydney Coordinated Adaptive Traffic System (SCATS)
          * UTOPIA
          * Optimized Policies for Adaptive Control (OPAC)
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
    * detect vehicle / request signal
    * end current phase (or extend current phase)
    * begin public transportation phase
    * detect vehicle / release signal
    * resume normal operations
* [Freeway / Motorway](https://en.wikipedia.org/wiki/Controlled-access_highway)
  * Objectives: increase traffic flow, increase safety, reduce emissions, reduce time lost
  * Classification
    * Network Control Systems e.g. rerouting for major events, traffic
      * [Variable Message Signs](https://en.wikipedia.org/wiki/Variable-message_sign)
      * [Navigation System](https://en.wikipedia.org/wiki/Automotive_navigation_system)
      * addative: recommend a new route or substantiative: change the route
      * manual or automatic control
      * Variable Lane Allocation e.g. Northbound CA-110 at I-5
    * Section Control Systems
      * [ATDM Program Brief: An Introduction to Active Transportation and Demand Management](https://ops.fhwa.dot.gov/publications/fhwahop12032/) [ops.fhwa.dot.gov]
      * Model-based Control INCA
        * Minimize the Objective Function = probability of a crash × cost of a crash + value of time / speed
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
  * [Interchange](https://en.wikipedia.org/wiki/Interchange_(road)) Control Systems
    * [Ramp Metering](https://en.wikipedia.org/wiki/Ramp_meter)
      * Purpose
        * Reduce congestion on freeway by temporarly reducing demand
        * Break up entering [Platoons](https://en.wikipedia.org/wiki/Platoon_(automobile))
      * ALINEA

### Automatic Incident Detection

* Incident: drop in speed/safety or any deviation from the norm
  * Characteristics
    * Severity
    * Length
    * Location
* Methods
  * Compare w/ Norm
  * [Kalman Filter](https://en.wikipedia.org/wiki/Kalman_filter)
  * Video Image Processing
  * California Algorithm
  * VkDIFF
  * ...
* Metrics
  * Detection Rate = Number of Detected Cases / Total Number of Cases
  * False Alarm Rate = Number of False Alarms / Total Number of Alarms
  * Alarm Reliability Rate = (Number of Alarms - Number of False Alarms) / Number of Alarms
  * Mean Time To Detect = Time of Detection - Time of Incident
* Examples
  * [Motorway Incident Detection and Automatic Signalling](https://en.wikipedia.org/wiki/Motorway_Incident_Detection_and_Automatic_Signalling) (MIDAS) (UK)
  * [Expressway Monitoring and Advisory System](https://en.wikipedia.org/wiki/Expressway_Monitoring_and_Advisory_System) (SG)
  * [Freeway Traffic Management System](https://en.wikipedia.org/wiki/Freeway_Traffic_Management_System) COMPASS (CA)
  * [Incident Detection Alogrithm Evaluation](http://www.mountain-plains.org/pubs/pdf/MPC01-122.pdf) [www.mountain-plains.org]


