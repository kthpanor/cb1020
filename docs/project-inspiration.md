# Project inspiration

## Agent-based modeling

### Detecting driving forces of biomolecular interactions
Agent-based modelling and simulation have been effectively applied to the study of complex biological systems, especially when composed of many interacting entities. Representing biomolecules as autonomous agents allows this approach to bring out the global behaviour of biochemical processes as resulting from local molecular interactions. In this paper, we leverage the capabilities of the agent paradigm to construct an in silico replica of the glycolytic pathway; the aim is to detect the role that long-range electrodynamic forces might have on the rate of glucose oxidation. Experimental evidences have shown that random encounters and short-range potentials might not be sufficient to explain the high efficiency of biochemical reactions in living cells. However, while the latest in vitro studies are limited by present-day technology, agent-based simulations provide an in silico support to the outcomes hitherto obtained and shed light on behaviours not yet well understood. Our results grasp properties hard to uncover through other computational methods, such as the effect of electromagnetic potentials on glycolytic oscillations [https://doi.org/10.1038/s41598-021-04205-8](https://doi.org/10.1038/s41598-021-04205-8).

:::{image} ../images/abm_biomolecular_interactions.jpg
:width: 400px
:align: center
:::


### Prostate tumor microenvironment
Inhibiting androgen receptor (AR) signaling through androgen deprivation therapy (ADT) reduces prostate cancer (PCa) growth in virtually all patients, but response may be temporary, in which case resistance develops, ultimately leading to lethal castration-resistant prostate cancer (CRPC). <br> The tumor microenvironment (TME) plays an important role in the development and progression of PCa. In addition to tumor cells, TME-resident macrophages and fibroblasts express AR and are therefore also affected by ADT. However, the interplay of different TME cell types in the development of CRPC remains largely unexplored. To understand the complex stochastic nature of cell-cell interactions, we created a PCa-specific agent-based model (PCABM) based on *in vitro* cell proliferation data [https://doi.org/10.1038/s41540-024-00344-6](https://doi.org/10.1038/s41540-024-00344-6).

:::{image} ../images/abm-cancer-model.png
:width: 400px
:align: center
:::

### Population dynamics of sea turtles under different temperature scenarios (CB1020 HT23)
There is a direct correlation between the number of male turtle hatchlings and the temperature during nesting season; increasing temperatures lead to decreasing number of males. The dynamics and interactions between sea turtles during and outside mating season can be modeled using ABM. By letting the temperature increase during the simulation, the effect of increasing temperatures on the gender distribution and reproduction patterns of sea turtles is illustrated.

### Modeling the genetic damage of arsenic (CB1020 HT23)
Reactive oxygen species are byproducts of mitochondrial metabolism. In healthy mitochondria, there is a balance in the levels of ROS being produced, converted and consumed. One of the effects of arsenic in the cell is an increased amount of reactive oxygen species (ROS).
If the concentration of ROSs becomes too high, it can cause damage to the host.
This damage can be countered by the Base Excision Repair (BER) pathway, a DNA damage repair mechanism. With ABM, the course of ROS-induced damage followed by the repair mechanism can be simulated and the effect of different arsenic intakes and the time and amount it takes to cause permanent gene damage can be simulated and studied.

## AI/ML

### Graph neural networks learn emergent tissue properties from spatial molecular profiles
Tissue phenotypes, such as metabolic states, inflammation, and tumor properties, emerge from both molecular states and spatial cell organization. Spatial molecular assays provide an unbiased view of tissue architecture, enabling phenotype prediction. Graph neural networks (GNNs) offer a natural framework for analyzing spatial proteomics by integrating expression profiles with structure. We apply GNNs to classify tissue phenotypes using spatial cell patterns. We show that for relatively simple classification tasks, such as tumor grading in breast cancer, incorporating spatial context does not significantly improve predictive performance over models trained on single-cell or pseudobulk representations. However, GNNs capture meaningful spatial features, retaining prognostic signals beyond tumor labels, highlighting tumor-grade-specific cell type interactions, and uncovering complex immune infiltration patterns in colorectal cancer not detectable with traditional approaches. These findings suggest that while spatial dependencies may not always enhance classification performance in small datasets, GNNs remain valuable tools for characterizing tissue organization and interactions [https://doi.org/10.1038/s41467-025-63758-8](https://doi.org/10.1038/s41467-025-63758-8).

:::{image} ../images/gnn_tissue.png
:width: 600px
:align: center
:::

### Machine Learning-Guided Protein Engineering
Find inspiration for using machine learning in protein engineering in the perspective article below. The authors provide an overview of ongoing trends in this domain, highlight recent case studies, and examine the current limitations of machine learning-based methods [https://doi.org/10.1021/acscatal.3c02743](https://doi.org/10.1021/acscatal.3c02743). They present their opinions on the fundamental problems and outline the potential directions for future research.

:::{image} ../images/ml_protein.jpeg
:width: 400px
:align: center
:::

### A new era of artificial intelligence in neuroradiology
Find inspiration in this review on the use of AI-based techniques in neuroradiology, focusing on conditions such as vascular diseases, epilepsy, and demyelinating and neurodegenerative conditions [https://dx.doi.org/10.1055/s-0044-1779486](https://dx.doi.org/10.1055/s-0044-1779486). Some of the algorithms behind the applications are introduced, briefly discussing a few of the challenges of generalization in the use of AI models in neuroradiology. If well designed, AI algorithms have the potential to radically improve radiology, strengthening image analysis, enhancing the value of quantitative imaging techniques, and mitigating diagnostic errors.

:::{image} ../images/ml_models.jpg
:width: 400px
:align: center
:::

### Identification of risk factors for cardiovascular disease using data analysis and machine learning (CB1020 HT24)
Cardiovascular disease (CVD) is the leading cause of death in Sweden, with over 2 million affected and approximately 30,000 annual deaths.<br>
The aim of this project was to use data analysis combined with the machine learning algorithms `GradientBoosting`, `RandomForest`, and `SHAP` in sklearn to investigate which five factors contribute most to CVD, and to use machine learning to predict whether a person has CVD or not.<br>
The project analyzed a file with patient data from 70,000 people in twelve different categories: age, height, weight, gender, systolic blood pressure, diastolic blood pressure, cholesterol level, glucose level, smoking, alcohol intake, physical activity and presence or absence of cardiovascular disease.

The five most important risk factors for CVD were identified as systolic and diastolic blood pressure, BMI, age, and cholesterol. The results showed that older people and individuals with higher BMI had an increased risk of CVD, which is consistent with previous research.<br>
The machine learning algorithms `GradientBoosting` and `RandomForest` demonstrated a test accuracy of 73.6%, with a better ability to identify CVD cases than non-CVD cases. Data analysis also indicated that there were shortcomings in the representation of different age groups and gender, which may have influenced the results.