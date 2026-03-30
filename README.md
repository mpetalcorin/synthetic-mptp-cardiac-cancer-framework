# synthetic-mptp-cardiac-cancer-framework
A synthetic, literature-benchmarked Python framework for modeling mitochondrial permeability transition pore dynamics across cardiac ischemia-reperfusion and cancer-associated stress states.
<img width="1293" height="774" alt="Screenshot 2026-03-31 at 00 40 30" src="https://github.com/user-attachments/assets/750a130f-bb12-4a00-8292-732cd659ec76" />
# Synthetic Proof-of-Concept Framework for Modeling Mitochondrial Permeability Transition Pore Dynamics Across Cardiac Injury and Cancer-Associated Stress States

## Overview

This repository contains a proof-of-concept computational framework for simulating mitochondrial permeability transition pore, mPTP, behavior across biologically distinct stress states relevant to cardiac injury and cancer-associated mitochondrial adaptation. The project uses synthetic, literature-benchmarked data to model how mitochondrial membrane potential, matrix calcium, mitochondrial reactive oxygen species, and candidate pore-regulatory mechanisms interact to influence sustained pore opening, mitochondrial DNA release, ATP-linked bioenergetic output, and cell viability.

The main aim is to provide an interpretable simulation platform for hypothesis generation, mechanistic prioritization, and future experimental design. This repository is not intended to provide clinically validated predictions or direct biological truth. Instead, it offers a structured computational environment for exploring state-dependent mitochondrial dysfunction.

## Biological Motivation

The mitochondrial permeability transition pore is a central mediator of mitochondrial stress responses. Sustained opening of the pore can collapse membrane potential, impair oxidative phosphorylation, promote matrix swelling, trigger mitochondrial DNA release, and reduce cell survival. These processes are especially relevant in myocardial ischemia-reperfusion injury and in cancer cells that adapt to chronic metabolic and oxidative stress.

Because the precise molecular architecture of the pore remains debated, this project does not attempt to prove a single structural model. Instead, it treats Cyclophilin D-associated sensitization, adenine nucleotide translocator-related function, and ATP synthase-associated pore propensity as biologically motivated mechanistic variables that can be perturbed and compared computationally.

## Repository Contents

This repository includes a Jupyter notebook that generates and analyzes a synthetic single-cell dataset representing four modeled biological states:

1. Cardiac Control  
2. Cardiac Ischemia-Reperfusion  
3. Cancer Therapy-Naive  
4. Cancer Stress-Adapted  

The analysis includes descriptive visualizations, grouped perturbation heatmaps, machine learning classification of sustained pore opening, regression of downstream injury-related outcomes, and counterfactual perturbation analysis.

Typical outputs include:

- Boxplots of mitochondrial membrane potential, matrix calcium, mtROS, sustained pore opening probability, and viability
- Heatmaps summarizing perturbation effects across disease states
- Permutation feature importance for sustained pore opening classification
- Observed-versus-predicted regression plots for viability and mitochondrial DNA release
- Summary tables for state-level statistics and grouped perturbation outcomes
- Synthetic single-cell dataset export

## Files

Suggested file organization:

- `mPTP_proof_of_concept_simulation.ipynb`  
  Main notebook containing synthetic data generation, analysis, visualization, and export of outputs

- `README.md`  
  Repository overview, motivation, usage, and interpretation guidance

- `modelcard.md`  
  Model card describing the synthetic modeling framework, intended use, limitations, and performance interpretation

- `datasheet.md`  
  Datasheet describing the synthetic dataset, how it was created, what variables are included, and appropriate use

- `outputs/`  
  Directory containing exported figures, tables, and synthetic datasets

## Methods Summary

The project simulates a synthetic single-cell dataset using state-dependent distributions for the following mitochondrial variables:

- Mitochondrial membrane potential, Δψm
- Matrix calcium
- Mitochondrial reactive oxygen species, mtROS
- Cyclophilin D-related sensitization
- ANT-related function
- ATP synthase-associated pore propensity

These variables are used to generate downstream outcomes:

- Transient pore-related score
- Sustained pore opening probability
- Sustained pore opening status
- Mitochondrial DNA release
- ATP index
- Viability fraction

The framework also applies simulated perturbation conditions:

- WT
- CypD_low
- ANT_low
- ATPsyn_low
- ANT_ATPsyn_low

These perturbations allow comparison of state-dependent protection or vulnerability across the four biological contexts.

## How to Run

1. Open the notebook.
2. Run all cells in sequence.
3. Review generated figures and summary tables.
4. Inspect exported outputs in the designated output directory.

## Dependencies

Typical Python dependencies include:

- Python 3
- numpy
- pandas
- matplotlib
- scikit-learn
- pathlib

Depending on notebook implementation, additional standard scientific Python packages may also be used.

## Intended Use

This repository is intended for:

- Proof-of-concept simulation
- Hypothesis generation
- Computational benchmarking
- Method development for interpretable machine learning on mitochondrial stress data
- Educational demonstration of state-dependent mPTP behavior
- Planning future experimental studies

## Not Intended For

This repository is not intended for:

- Clinical diagnosis
- Clinical decision-making
- Patient risk prediction
- Definitive mechanistic proof of mPTP structure
- Quantitative estimation of treatment effect in real biological systems without experimental calibration

## Interpretation Notes

The outputs generated by this repository should be interpreted as synthetic and biologically motivated, not experimentally measured. Numerical values are useful for exploring relationships and testing workflows, but they should not be treated as direct biological truth. Any mechanistic conclusions require validation using real experimental systems.

## Citation
Petalcorin, M.I.R. (2026). A Synthetic Proof-of-Concept Framework for Modeling Mitochondrial Permeability Transition Pore Dynamics Across Cardiac Injury and Cancer-Associated Stress States. https://github.com/mpetalcorin/synthetic-mptp-cardiac-cancer-framework

If you use this repository in academic work, cite the associated manuscript or project description for the synthetic mPTP proof-of-concept framework.

## License

MIT License

## Contact

m.petalcorin@gmail.com
