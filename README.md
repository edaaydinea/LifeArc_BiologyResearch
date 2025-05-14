# Project 1: Optimization of Fibroblast-to-Sensory Neuron Differentiation Protocol

## 1. Project Overview

This project, undertaken within LifeArc, focuses on developing and optimizing an *in vitro* model system of human sensory neurons. The primary goal is to create a reliable and reproducible platform for testing novel analgesic compounds by directly converting human skin fibroblasts into functional sensory neurons.

## 2. Background

Traditional pain research often relies on animal models or scarce primary human neurons. Direct reprogramming, or transdifferentiation, of easily accessible cells like fibroblasts into specific neuronal types offers a promising alternative. This project utilizes a method based on the ectopic expression of key neurogenic transcription factors (initially planned as BRN3A and NGN1, but Task 2 focused on NGN2 optimization) delivered via lentiviral vectors, combined with specialized culture conditions, to drive this conversion.

## 3. Current Task (Task 1): Experimental Design

This initial phase focused specifically on **designing an experiment to optimize the fibroblast-to-sensory neuron differentiation protocol**. The objectives were:

* Thoroughly analyze the baseline differentiation protocol provided.
* Identify key parameters and reagents suitable for optimization (e.g., viral MOI for neurogenic factors, growth factor concentrations like NT3).
* Define appropriate experimental conditions, including dose ranges for variables being tested.
* Determine necessary positive and negative controls.
* Structure the complete optimization experiment.

## 4. Methodology Employed (Initial Plan)

The core differentiation protocol involves:

* **Lentiviral Transduction:** Using pre-prepared lentiviruses to deliver neurogenic genes (e.g., NGN2) under the control of a doxycycline-inducible promoter.
* **Fibroblast Infection:** Infecting human fibroblasts with the lentiviral particles.
* **Induction:** Inducing transcription factor expression.
* **Culture & Differentiation:** Sequentially culturing the cells in specialized media and supplements (e.g., NT3) to support neuronal differentiation and survival.
* **Optimization Design:** Systematically varying selected parameters.

## 5. Key Project Files (For All Tasks)

* **`Experimental Protocol.pdf`**: Details the baseline protocol.
* **`Experiment design template (1).xlsx - Sheet1.csv`**: Output of the experimental design from Task 1.
* **`Task 1_LifeArc_Glossary.pdf`, `Task 3_LifeArc_Glossary.pdf`**: Glossaries defining key technical terms.
* **`Further reading.pdf`**: Suggested background reading materials.
* **`Data analysis notebook.Rmd`**: R Markdown for Task 2 MAP2 data analysis.
* **`Input data.txt`**: Data for Task 2.
* **`NGN2_barplot_outlier_removed.png`**: Key visual output from Task 2.
* **`Email_from_Ela.pdf`**: Colleague's follow-up data for Task 3.

## 6. Status & Next Steps (Post-Task 1)

* **Status:** The experimental design phase (Task 1) is complete.
* **Next Steps (were):** Execute the experiment, collect data, analyze results.

---

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

---

# Project 3: Synthesising Evidence for Functional Nociceptor Generation (Task 3)

## 1. Project Overview

This project integrates the findings from Task 2 (MAP2 optimization) with new experimental data from a colleague (Ela) focusing on specific nociceptor markers (TRPA+) and functionality (Ca2+ response to mustard oil). The goal is to make a more informed decision about the use of NT3 supplement in the differentiation protocol for generating functional nociceptors.

## 2. Background

While Task 2 showed that 10 ng/mL NT3 (with 5 MOI NGN2) increased the overall yield of MAP2+ mature neurons, MAP2 is a general neuronal marker. For pain research, the specific generation of functional nociceptors is crucial. Ela's experiments aimed to:

* Assess the proportion of TRPA+ cells (a nociceptor marker) among MAP2-GFP+ neurons.
* Measure the proportion of MAP2-GFP+ neurons showing a functional Ca2+ response to mustard oil (a nociceptor stimulant).
Both tests were done comparing 0 ng/mL NT3 vs. 10 ng/mL NT3, using the optimal 5 MOI NGN2 dose.

## 3. Current Task (Task 3): Synthesising Evidence and Collaboration

This phase focused on:

* Reviewing and interpreting Ela's TRPA+ expression and Ca2+ imaging data.
* Comparing Ela's findings with the MAP2 expression results from Task 2.
* Performing ballpark calculations to estimate the overall yield of TRPA+ and Ca2+ responsive cells relative to the total initial cell population under both NT3 conditions.
* Formulating a recommendation on the use of NT3 based on the combined evidence.
* Communicating these synthesized findings and recommendations to Ela.

## 4. Methodology Employed (Task 3)

1. **Comparative Analysis:** Ela's data (TRPA% and Ca2+ response % *within* MAP2-GFP+ cells) was compared with Task 2 data (overall MAP2+ yield).
2. **Yield Estimation:** Ballpark calculations were made:
    * `Overall Nociceptor Yield = (Task 2 MAP2+ % of total) * (Ela's Nociceptor-specific % within MAP2-GFP+)`
3. **Decision Making:** The benefits of NT3 (higher total MAP2+ and potentially TRPA+ cells) were weighed against its drawbacks (significantly lower proportion of Ca2+ responsive cells within the MAP2+ population, leading to no net gain in total Ca2+ responsive cells).
4. **Collaboration:** Findings and recommendations were structured for an email response to a colleague.

## 5. Key Findings from Task 3 Integration

* **TRPA+ Expression:**
  * Ela's data showed a slight, but not statistically significant (p=0.107), increase in the proportion of TRPA+ cells among MAP2-GFP+ neurons with 10 ng/mL NT3 (39%) compared to 0 ng/mL NT3 (37%).
  * Combined with Task 2's higher MAP2+ yield with NT3, the estimated *overall yield of TRPA+ cells from the total initial population was higher with NT3* (approx. 4.68% with NT3 vs. 3.15% without NT3).
* **Ca2+ Response (Functionality):**
  * Ela's data showed a statistically significant (p < 2.2e-16) *decrease* in the proportion of Ca2+ responsive cells among MAP2-GFP+ neurons with 10 ng/mL NT3 (22%) compared to 0 ng/mL NT3 (31%).
  * Despite NT3 increasing the total MAP2+ neuron yield (Task 2), the *estimated overall yield of Ca2+ responsive cells from the total initial population was virtually identical* with or without NT3 (approx. 2.64%).
* **Conclusion on NT3 Use:**
  * NT3 increases the total number of MAP2+ neurons and appears to increase the absolute number of TRPA+ expressing cells.
  * However, NT3 significantly reduces the *proportion* of functional (Ca2+ responsive) neurons within the MAP2+ population, resulting in no net gain in the absolute number of functionally responsive cells to mustard oil.
  * This presents a trade-off: NT3 yields more cells expressing a nociceptor marker but does not improve, and may even compromise, the functional quality (in terms of Ca2+ response proportion) of the neuronal population generated.

## 6. Status & Next Steps (Post-Task 3)

* **Status:** Synthesis of MAP2, TRPA+, and Ca2+ response data is complete. A nuanced understanding of NT3's role has been achieved. Provisional recommendations have been formulated and communicated to the collaborator (Ela).
* **Recommendation:** Based on the current data, if the primary goal is to maximize *functionally responsive nociceptors (Ca2+ assay)* as a proportion of differentiated neurons or to maintain a similar absolute number of functional cells without added cost/complexity, **omitting NT3 (0 ng/mL) with 5 MOI NGN2 appears to be a more favorable or equally effective condition.** If maximizing cells expressing the TRPA marker is prioritized, NT3 might be considered, but with the caveat of reduced functional responsiveness in the Ca2+ assay.
* **Next Steps:**
  * Further discussion with the team (including Ela's presentation) to decide on the definitive NT3 strategy.
  * Consideration of additional functional assays or markers to get a more comprehensive understanding of nociceptor "quality" under both NT3 conditions.
  * Investigate the *magnitude or characteristics* of the Ca2+ response, not just the percentage of responding cells.
  * Proceed with the chosen optimized protocol (5 MOI NGN2, and a decision on NT3) for generating nociceptors for compound screening.

---

# Project 4: Results Presentation and Strategic Recommendations (Task 4)

## 1. Project Overview

This project culminates the initial optimization phase by synthesizing and presenting the experimental findings from Tasks 1, 2, and 3. The primary goal is to communicate the results of the fibroblast-to-sensory neuron differentiation protocol optimization, including the analysis of MAP2 expression and functional nociceptor data, to the team and provide data-driven recommendations for future work.

## 2. Background

Previous tasks established the experimental design (Task 1), identified optimal conditions for maximizing general neuronal yield based on MAP2 expression (Task 2: 5 MOI NGN2 + 10 ng/mL NT3), and integrated these findings with colleague Ela's data on nociceptor-specific markers and function (Task 3). Task 3 revealed a trade-off regarding NT3 use: while it increases total MAP2+ and TRPA+ cell numbers, it reduces the proportion of functionally responsive (Ca2+) neurons, leading to no net gain in functional cell yield. This comprehensive dataset now requires clear communication to inform strategic decisions.

## 3. Current Task (Task 4): Presentation of Results and Recommendations

This phase focuses specifically on:

* Populating a standardized presentation template with key data, plots, and summaries from Tasks 1, 2, and 3.
* Clearly summarizing the experimental aims, design, and results (MAP2 analysis, TRPA+ analysis, Ca2+ functional analysis).
* Articulating the conclusions regarding optimal conditions for both general mature neurons and functional nociceptors.
* Presenting the calculated overall efficiency for generating functional nociceptors (~2.6%).
* Formulating and presenting clear recommendations for the next steps, including the preferred protocol conditions and potential needs for further optimization or enrichment.
* Preparing concise speaker notes to deliver a clear, informal (~10 minute) work-in-progress style presentation.

## 4. Methodology Employed (Task 4)

1.  **Template Population:** Utilized the provided PowerPoint template (`Presentation template.pptx`).
2.  **Data Integration:** Inserted key data plots (MAP2 bar chart, logistic regression effect plots, Ela's TRPA+ and Ca2+ response plots) into the template.
3.  **Content Synthesis:** Wrote concise summaries, interpretations, and conclusions for each slide, drawing directly from the analyses performed in Tasks 2 and 3.
4.  **Efficiency Calculation:** Included the previously calculated overall yield for functional nociceptors (~2.6%) in the conclusion slide.
5.  **Recommendation Formulation:** Developed specific recommendations based on the synthesized evidence, particularly addressing the NT3 dilemma and the low overall yield.
6.  **Presentation Preparation:** Drafted speaker notes to accompany the slides for a clear and timed delivery.

## 5. Key Outputs from Task 4

* A completed PowerPoint presentation summarizing the project aims, methods, key findings (MAP2 optimization, TRPA+ yield, Ca2+ functional yield), conclusions, and proposed next steps.
* Clear articulation of the recommended protocol conditions for generating functional nociceptors (5 MOI NGN2, likely without NT3 based on functional data).
* Highlighting the low overall efficiency (~2.6%) and the potential need for further optimization or enrichment before large-scale screening.
* Speaker notes to facilitate the presentation delivery.

## 6. Status & Next Steps (Post-Task 4)

* **Status:** Presentation summarizing the optimization findings and recommendations is prepared (and notionally delivered). Key insights communicated.
* **Next Steps:**
    * Facilitate team discussion based on the presented data to reach a consensus on the go-forward protocol, particularly the use of NT3.
    * Decide whether the current ~2.6% functional nociceptor yield is sufficient to proceed with pilot compound screening or if further protocol optimization/cell enrichment strategies (as proposed in the presentation) are necessary first.
    * Consider investigating the alternative markers or functional assays suggested to gain deeper insights into neuronal subtype specification and function.
    * Initiate the next phase of work based on the team's decision (e.g., start screening or plan new optimization experiments).