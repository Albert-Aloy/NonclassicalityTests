# Numerical Methods and Experimental Data from the paper *Theory-independent monitoring of the decoherence of a superconducting qubit with generalized contextuality*

This repository contains the numerical methods, code, and experimental data accompanying the paper [arXiv:2411.13421](https://arxiv.org/abs/2411.13421). The provided Jupyter notebook is self-contained, allowing users to reproduce the results presented in the paper. Additionally, it includes illustrative examples to demonstrate the methods in action. Feel free to contact us for any doubt or suggestion.

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
Demonstrate how to stack data matrices for different time evolutions into a single matrix for analysis.

### **Step 4**: State Space Transformation  
Find a transformation that aligns the states' consistent space with the unit sphere. Use this transformation to compare different state realized spaces.

### **Step 5**: Volume Analysis  
Compute the volume of state spaces for various time evolutions, examining how the volume changes as the qubit decoheres.

---

## Technical Notes

- The code is implemented and tested in **Python 3.9**.  
- We have noticed that higher versions of Python on Windows may conflict with the `cdd` package, though this issue can be ignored unless **Step 4** is relevant to your analysis.

---
