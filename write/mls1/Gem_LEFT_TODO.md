
### **Suggestions for Refactoring Your Methodology Section**

#### **Rationale for Changes**

Your current methodology section is good, but it describes the project's goals at a very high level. Your actual progress shows you are engaged in a much more specific and systematic foundational study. By restructuring the methodology, we can:

1.  **Align the Plan with Reality:** Showcase the detailed work you are currently doing on rheology and sliding laws as a formal, critical first phase of your project.
2.  **Create a Stronger Narrative:** Frame your project as a logical progression: first, systematically understand the forward problem (how the bed affects the surface under different physical rules), and then use that knowledge to build a better inverse model (BedSAT).
3.  **Highlight a Key Output:** Explicitly state that this foundational study will be the basis for your first peer-reviewed paper, which is a key milestone.

---

### **Suggested Refactored Text for `methodology.tex`**

Here is a draft of how you could rewrite the `\section{Research plan methodology}`. This version integrates the specific details from your "Progress" section into a phased approach.

**\section{Research plan methodology}**

My research plan is structured around the three main objectives of the project. The primary focus of the initial phase is on Objective 1: deriving the BedSAT method. This objective will be tackled in sequential phases, beginning with a foundational forward-modelling study before proceeding to the development of the inversion technique itself.

**Objective 1: Derive the BedSAT method**

This objective will be achieved through the following phased approach:

**Phase 1.1: Foundational Analysis of Bed-to-Surface Signal Transfer (Current Focus)**

The first critical step is to systematically quantify how fundamental physical assumptions influence the expression of subglacial topography at the ice surface. This directly addresses my first research question: "How does the bed topography manifest on the ice surface?". This foundational work will leverage the Ice-sheet and Sea-level System Model (ISSM) and a custom-built computational framework.

* [cite_start]**Synthetic Bedrock Generation:** I will generate a comprehensive suite of synthetic 1D bedrock profiles with systematically varying geometric properties, including amplitude, wavelength, skewness, and kurtosis[cite: 1758, 1759, 1761, 1762, 1763, 1764].
* [cite_start]**Systematic Forward Modelling:** Using these profiles, I will run a large ensemble of 2D ice flowline simulations using the full-Stokes equations[cite: 1771]. [cite_start]The experimental design is built around four benchmark scenarios to isolate the effects of different physical conditions[cite: 1773]:
    1.  [cite_start]No-slip (frozen) bed + Linear rheology (n=1)[cite: 1774].
    2.  [cite_start]No-slip (frozen) bed + Non-linear rheology (n=3)[cite: 1775].
    3.  [cite_start]Linear sliding + Linear rheology (n=1)[cite: 1776].
    4.  [cite_start]Linear sliding + Non-linear rheology (n=3)[cite: 1777].
* **Quantitative Analysis:** The simulation outputs will be rigorously analysed to quantify the bed-to-surface relationship. [cite_start]I will use cross-correlation analysis to calculate the precise phase shift and amplitude damping between the bedrock signal and the surface response[cite: 1797]. This will allow me to directly test and extend the theoretical predictions of Budd (1970) under fully non-linear conditions.
* **Anticipated Outcome and Publication:** This systematic study will produce a new set of constraints on bed-to-surface transfer functions that account for realistic ice dynamics. The results from this comprehensive analysis of rheology and sliding effects will form the basis of the **first peer-reviewed manuscript** of this PhD.

**Phase 1.2: Development of the BedSAT Inversion Framework**

The knowledge gained in Phase 1.1 will directly inform the development of the BedSAT inversion method.

* [cite_start]**Informed Transfer Functions:** By understanding how non-linear rheology and sliding conditions alter the surface expression of the bed, I can develop more physically robust transfer functions for the inversion process[cite: 1596].
* [cite_start]**Model Development and Validation:** The inversion model will be developed and tested using a regional catchment in Antarctica with extensive radar data, such as the Aurora Subglacial Basin[cite: 1582, 1583]. [cite_start]This will allow for direct validation of the inversion results against known bed configurations[cite: 1597, 1598]. [cite_start]The model will be constrained by available observations of surface velocity, thermal distribution, and ice thickness[cite: 1592, 1593, 1595]. [cite_start]The robustness of the model will be ensured through grid independence testing and a sensitivity analysis of model assumptions[cite: 1603, 1604].

**Objective 2: Derive a new bed topography for Antarctica using BedSAT**

[cite_start]The second phase of the project will apply the validated BedSAT methodology from Objective 1 to the entire Antarctic continent, deriving a new continent-wide bed topography dataset[cite: 1587]. [cite_start]Using covariance properties from existing radar surveys, I will generate multiple realisations of the bed, each with unique and statistically-consistent topographic roughness[cite: 1588].

**Objective 3: Evaluate the impact of the improved bed topography**

[cite_start]In the third and final phase, the new bed topography datasets will be used to conduct a sensitivity analysis of ice sheet model projections to 2300 CE[cite: 1589]. [cite_start]This will investigate the impact of the improved topography and different roughness realisations on ice dynamics, subglacial hydrology, and overall ice mass loss from Antarctica, directly addressing the project's main research questions[cite: 1576, 1577].