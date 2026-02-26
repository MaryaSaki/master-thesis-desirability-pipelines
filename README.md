# Interactive Visualization of Multi-Objective Optimization  
## Using Desirability Functions  

**Master’s Thesis – M.Sc. Automation & IT**  
TH Köln – University of Applied Sciences (2026)  
Author: Maryam Saki  
Supervisor: Prof. Dr. Thomas Bartz-Beielstein  
Second Reviewer: Prof. Dr. Boris Naujoks

---

##  Overview

In multi-objective optimization (MOO), decision-makers are often confronted with large sets of Pareto-optimal solutions. Selecting a single preferred solution becomes challenging, especially when objectives conflict or when the dimensionality increases.

This project investigates **desirability functions** as a preference-based decision support mechanism integrated into a Python-based multi-objective optimization and visualization workflow.

The repository contains the full Jupyter-based experimental pipelines developed for systematic evaluation, visualization-driven interpretation, and real-world validation.

---
## 📊 Example Visualization

## 📊 Example Visualization

Pareto-front analysis on the ZDT1 benchmark.  
Left: Non-dominated vs dominated solutions.  
Right: Aggregated desirability-based ranking (color-coded).

![ZDT1 Analysis](figures/zdt1_analysis.png)

The color encoding represents aggregated desirability values, illustrating how preference-based ranking aligns with the Pareto-optimal set.

##  Research Objectives

This work addresses the following key questions:

- How reliably do desirability-based rankings align with Pareto-optimality?
- How can visualization improve interpretability of aggregated desirability scores?
- How does performance change for convex, multimodal, or disconnected Pareto fronts?
- Do desirability functions remain informative in many-objective settings?
- How robust is the framework under surrogate modeling and limited real-world data?

---

##  Methodology

A structured **three-stage evaluation framework** was developed:

### 🔹 Pipeline 1 — Benchmark Evaluation (ZDT & DTLZ)

- Quantitative evaluation using ZDT and DTLZ benchmark suites  
- Rank correlation and Pareto-based performance analysis  
- Comparison between non-dominated and dominated solutions  
- Analysis across convex, multimodal, and disconnected Pareto fronts  

---

### 🔹 Pipeline 2 — Visualization-Driven Analysis

Objective-space and decision-space visual exploration including:

- 2D and 3D scatter plots  
- Heatmaps  
- Bubble plots  
- RadVis projections  
- Parallel coordinate plots  
- Input-space contour and surface plots  
- Individual and aggregated desirability mappings  

This stage focuses on interpretability and preference-structure transparency.

---

### 🔹 Pipeline 3 — Real-World Case Study

- Application to an industrial dataset  
- Surrogate modeling (Random Forest)  
- NSGA-II optimization  
- Desirability-based ranking under predictive uncertainty  
- Decision-variable distribution analysis  

(Industrial dataset not included due to confidentiality.)

---

##  Technology Stack

- Python (Jupyter Notebook workflow)  
- NumPy, pandas, SciPy  
- scikit-learn (surrogate modeling)  
- Matplotlib (2D & 3D visualization)  
- spotdesirability (desirability aggregation)  
- spotoptim (Pareto utilities & optimization tools)  

---

## 📊 Key Contributions

- Development of a reproducible Jupyter-based MOO evaluation workflow  
- Systematic quantitative study on ZDT & DTLZ benchmark problems  
- Visualization-enhanced interpretation of desirability functions  
- Integration of desirability with surrogate-assisted optimization  
- Critical assessment of strengths and limitations of desirability-based decision support  

---

##  Key Insight

Desirability functions should be considered as a **decision-support layer**, not as a replacement for multi-objective optimizers.  

Their effectiveness strongly depends on objective-space geometry (e.g., convexity, multimodality, disconnected fronts) and must be interpreted in conjunction with visualization tools.

---

## Repository Structure

```
master-thesis-desirability-pipelines/
│
├── pipeline1/   # Benchmark evaluation
├── pipeline2/   # Visualization analysis
├── pipeline3/   # Real-world application
└── README.md
```

---

## ▶ How to Run

1. Clone the repository  
2. Install required dependencies  
3. Execute the Jupyter notebooks within each pipeline  

Recommended environment: Python 3.10+

---

##  Thesis Reference

Saki, M. (2026).  
*Interactive Visualization of Multi-Objective Optimization Using Desirability Functions.*  
Master’s Thesis, TH Köln – University of Applied Sciences.

---
