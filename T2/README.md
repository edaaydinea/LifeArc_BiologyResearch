# Project 2: Analysis of MAP2 Immunofluorescence Data for Neuronal Differentiation Optimization (Task 2)

## 1. Project Overview

This project focused on analyzing the results of the neuronal differentiation optimization experiment designed in Task 1. The primary goal was to identify the combination of NGN2 virus dose and NT3 supplement that yields the highest proportion of MAP2-positive cells (mature neurons).

## 2. Background

The experiment tested:

* Four doses of NGN2 virus (0, 2, 5, and 10 MOI).
* Two NT3 supplement concentrations (0 and 10 ng/mL).
* Three replicates per condition.
MAP2 expression was the primary outcome.

## 3. Current Task (Task 2): Data Analysis

This phase focused on:

* Visualizing NGN2 and NT3 effects on MAP2 expression.
* Identifying the treatment combination maximizing neuronal differentiation.
* Performing statistical analysis (logistic regression).

## 4. Methodology Employed (Task 2)

1. **Data Loading and Preprocessing:** Data loaded into R, treatment doses as categorical.
2. **Data Visualization:** Bar plots for mean MAP2+ cells.
3. **Statistical Analysis:** Logistic regression, outlier removal.
4. **Optimization:** Optimal treatment identified.

## 5. Key Findings from Task 2

* The optimal NGN2 virus dose was determined to be **5 MOI**.
* The addition of **NT3 supplement (10 ng/mL)** significantly increased the overall proportion of MAP2-positive mature neurons compared to no NT3, when combined with 5 MOI NGN2 (approx. 12% MAP2+ cells with NT3 vs. 8.5% MAP2+ cells without NT3).
* The combination of **5 MOI NGN2 and 10 ng/mL NT3** was recommended for maximizing MAP2+ neuron yield.

## 6. Status & Next Steps (Post-Task 2)

* **Status:** Data analysis for general neuronal maturation (MAP2 expression) complete. Optimal conditions for MAP2+ yield identified.
* **Next Steps (were):** Further characterization for specific neuronal subtypes relevant to pain research (nociceptors).
