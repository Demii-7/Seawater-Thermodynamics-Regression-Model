# Seawater-Thermodynamics-Regression-Model
A C++ tool for modeling the relationship between salinity and freezing points using Least Squares Estimation for civil/maritime safety.

Engineering Objective: Designed and implemented a predictive software tool to model the relationship between seawater salinity and freezing temperatures using C++. This tool translates raw environmental sensor data into a functional mathematical model for use in cold-region civil engineering and maritime safety assessments.

## Tools & Technologies
Language: C++

Concepts: Least Squares Estimation, Numerical Modeling, Linear Regression, Algorithm Design.

Systems: File Stream Management (I/O), Data Structures, Flow Control.


## Key Implementation Features
1. Numerical Modeling Engine

    Instead of relying on external libraries, I programmed the mathematical logic to calculate model parameters m (slope) and b (intercept) using the Least Squares Method. 
    This allows for the conversion of raw experimental data into a linear interpolation function:
                                                                                       Tf =m(S)+ b
2. Robust File I/O System
  
    Developed a module to parse external data files containing salinity and temperature measurements. The system features:
    
    Dynamic file reading to handle datasets of varying lengths.
    
    Error checking to prevent program crashes during data ingestion.

3. Interactive Predictive UI

    Engineered a menu-driven Command Line Interface (CLI) that manages program state. Users can:
    
    Generate a new model from a raw data file.
    
    Input specific salinity levels to receive real-time freezing point predictions.
    
    Toggle between modes without restarting the application.


## Analysis & Validation
To ensure the reliability of the software for engineering applications, the following validation steps were taken:

Statistical Validation: Verified regression accuracy by comparing output parameters against known manual calculation sets (e.g., verifying that a salinity of 35 ppt correlates to a predicted freezing point of ~28.6°F).

Performance Testing: Conducted verification using four distinct test cases to ensure the algorithm remained accurate across varying datasets.

Error Handling: Implemented logic to handle "out-of-bounds" menu selections and invalid data types, ensuring software stability during runtime.
