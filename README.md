# COVID-19 Modeling using Particle Swarm Optimization (PSO)

## Overview
This project implements a Particle Swarm Optimization (PSO) algorithm to optimize the parameters of the SIR (Susceptible-Infected-Recovered) epidemiological model for COVID-19 prediction across multiple countries.

## Features
- **PSO Algorithm**: Custom implementation of Particle Swarm Optimization for parameter tuning
- **SIR Model**: Epidemiological modeling using differential equations
- **Multi-Country Analysis**: Comparative analysis across India, US, Brazil, Russia, and Nigeria
- **Visualization**: Comprehensive plotting of actual vs predicted cases
- **Performance Comparison**: MSE comparison between PSO-optimized and traditional fixed parameters

## Mathematical Background

### SIR Model Equations
```
dS/dt = -β * S * I / N
dI/dt = β * S * I / N - γ * I
dR/dt = γ * I
```

Where:
- **S**: Susceptible population
- **I**: Infected population  
- **R**: Recovered population
- **β**: Transmission rate (infection rate)
- **γ**: Recovery rate
- **N**: Total population

### PSO Algorithm
The PSO algorithm optimizes the parameters (β, γ) by:
1. Initializing particles with random positions in the parameter space
2. Evaluating fitness using Mean Squared Error (MSE) between predicted and actual cases
3. Updating particle velocities and positions based on personal and global best positions
4. Iteratively improving parameter estimates

## Results
The project demonstrates that PSO-optimized parameters significantly outperform traditional fixed parameters in predicting COVID-19 case trajectories across all analyzed countries.

## Technologies Used
- **Python 3.x**
- **NumPy**: Numerical computations
- **Pandas**: Data manipulation
- **Matplotlib**: Data visualization
- **SciPy**: Differential equation solving

## Installation
```bash
pip install numpy pandas matplotlib scipy
```

## Usage
1. Ensure you have the COVID-19 dataset (`covid_19_clean_complete.csv`) in the project directory
2. Run the Jupyter notebook: `jupyter notebook PSO_assignment.ipynb`
3. Execute all cells to see the analysis and visualizations

## Project Structure
```
├── PSO_assignment.ipynb    # Main analysis notebook
├── README.md              # Project documentation
├── requirements.txt       # Python dependencies
└── .gitignore            # Git ignore file
```

## Key Findings
- PSO successfully optimizes SIR model parameters for each country
- Optimized parameters vary significantly between countries, reflecting different transmission dynamics
- PSO-optimized predictions show much lower MSE compared to traditional fixed parameters
- The model captures the general trend of COVID-19 spread across different regions

## Future Enhancements
- Add more sophisticated epidemiological models (SEIR, SEIRD)
- Implement additional optimization algorithms for comparison
- Include vaccination data in the model
- Add confidence intervals for predictions
- Extend analysis to more countries and time periods

## License
This project is open source and available under the MIT License. 