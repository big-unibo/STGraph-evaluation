# STGraph - something for someone

## Research papers

This repository contains the evaluation pipelines and results of the following research paper:

- Francia, Matteo, Golfarelli Matteo, and Pasini Manuele. "STGraph - A something for someone". Submitted to **somewhere** (2025).

## Getting Started
### Repository organization
- `/data`: contains experimental data mentioned in the article
- `/figures`: contains the article figures.
- `/architectures`: contains the implementations of STGraph and its competitors.
- `STGraph.ipynb`: Python notebook to reproduce articles figures from data.

### Experiments reproducibility

All data and figures are reproducible through Docker (no other mandatory dependencies required).

To reproduce the experiments, open a shell within the project folder and run:
   ```sh
   ./run_tests.sh
   ```
All the configurations required to run the experiments are specified in the .env.example file.
The above command needs to be run twice, the first one creates the .env from the .env.example, the second one runs the experiments through Docker.
The .env file can be modified accordingly w.r.t. the configuration to be tested.

Tests' results data which will then be available in the `/data` folder and appended to previous experiments' results.


#### Reproducing scale-out tests

Scale-out tests are not directly reproducible due 
