# STAT550 - Applied Probability
**San Diego State University | Professional Portfolio**

A comprehensive collection of probability theory applications through computational simulation and statistical analysis. This repository showcases advanced R programming skills, mathematical modeling, and Monte Carlo methods developed throughout an applied probability course.

## 📋 Repository Overview

This repository contains 11 professionally documented projects covering discrete and continuous probability distributions, random variable simulation, Monte Carlo methods, and statistical validation techniques. All code is enhanced with detailed comments, comprehensive README documentation, and follows reproducible research principles.

## 🎯 Key Skills Demonstrated

- **Statistical Computing**: Monte Carlo simulation, random number generation, distribution modeling
- **R Programming**: Advanced R techniques including custom functions, vectorization, and for-loop optimization
- **Mathematical Modeling**: Translating probability theory into computational implementations
- **Data Visualization**: Professional histograms, empirical CDFs, density plots, and probability visualizations
- **Statistical Analysis**: Hypothesis testing, goodness-of-fit tests, empirical validation
- **Documentation**: R Markdown reports with LaTeX mathematical notation and reproducible workflows

## 📊 Technologies Used

- **R** - Primary programming language for statistical computing
- **R Markdown** - Reproducible research and dynamic report generation
- **LaTeX** - Mathematical typesetting within R Markdown documents
- **Git** - Version control and portfolio management

### R Packages
`stats`, `graphics`, `knitr`, `xtable`, `pander`

## 📁 Repository Structure

### R Coding Assignments (RCA)

#### [RCA1: Monte Carlo Simulation & Combinatorics](./monte-carlo-simulation-combinatorics/)
Monte Carlo estimation of probabilities through large-scale simulation experiments. Implements combinatorial probability calculations and validates results against theoretical values.

**Key Concepts**: Monte Carlo methods, combinatorial probability, empirical validation, simulation convergence

#### [RCA2: BMW Customer Interest Simulation](./bmw-customer-interest-simulation/)
Discrete probability simulation modeling customer purchase behavior using binomial distribution. Analyzes purchase probabilities and expected customer counts.

**Key Concepts**: Binomial distribution, probability mass functions, expected values, discrete simulation

#### [RCA3: Binomial Probability Analysis](./binomial-probability-analysis/)
Comprehensive binomial distribution analysis including parameter estimation, probability calculations, and conditional probability. Applications include quality control and survey analysis.

**Key Concepts**: Binomial PMF/CDF, parameter fitting, conditional probability, statistical inference

#### [RCA4: Probability Distributions Analysis](./probability-distributions-analysis/)
Survey of discrete probability distributions including Poisson, negative binomial, geometric, hypergeometric, exponential, and multinomial. Real-world applications across multiple domains.

**Key Concepts**: Multiple distribution families, parameter interpretation, distribution selection, applied probability

#### [RCA5: Continuous Probability Distributions](./continuous-probability-distributions/)
Analysis of continuous distributions including normal, exponential, and uniform. Covers percentile calculations, CDF derivations, and uniform distribution applications in quality control.

**Key Concepts**: Normal distribution, exponential distribution, uniform distribution, CDF/PDF relationships, percentile calculations

### Laboratory Exercises (Labs)

#### [Lab 1: R Simulation Fundamentals](./r-simulation-fundamentals/)
Introduction to R programming for probability simulation. Covers random sampling, for-loops, histograms, and Central Limit Theorem demonstration.

**Key Concepts**: R basics, `sample()` function, simulation loops, CLT visualization, histogram creation

#### [Lab 2: Basic Probability Simulations](./basic-probability-simulations/)
Law of Large Numbers demonstration through coin flip simulations. Explores empirical probability convergence and divisibility problems with modular arithmetic.

**Key Concepts**: Law of Large Numbers, empirical probability, convergence visualization, modular arithmetic

#### [Lab 3: Conditional Probability Simulations](./conditional-probability-simulations/)
Birthday problem simulation and random permutation algorithms. Implements while loops for geometric distributions and analyzes card shuffling probabilities.

**Key Concepts**: Birthday paradox, geometric distribution, while loops, random permutations, conditional probability

#### [Lab 4: Random Number Generation & Simulation](./random-number-generation-simulation/)
Evaluation of pseudo-random number generators (RANDU, Matlab rand). Statistical validation using Kolmogorov-Smirnov tests and discrete distribution simulation.

**Key Concepts**: Linear congruential generators, K-S test, random number validation, empirical PMFs

#### [Lab 5: Discrete Probability Model Simulation](./discrete-probability-model-simulation/)
Algorithm comparison for negative binomial distribution generation. Evaluates computational efficiency and validates against theoretical values.

**Key Concepts**: Negative binomial distribution, algorithm efficiency, recursion relations, computational complexity

#### [Lab 6: Continuous Random Variable Simulation](./continuous-random-variable-simulation/)
Box-Muller algorithm implementation for Gaussian random variate generation. Demonstrates transformation methods and validates empirical rule (68-95-99.7).

**Key Concepts**: Box-Muller transformation, normal distribution, transformation of random variables, empirical rule validation

## 🎓 Learning Outcomes

Through these projects, I developed proficiency in:

1. **Probability Theory Application**: Converting theoretical probability concepts into computational implementations
2. **Monte Carlo Methods**: Designing and executing large-scale simulation experiments for probability estimation
3. **Statistical Validation**: Comparing empirical results to theoretical distributions using formal hypothesis tests
4. **Algorithm Development**: Implementing and optimizing probability distribution simulators
5. **R Programming**: Advanced R techniques including custom functions, vectorization, and efficient loops
6. **Professional Documentation**: Creating reproducible research documents with R Markdown and comprehensive README files
7. **Data Visualization**: Designing clear, informative statistical graphics for probability distributions
8. **Mathematical Modeling**: Translating mathematical formulas and algorithms into working code

## 📈 Project Highlights

### Monte Carlo Convergence Analysis
Demonstrated Law of Large Numbers through biased coin flip simulation showing convergence from high early variability to stable long-run probabilities matching theoretical values.

### Birthday Paradox Validation
Empirical verification that 47 people are needed for 95% probability of shared birthdays, confirming counterintuitive theoretical result through 10,000 simulation trials.

### Algorithm Efficiency Comparison
Compared two negative binomial generators showing 2x speedup using recursion-based inverse CDF method versus sum-of-geometrics approach, with identical statistical accuracy.

### Box-Muller Implementation
Successfully implemented transformation method converting uniform random numbers to normal variates, validated against 68-95-99.7 empirical rule with <1% error.

### Random Number Generator Evaluation
Validated Matlab's original `rand` command using Kolmogorov-Smirnov test (p-value = 0.37), confirming uniform distribution quality of linear congruential generator.

## 🔍 Repository Statistics

- **Total Projects**: 11 (5 R Coding Assignments + 6 Labs)
- **Lines of Code**: 2,000+ lines of documented R code
- **Simulation Trials**: 100,000+ Monte Carlo experiments across all projects
- **Distributions Covered**: 10+ probability distributions (discrete and continuous)
- **Documentation**: 11 comprehensive README files + inline code comments

## 💼 Professional Applications

The skills demonstrated in this repository are directly applicable to:

- **Data Science**: Statistical modeling, simulation-based inference, Monte Carlo methods
- **Financial Modeling**: Risk analysis, option pricing, portfolio simulation
- **Machine Learning**: Random sampling, probabilistic algorithms, distribution fitting
- **Operations Research**: Queueing theory, inventory modeling, discrete event simulation
- **Quality Control**: Process monitoring, acceptance sampling, reliability analysis
- **Actuarial Science**: Risk assessment, insurance modeling, probability analysis

## 📚 Course Information

**Course**: STAT550 - Applied Probability  
**Institution**: San Diego State University  
**Instructor**: Professor Scott  
**Author**: Aiden B Jajo  

## 📖 How to Use This Repository

Each project folder contains:
- **`.Rmd` file**: Complete R Markdown source code with detailed comments
- **`.pdf` file**: Knitted report showing code execution and results
- **`README.md`**: Project documentation with overview, concepts, and key findings

To reproduce any analysis:
1. Clone this repository
2. Open the `.Rmd` file in RStudio
3. Install required packages listed in the file header
4. Knit to PDF or run code chunks interactively

## 🔗 Related Skills

- Statistical Computing & Simulation
- R Programming & Data Analysis
- Monte Carlo Methods
- Probability Theory & Stochastic Processes
- Algorithm Design & Optimization
- Scientific Writing & Documentation
- Reproducible Research Practices

## 🤝 Connect

This repository showcases academic work completed as part of my computer science degree at San Diego State University. For professional inquiries or collaboration opportunities, please reach out through LinkedIn.

---

*Portfolio curated and documented by Aiden B Jajo | San Diego State University Computer Science*
