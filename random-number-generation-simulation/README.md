# Random Number Generation & Simulation
*Lab 4 from STAT550 - Applied Probability*

## Overview
This lab explores pseudo-random number generation and discrete distribution simulation. Students evaluate linear congruential generators (LCG) used historically in computing, test uniformity using statistical methods, and simulate discrete probability distributions through repeated sampling experiments. The lab demonstrates both the theory behind random number generation and practical applications in probability estimation.

## Topics Covered

### Pseudo-Random Number Generation
- Linear congruential generators (LCG)
- RANDU generator: $X_{n+1} = 65539 X_n \mod 2^{31}$
- Matlab's original rand: $X_{n+1} = 16807 X_n \mod (2^{31}-1)$
- Seed values and deterministic sequences
- Scaling to uniform [0,1] interval

### Statistical Validation of Generators
- Histogram analysis for visual uniformity assessment
- Empirical cumulative distribution functions (ECDF)
- Kolmogorov-Smirnov (K-S) goodness-of-fit test
- Comparing empirical vs. theoretical distributions
- Hypothesis testing at $\alpha = 0.05$ significance level

### Discrete Distribution Simulation
- Sampling without replacement
- Hypergeometric distribution applications
- Empirical probability mass functions (PMF)
- Large-scale simulation experiments (10,000 trials)
- Mean and variance estimation from simulations

### Validation Techniques
- Visual assessment with histograms
- Probability plots (P-P plots)
- Statistical hypothesis testing
- Comparing empirical results to theoretical values
- Assessing convergence with large sample sizes

## Technologies Used
- R
- R Markdown
- knitr package
- xtable package
- pander package

## Files
- `random_number_generation_simulation.Rmd` - R Markdown source code with lab exercises
- `random_number_generation_simulation.pdf` - Knitted PDF output showing results
- `README.md` - Project documentation

## Key Concepts
- Linear congruential generators (LCG) for pseudo-random numbers
- Modular arithmetic in random number generation
- Uniform distribution on [0,1]
- Kolmogorov-Smirnov test for distribution validation
- Empirical CDF construction
- Probability mass functions (PMF)
- Sampling without replacement
- Law of Large Numbers validation
- Discrete probability distribution estimation

## Skills Demonstrated
- Implementing random number generators from formulas
- Statistical testing with K-S test
- Creating empirical distribution functions with `plot.ecdf()`
- Large-scale simulation experiments (10,000+ trials)
- Computing empirical probability distributions
- Comparing simulation results to theoretical values
- Data frame construction for results presentation
- Visual and statistical validation of randomness
- Professional statistical reporting

## Lab Exercises

### Task 1: Random Number Generator Evaluation
Implements and evaluates Matlab's original `rand` command using the linear congruential formula $X_{n+1} = 16807 X_n \mod (2^{31}-1)$. Generates 1000 pseudo-random numbers and validates uniformity through:
- Histogram showing distribution across [0,1] interval
- Empirical CDF compared to theoretical uniform distribution
- Kolmogorov-Smirnov test (p-value = 0.3709, failing to reject uniformity)

Demonstrates that this LCG produces statistically acceptable uniform random numbers.

### Task 2: Marble Drawing Simulation
Simulates drawing 3 marbles without replacement from a bag containing 1 red, 2 blue, 3 green, and 4 yellow marbles. Runs 10,000 experiments to estimate:
- Empirical PMF for blue marbles: P(B=0)≈0.465, P(B=1)≈0.468, P(B=2)≈0.068
- Empirical PMF for yellow marbles: P(Y=0)≈0.175, P(Y=1)≈0.494, P(Y=2)≈0.303, P(Y=3)≈0.029
- Mean and variance for both distributions

Results match theoretical probabilities within 1%, validating the simulation approach and demonstrating the Law of Large Numbers.

## Course Information
**Course**: STAT550 - Applied Probability  
**Institution**: San Diego State University  
**Author**: Aiden B Jajo
