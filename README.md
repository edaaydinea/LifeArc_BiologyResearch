# Project 1: Optimization of Fibroblast-to-Sensory Neuron Differentiation Protocol

## 1. Project Overview

This project, undertaken within LifeArc, focuses on developing and optimizing an *in vitro* model system of human sensory neurons. The primary goal is to create a reliable and reproducible platform for testing novel analgesic compounds by directly converting human skin fibroblasts into functional sensory neurons.

## 2. Background

Traditional pain research often relies on animal models or scarce primary human neurons. Direct reprogramming, or transdifferentiation, of easily accessible cells like fibroblasts into specific neuronal types offers a promising alternative. This project utilizes a method based on the ectopic expression of key neurogenic transcription factors (BRN3A and NGN1) delivered via lentiviral vectors, combined with specialized culture conditions, to drive this conversion.

## 3. Current Task: Experimental Design (Task 1)

This initial phase focuses specifically on **designing an experiment to optimize the fibroblast-to-sensory neuron differentiation protocol**. The objectives were:

* Thoroughly analyze the baseline differentiation protocol provided.
* Identify key parameters and reagents suitable for optimization (e.g., viral MOI, duration/concentration of doxycycline induction, composition/timing of media changes, growth factor concentrations).
* Define appropriate experimental conditions, including dose ranges for variables being tested.
* Determine necessary positive and negative controls (e.g., uninfected cells, cells infected with control virus).
* Structure the complete optimization experiment using the provided Excel template.

## 4. Methodology Employed

The core differentiation protocol involves:

* **Lentiviral Transduction:** Using pre-prepared lentiviruses to deliver BRN3A and NGN1 genes under the control of a doxycycline-inducible promoter (Tet-On system). A control virus (empty vector) is used for comparison.
* **Fibroblast Infection:** Infecting human fibroblasts (cultured in DMEM + 10% FBS) with the lentiviral particles at a target Multiplicity of Infection (MOI).
* **Induction:** Inducing transcription factor expression using doxycycline.
* **Culture & Differentiation:** Sequentially culturing the cells in specialized media (N3 medium, followed by DMEM/F12:Neurobasal mix supplemented with B27, NGF, BDNF, GDNF) to support neuronal differentiation and survival.
* **Optimization Design:** Systematically varying selected parameters across different experimental wells, as documented in the `Experiment design template (1).xlsx`.

## 5. Key Project Files

* **`Experimental Protocol.pdf`**: Details the baseline protocol for differentiating fibroblasts into sensory neurons (adapted from Blanchard et al., Nature Neurosci 2015).
* **`Experiment design template (1).xlsx - Sheet1.csv`**: The output/structure of the experimental design, outlining the conditions, variables, concentrations, and controls for the optimization experiment. (Note: This represents the plan laid out in the original Excel template).
* **`Task 1_LifeArc_Glossary.pdf`**: A glossary defining key technical terms relevant to this project phase.
* **`Further reading.pdf`**: A list of suggested background reading materials, including scientific reviews and technical notes.

## 6. Status & Next Steps

* **Status:** The experimental design phase (Task 1) is complete. The optimization strategy, including variables, ranges, and controls, has been defined.
* **Next Steps:**
  * Execute the designed optimization experiment based on the plan.
  * Collect data from multiple experimental readouts (to be defined in subsequent tasks).
  * Analyze the results to identify the optimal differentiation conditions.
  * Report the findings.

# Project 2: Analysis of MAP2 Immunofluorescence Data for Neuronal Differentiation Optimization

## 1. Project Overview

This project focuses on analyzing the results of a neuronal differentiation optimization experiment. The primary goal is to identify the combination of treatments that yields the highest proportion of MAP2-positive cells, which serve as a marker for neuronal differentiation. The analysis involves data visualization and statistical modeling to determine the optimal experimental conditions.

## 2. Background

The differentiation of fibroblasts into neurons is a critical step in developing reliable *in vitro* models for neuroscience research. This project builds on the experimental design phase (Project 1) by analyzing the data generated from the optimization experiment. The experiment tested various doses of NGN2 virus and the NT3 supplement to evaluate their effects on neuronal differentiation efficiency.

The experimental design included:

* Four doses of NGN2 virus (0, 2, 5, and 10 MOI).
* Two NT3 supplement concentrations (0 and 10 ng/mL).
* Three replicates per condition, resulting in 24 samples.

The proportion of MAP2-positive cells in each well was measured as the primary outcome.

## 3. Current Task: Data Analysis (Task 2)

This phase focuses on analyzing the experimental data to:

* Visualize the effects of NGN2 and NT3 on MAP2 expression.
* Identify the treatment combination that maximizes neuronal differentiation efficiency.
* Perform statistical analysis using logistic regression to formally test the effects of treatments.

## 4. Methodology Employed

The analysis involves the following steps:

1. **Data Loading and Preprocessing:**
   * The experimental data is loaded into R and preprocessed to represent treatment doses as categorical variables.

2. **Data Visualization:**
   * Bar plots are generated to visualize the mean proportion of MAP2-positive cells for each treatment condition, with error bars representing standard deviations.

3. **Statistical Analysis:**
   * Logistic regression is used to model the effects of NGN2 and NT3 on MAP2 expression.
   * Interaction effects between NGN2 and NT3 are tested.
   * Outlier removal is performed to ensure robust results.

4. **Optimization:**
   * The optimal treatment combination is identified based on the analysis results.

## 5. Key Project Files

* **`Data analysis notebook.Rmd`**: The R Markdown file containing the analysis code and documentation.
* **`Input data.txt`**: The raw experimental data file used for analysis.
* **`Output plots and tables`**: Visualizations and summary tables generated during the analysis.

## 6. Status & Next Steps

* **Status:** The data analysis phase (Task 2) is complete. The optimal treatment combination has been identified.
* **Next Steps:**
  * Validate the findings by repeating the experiment under the identified optimal conditions.
  * Extend the analysis to include additional experimental readouts, such as cell viability or morphology.
  * Report the findings in a scientific manuscript or presentation.
