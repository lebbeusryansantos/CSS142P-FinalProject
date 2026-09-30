# Priority-Tier Queueing in an LLM API Inference Service

**Team:** Group 6 (Pelayo, Sanchez, Santos, Tazarte)  
**Course:** CSS142P - Modelling and Simulation Theory  

## Project Overview
This project simulates a Priority-Tier Queueing system for a Large Language Model (LLM) API Inference Service. Using the SimPy framework, the model evaluates system performance and resource allocation under normal peak traffic and a +20% traffic stress test. The simulation tracks key performance metrics, including average wait times and Service Level Agreement (SLA) breach rates across varying priority tiers.

## Repository Contents
* `CSS142P_FinalProject.ipynb`: The primary executable Google Colab Notebook containing the simulation logic, configurations, and scenario definitions.
* `README.txt`: Documentation and instructions for environment setup and result reproduction.
* `Simulation_Results.csv`: The formatted output data table containing wait times and SLA breach rates (generated automatically during execution).

## Instructions for Reproducing Results

**1. Open the Google Colab Notebook**  
Upload and open the provided executable model file (`CSS142P_FinalProject.ipynb`) in Google Colab.

**2. Dependencies & Environment Setup**  
The simulation relies on standard Python data science and simulation libraries. Run the initial setup cell in the notebook, which will automatically install the SimPy framework (`!pip install -q simpy`) and import the required dependencies (`numpy`, `pandas`, and `random`).

**3. Sequential Execution**  
Run all code cells sequentially from top to bottom to initialize the simulation logic, environment parameters, and scenario definitions in the runtime.

**4. Replications and Control Variables**  
The simulation is pre-configured to execute 30 independent replications per scenario. Fixed random seeds (starting at base seed 42) are explicitly implemented across all comparative runs. This ensures variance reduction and guarantees that every scenario processes identical traffic patterns for an accurate baseline comparison.

**5. Output and CSV Data Generation**  
Run the final execution cells to calculate and output the simulation results for normal peak traffic, followed by the results for the +20% traffic stress test. Executing the final cell will automatically compile the metrics into a formatted table and trigger a local browser download for `Simulation_Results.csv`.
