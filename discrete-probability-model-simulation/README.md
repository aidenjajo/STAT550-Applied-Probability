# Discrete Probability Model Simulation
*Lab 5 from STAT550 - Applied Probability*

## Overview
This lab explores simulation techniques for discrete probability distributions, focusing on geometric and negative binomial distributions. Students implement and compare two different algorithms for generating random variates, analyze computational efficiency, and validate simulations against theoretical values. The lab demonstrates both mathematical relationships between distributions and practical computational trade-offs in simulation design.

## Topics Covered

### Geometric Distribution Simulation
- While loops for generating geometric random variables
- Bernoulli trials until first success
- Roulette wheel probability modeling
- Winning streak analysis
- Empirical vs. theoretical distribution comparison

### Negative Binomial Distribution
- Mathematical relationship: NB(r,p) as sum of r Geometric(p) variables
- Two simulation algorithms:
  - **Algorithm A**: Direct sum of geometric random variables
  - **Algorithm B**: Inverse CDF method with recursion relation
- Computational complexity analysis
- Algorithm efficiency comparison

### Recursion Relations
- PMF recursion for negative binomial: $P(X = i+1) = \frac{(i+r)(1-p)}{(i+1)} \cdot P(X=i)$
- Inverse cumulative distribution function (CDF) method
- Efficient random variate generation
- Trading mathematical complexity for computational speed

### Computational Efficiency
- Timing R code with `proc.time()`
- Comparing algorithm run times
- Understanding "simulation flops" (uniform random number calls)
- Speed vs. simplicity trade-offs

### Statistical Validation
- Histogram visualization for discrete distributions
- Mean and variance estimation from simulations
- Comparing empirical statistics to theoretical values
- Large-scale simulation experiments (1000+ trials)

## Technologies Used
- R
- R Markdown

## Files
- `discrete_probability_model_simulation.Rmd` - R Markdown source code with lab exercises
- `discrete_probability_model_simulation.pdf` - Knitted PDF output showing results
- `README.md` - Project documentation

## Key Concepts
- Geometric distribution: trials until first success
- Negative binomial distribution: trials until r successes
- While loops for conditional iteration
- Inverse CDF method for random variate generation
- Recursion relations in probability distributions
- Algorithm complexity and efficiency
- Random number generation overhead
- Empirical validation of theoretical distributions

## Skills Demonstrated
- While loop implementation for stochastic processes
- Multiple algorithm development for same problem
- Computational timing and performance analysis
- Code optimization techniques
- Statistical validation of simulations
- Side-by-side comparison visualizations with `par(mfrow)`
- Understanding trade-offs in algorithm design
- Translating mathematical formulas to code

## Lab Exercises

### Task 1: Roulette Wheel Simulation
Simulates winning streaks when betting on red in roulette (18 red, 18 black, 2 green slots). Models the geometric distribution with p=20/38 (probability of losing). Results from 1000 simulations:
- Empirical mean: 1.901 spins (theoretical: 1.9)
- Empirical SD: 1.29 (theoretical: 1.31)
- Longest streak: 10 consecutive red spins

Demonstrates how empirical results converge to theoretical values with sufficient trials.

### Task 2: Negative Binomial Algorithm Comparison
Implements two algorithms for generating NB(10, 0.6) random variates:

**Algorithm A (Sum of Geometrics)**
- Generates 10 geometric random variables and sums them
- Conceptually simple, directly follows mathematical definition
- More uniform random numbers required per variate
- Slower: ~0.015 seconds for 1000 variates

**Algorithm B (Recursion/Inverse CDF)**
- Uses PMF recursion relation for direct generation
- Mathematically sophisticated, computationally efficient
- Exactly one uniform random number per variate
- Faster: ~0.007 seconds for 1000 variates (~2x speedup)

Both algorithms produce statistically equivalent results (mean ≈ 16.5, SD ≈ 3.2) matching theoretical values (mean = 16.67, SD = 3.33), but Algorithm B demonstrates significant computational advantages.

## Course Information
**Course**: STAT550 - Applied Probability  
**Institution**: San Diego State University  
**Author**: Aiden B Jajo
