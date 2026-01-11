# Continuous Random Variable Simulation
*Lab 6 from STAT550 - Applied Probability*

## Overview
This lab explores simulation techniques for continuous random variables and functions of random variables. Students work with uniform-to-normal transformations, implement the Box-Muller algorithm for Gaussian random variate generation, and visualize probability distributions through Monte Carlo simulation. The lab demonstrates transformation methods, empirical validation of theoretical distributions, and the empirical rule for normal distributions.

## Topics Covered

### Functions of Random Variables
- Transforming uniform random variables
- Linear transformations: H = √2 · X
- Expected value and variance of transformations
- Relationship between parent and derived distributions

### Isosceles Right Triangle Simulation
- Simulating side lengths from U(0,1)
- Calculating hypotenuse lengths via transformation
- Geometric visualization of random variates
- Empirical validation against theoretical values

### Box-Muller Transformation
- Converting uniform variates to normal variates
- Polar coordinate transformation method
- Algorithm: Z₁ = √(-2ln(U₁))cos(2πU₂), Z₂ = √(-2ln(U₁))sin(2πU₂)
- Scaling standard normal to arbitrary N(μ, σ²)

### Gaussian Distribution Properties
- The 68-95-99.7 empirical rule
- Probability within k standard deviations
- Monte Carlo estimation of normal probabilities
- Histogram density plots with theoretical overlays

### Statistical Validation
- Comparing empirical statistics to theoretical values
- Mean, variance, and median estimation
- Visual assessment with density overlays
- Large-scale Monte Carlo experiments (1000+ trials)

## Technologies Used
- R
- R Markdown

## Files
- `continuous_random_variable_simulation.Rmd` - R Markdown source code with lab exercises
- `continuous_random_variable_simulation.pdf` - Knitted PDF output showing results
- `README.md` - Project documentation

## Key Concepts
- Transformation of random variables
- Box-Muller algorithm for normal variate generation
- Monte Carlo integration and probability estimation
- Empirical rule (68-95-99.7) for normal distributions
- Linear transformations preserving distribution shape
- Expected value and variance of transformed variables
- Uniform random number generation as basis for all simulations

## Skills Demonstrated
- Implementing mathematical transformation algorithms
- Function creation in R for reusable code
- Geometric visualization with `plot()` and `lines()`
- Density histogram overlays
- Statistical validation of simulation results
- Understanding transformation method for random variate generation
- Professional visualization of continuous distributions
- Empirical probability estimation via simulation

## Lab Exercises

### Task 1: Triangle Hypotenuse Simulation
Simulates 500 isosceles right triangles with side lengths X ~ U(0,1) and calculates hypotenuses H = √2 · X. Results:
- Empirical mean: ~0.746 (theoretical: 0.707 = √2/2)
- Empirical variance: ~0.153 (theoretical: 0.167 = 1/6)
- Distribution: Uniform on [0, √2]

Creates striking visualization showing all 500 triangle hypotenuses overlaid, with darker regions indicating more frequently sampled values. Demonstrates that linear transformation of uniform random variable yields uniform distribution with scaled parameters.

### Task 2: Box-Muller Gaussian Simulation
Implements Box-Muller algorithm to generate 1000 variates from N(2, 2):

**Algorithm Steps:**
1. Generate pairs of uniform(0,1) random numbers
2. Apply transformation: Z₁ = √(-2ln(U₁))cos(2πU₂), Z₂ = √(-2ln(U₁))sin(2πU₂)
3. Scale to desired N(μ, σ²): X = σZ + μ

**Results:**
- Empirical mean: ~1.95 (theoretical: 2.0)
- Empirical SD: ~1.36 (theoretical: √2 ≈ 1.41)
- Empirical median: ~1.97 (theoretical: 2.0)

**Empirical Rule Validation:**
- Within 1 SD: ~70% (theoretical: 68%)
- Within 2 SD: ~96% (theoretical: 95%)
- Within 3 SD: ~99.9% (theoretical: 99.7%)

Histogram with theoretical normal density overlay demonstrates excellent agreement, validating both the Box-Muller algorithm implementation and the empirical rule for normal distributions.

## Mathematical Foundations

### Transformation Theory
For X ~ U(0,1) and H = √2 · X:
- E[H] = √2 · E[X] = √2/2
- Var(H) = 2 · Var(X) = 1/6

### Box-Muller Justification
Uses inverse transform and polar coordinate methods to convert rectangular uniform coordinates to Gaussian variates. Generates two independent standard normals from two independent uniforms.

## Course Information
**Course**: STAT550 - Applied Probability  
**Institution**: San Diego State University  
**Author**: Aiden B Jajo
