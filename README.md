
# Integrated Flood-Risk Management for the IJssel River
Project with Ralph van Engelen
### Simulation, Multi-Objective Optimization & Robust Decision Making

[View Project Portfolio](https://lorenzobettin.github.io/projects/ijssel-flood-risk/)

## Overview

This project explores the design and evaluation of flood-risk
management strategies for a stylised IJssel River dike system
in the Netherlands.

Using Python and the Exploratory Modelling and Analysis (EMA)
Workbench, the study examines how flood-risk policies perform
across uncertain future conditions.

The objective is to identify strategies that balance economic
damage, human safety and investment costs while remaining
robust under uncertainty.

## Research Objective

How can flood-risk management strategies be designed and
evaluated to balance economic costs, casualties and flood
damage across a wide range of uncertain futures?

## Methodology

The analysis follows five main stages:

### 1. Exploratory Modelling

**Notebook:** `Exploratory_Modelling.ipynb`

- Simulated 40,000 uncertain scenarios for Zero Policy.
- Simulated 40,000 scenarios for One Policy.
- Compared baseline and maximum-intervention outcomes.

### 2. Scenario Discovery

**Notebook:** `Scenario_Discovery.ipynb`

- Applied the Patient Rule Induction Method (PRIM).
- Identified combinations of uncertain conditions associated
  with severe flood-risk outcomes.
- Selected representative scenarios for subsequent analysis.

### 3. Global Sensitivity Analysis

**Notebook:** `Sensitivity_Analysis.ipynb`

- Applied Sobol sensitivity analysis.
- Evaluated uncertainties affecting expected annual damage
  and fatalities.
- Identified influential dike-failure parameters.

### 4. Multi-Objective Optimization

**Notebook:** `Policy_Discovery.ipynb`

- Used the epsilon-NSGA-II optimization algorithm.
- Explored policies balancing five performance objectives.
- Examined Pareto-optimal alternatives and policy trade-offs.

`Epsilon_Discovery.ipynb` contains additional optimization
experiments.

### 5. Policy Robustness Evaluation

**Notebook:** `Policy_Robustness.ipynb`

- Evaluated candidate policies across uncertain scenarios.
- Applied signal-to-noise and regret analysis.
- Compared policy performance and investment requirements.
- Examined practical constraints on policy interventions.

## Technologies

- Python
- EMA Workbench
- pandas and NumPy
- Matplotlib and Seaborn
- SALib
- scikit-learn
- Multi-objective optimization
- Robust Decision Making

## Policy Objectives

1. Minimize Expected Annual Damage.
2. Minimize Expected Number of Deaths.
3. Minimize Dike Investment Costs.
4. Minimize Room-for-the-River Investment Costs.
5. Minimize Evacuation Costs.

## Key Findings

- Dike-failure probabilities at A1 and A3 emerged as
  influential uncertainties.
- Scenario discovery identified combinations of parameters
  associated with particularly adverse outcomes.
- Optimization revealed trade-offs between investment costs,
  expected flood damage and casualties.
- Robustness assessment helped compare policies across
  uncertain futures rather than a single assumed scenario.

These findings concern a stylised simulation model and
should not be interpreted as actual flood predictions.

## Reproducibility

The notebooks use Python 3.9+ and several analytical
dependencies, including EMA Workbench.

The complete workflow also requires external model-input
files, including hydrological, economic and infrastructure
data referenced by the Python scripts.

Those input datasets are not included in this repository
unless explicitly provided. Consequently, the uploaded
code may not run end-to-end without additional files.

## Project Portfolio

For project background, figures, methodology and
interpretation, visit:

[Integrated Flood-Risk Management — Lorenzo Bettin](https://lorenzobettin.github.io/projects/ijssel-flood-risk/)

## Attribution

Academic modelling project. Team contributions, original
model authorship and third-party source material should
be credited as applicable.
