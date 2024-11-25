# Numerical Methods and Experimental Data from the paper *Theory-independent monitoring of the decoherence of a superconducting qubit with generalized contextuality* [arXiv:2411.13421](https://arxiv.org/abs/2411.13421)

This repository contains the numerical methods, code, and experimental data accompanying the paper [(arXiv:2411.13421)](https://arxiv.org/abs/2411.13421). The provided Jupyter notebook is self-contained, allowing users to reproduce the results presented in the paper. Additionally, it includes illustrative examples to demonstrate the methods in action. Feel free to contact us for any doubt or suggestion.

---

## Organization of the Notebook

The notebook is structured into the following steps:

### **Step 0**: Import Dependencies  
Import the necessary packages and define most of the required functions.

### **Step 1**: Single-Rank Analysis  
Perform a case study to find a GPT model of a specific rank that best fits a given frequency table (see Section II.B of the paper).

### **Step 2**: Multi-Rank Analysis  
Iterate the single-rank analysis for multiple ranks to estimate which rank provides the best fit (see Section II.C of the paper).

### **Step 3**: Analysis for Different Time Evolutions  
Demonstrate how to stack frequency data matrices for different time evolutions into a single matrix to carry-out the above analysis based solely on the stacked matrix.

### **Step 4**: State Space Transformation  
Find a transformation that aligns the states' consistent space with the unit sphere. Use this transformation to normalize and compare different state realized spaces.

### **Step 5**: Volume Analysis  
Compute the volume of state spaces for various time evolutions, examining how the volume changes as the qubit decoheres.

---

The experimental data is organized into two main folders:

1. **`Data` Folder**:
   - This folder contains data from the experimental runs without time evolution in the preparation procedure.
   - Each file is named as `zzzGPTrun{run_number}`, where `{run_number}` goes from 1 to 10, labeling the experimental run.

2. **`Data_with_time_evolutions` Folder**:
   - This folder contains data from experimental runs where the qubit was allowed to evolve for a specified duration (`τ`) as part of the preparation procedure.
   - Each file is named as `zzzGPTwait{tau}run{run_number}`, where:
     - `{tau}` specifies the time duration in nanoseconds for which the qubit was left evolving.
     - `{run_number}` labels the specific experimental run.

Both folders also include pre-computed data from the jupyter notebook analysis.
    
---

## Technical Notes

- The code is implemented and tested in **Python 3.9**.  
- We have noticed that higher versions of Python on Windows may conflict with the `cdd` package, though this issue can be ignored unless **Step 4** is relevant to your analysis.

---
