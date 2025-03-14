# TestSmells-LLMs_EmpiricalStudy_ReplicationPackage

# Overview

This repository contains the resources and results from a study investigating the impact of refactoring performed by Large Language Models on test smells, which include GPT-4, Gemini 1.5 Pro and LLaMA 3 70B. The study involved evaluating various prompt templates for detecting and refactoring test smells, analyzing the outcomes, assessing the impact on code coverage metrics, and documenting the entire process.

## Repository Structure

### Prompt Templates

The `prompt templates` folder includes templates used in projects Python and Java:
- **10 templates** for **test smell detection**
- **10 templates** for **test smell refactoring**
>All text files

These templates were used to guide the analysis and refactoring processes.

### Dataset

The `dataset` folder contains the URLs of the repositories used in this study, which served as the basis for evaluating the effectiveness of the refactoring techniques. It includes:
- An `.xlsx` file with structured data.

### Results

The `results` folder contains the outcomes of the refactoring process. Each project was refactored with respect to a specific type of test smell, and the refactoring was performed using all LLMs. The folder includes:
- **Changes in code coverage metrics**: Analysis of how refactoring impacted code coverage.
- **Mitigated and introduced test smells**: Documentation of test smells that were resolved or introduced during the refactoring process.
- **Comparative results**: Outcomes from refactoring performed by each LLM, enabling a comparison of their effectiveness.
- **The projects refactored by each LLM**
>The *final* results are those outcomes achieved with the best prompt template.

### Source Code

The `src` folder includes the scripts used to:

- Send prompts to the models.
- Save and process the results.


## Usage

To replicate or extend this study, follow the instructions provided in the `README` files within each folder. Ensure all dependencies are installed and the dataset is properly configured before running the scripts.