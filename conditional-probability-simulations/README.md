# Conditional Probability Simulations
*Lab 3 from STAT550 - Applied Probability*

## Overview
This lab explores conditional probability through simulation, focusing on the famous birthday problem and card shuffling probabilities. Students use for-loops and if-else statements to simulate complex probability scenarios, demonstrating how empirical methods can estimate probabilities for problems that are challenging to solve analytically.

## Topics Covered

### For-Loops for Simulation
- Embedding single experiments within for-loops
- Storing success indicators in vectors
- Computing empirical probabilities from simulation results
- Brute-force simulation approaches

### If-Else Statements vs. Boolean Expressions
- Using if-else statements to record successes
- Using Boolean expressions for conditional checks
- Comparing two approaches to the same problem
- Efficient coding practices for simulations

### Birthday Problem
- Classical probability paradox
- Simulating shared birthdays in groups
- Understanding counterintuitive probability results
- Finding threshold values through trial and error
- Extending to triple birthday matches

### Random Permutations
- Shuffling algorithms for random arrangements
- Card deck permutations
- Conditional probability with card suits
- Modular arithmetic for suit identification

### Empirical Probability Estimation
- Running large-scale simulations (1000-10000 trials)
- Comparing empirical results to theoretical values
- Understanding simulation variability
- Trial-and-error parameter search

## Technologies Used
- R
- R Markdown

## Files
- `conditional_probability_simulations.Rmd` - R Markdown source code with lab exercises
- `conditional_probability_simulations.pdf` - Knitted PDF output showing results
- `README.md` - Project documentation

## Key Concepts
- Birthday paradox and its surprising results
- Conditional probability through simulation
- Random permutation algorithms
- Modular arithmetic for grouping (suit detection)
- Empirical vs. theoretical probability comparison
- Frequency table analysis with `table()` function
- Success indicator vectors for probability estimation

## Skills Demonstrated
- For-loop construction for repeated simulations
- If-else statement logic
- Boolean expression evaluation
- Random sampling and permutation
- Probability estimation from simulation data
- Trial-and-error optimization
- Algorithm implementation from pseudocode
- Statistical reasoning about counterintuitive results

## Lab Exercises

### Task 1: Birthday Problem
Simulates the famous birthday paradox to estimate:
- Probability that 2 people share a birthday in a class of 23 (~50%)
- Minimum class size needed for 95% probability of a match (47 students)
- Probability that 3 people share a birthday in a class of 50 (~14%)

Demonstrates how quickly probabilities increase with group size and provides intuition for this counterintuitive result.

### Task 2: Card Shuffling
Implements a random permutation algorithm to shuffle a 52-card deck and estimates the probability that the top and bottom cards are the same suit (~25% or 1/4). Uses modular arithmetic with `floor()` to identify card suits and demonstrates conditional probability in a familiar context.

## Course Information
**Course**: STAT550 - Applied Probability  
**Institution**: San Diego State University  
**Author**: Aiden B Jajo
