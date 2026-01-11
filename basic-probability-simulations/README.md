# Basic Probability Simulations
*Lab 2 from STAT550 - Applied Probability*

## Overview
This lab explores fundamental probability concepts through simulation, demonstrating the Law of Large Numbers and empirical probability estimation. Students use R to simulate coin flips and divisibility problems, observing how experimental outcomes converge to theoretical probabilities as sample size increases.

## Topics Covered

### Law of Large Numbers
- Long-run relative frequency interpretation of probability
- Convergence of empirical probabilities to theoretical values
- Effect of sample size on estimation accuracy
- Visualizing probability convergence over trials

### Biased vs. Fair Coins
- Simulating fair coins (P(heads) = 0.5)
- Simulating biased coins (P(heads) = 0.4)
- Using `prob` parameter in `sample()` function
- Comparing observed proportions to theoretical probabilities

### Cumulative Proportion Analysis
- Computing running proportions with `cumsum()`
- Creating time series plots of cumulative proportions
- Interpreting convergence patterns in visualizations
- Understanding early variation vs. long-run stability

### Divisibility Problems
- Using modular arithmetic (`%%` operator) in R
- Creating custom functions for simulation trials
- Using `replicate()` for repeated experiments
- Comparing empirical vs. theoretical probability calculations

### Statistical Analysis
- Demonstrating convergence with increasing sample sizes
- Observing how variability decreases with more trials
- Empirical probability estimation from simulations
- Inclusion-exclusion principle for divisibility

## Technologies Used
- R
- R Markdown
- xtable package
- pander package
- knitr package

## Files
- `basic_probability_simulations.Rmd` - R Markdown source code with lab exercises
- `basic_probability_simulations.pdf` - Knitted PDF output showing results
- `README.md` - Project documentation

## Key Concepts
- Law of Large Numbers (empirical convergence)
- Long-run relative frequency interpretation
- Empirical vs. theoretical probability
- Simulation-based probability estimation
- Modular arithmetic for divisibility testing
- Custom R functions for repeated experiments
- Statistical tables for results presentation

## Skills Demonstrated
- R programming for probability simulations
- Creating cumulative proportion plots
- Using `cumsum()` for running totals
- Writing custom simulation functions
- Using `replicate()` for experiment repetition
- Professional table formatting with xtable/pander
- Interpreting convergence patterns
- Understanding sampling variability

## Lab Exercises

### Task 1: Coin Flipping
Simulates 1000 flips of a biased coin (P(heads) = 0.4) and tracks the running proportion of heads. Demonstrates how the observed proportion stabilizes around the true probability as the number of tosses increases. Includes visualization showing early fluctuation followed by convergence.

### Task 2: Divisibility Probability
Simulates random integer selection from 1 to 5000 and tests divisibility by 4, 7, or 10. Compares empirical probabilities from 100, 1,000, 10,000, and 100,000 experiments to the theoretical probability of 0.40. Demonstrates how larger sample sizes yield more accurate estimates.

## Course Information
**Course**: STAT550 - Applied Probability  
**Institution**: San Diego State University  
**Author**: Aiden B Jajo
