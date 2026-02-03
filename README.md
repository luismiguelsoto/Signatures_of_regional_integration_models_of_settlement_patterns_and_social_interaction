Signatures of regional integration and models of settlement patterns in the Tairona and Quimbaya chiefdoms (under review)
--------------------------------------------------------------

This repository contains code and data for a multidimensional spatial analysis framework designed to evaluate regional integration in chiefdom societies. The protocol integrates (1) Area-weighted Kernel Density Estimation (KDE) for nucleation intensity, (2) Approximate Bayesian Computation (ABC) for generative settlement models, (3) Topological Data Analysis (TDA) using persistent homology for spatial complexity, (4) k-NN networks for connectivity analysis, and (5) Random Forest classification. The protocol is applied comparatively to two pre-Hispanic sequences in Colombia: the Tairona tradition (Río Frío) and the Quimbaya tradition (Filandia).

Repository Structure:
----------------------------------
1. GIS:
   - Contains the spatial data files (shapefile components) defining the study areas and settlement distributions. The R code downloads these automatically from this repository:
     • Rio_Frio_Limite_Survey (Survey boundary)
     • Rio_Frio_Sitios_Neguanje (Periods: Neguanje, Buritaca, Tairona)
     • Filandia_Limite_Survey (Survey boundary)
     • Filandia_Sitios_Periodo_Temprano (Periods: Early, Middle, Late)

2. R Code Files:
   - The main R script (JAS_RNOTEBOOK_CLEAN.Rmd) contains the code to:
     a) Load required packages and configure the environment.
     b) Download GIS files directly from GitHub using a raw URL connection.
     c) Perform spatial metric calculations, TDA, network analysis, and ML classification.
     d) Generate Figures 2 through 7 and Tables 1 & 2 as presented in the manuscript.

Software and Key Package Versions:
----------------------------------
- R version: [R 4.5.2 (2025-10-31 ucrt)]
- Platform: Windows 11 x64 (build 26200)

Key R packages used in this project include (versions derived from sessionInfo):
    • boot: version 1.3-32
    • caret: version 7.0-1
    • dplyr: version 1.1.4
    • ggplot2: version 4.0.1
    • ggpubr: version 0.6.2
    • ggspatial: version 1.1.10
    • gridExtra: version 2.3
    • httr: version 1.4.7
    • igraph: version 2.2.1
    • knitr: version 1.50
    • patchwork: version 1.3.2
    • randomForest: version 4.7-1.2
    • rstatix: version 0.7.3
    • scales: version 1.4.0
    • sf: version 1.0-22
    • sp: version 2.2-0
    • spatstat.explore: version 3.5-3
    • spatstat.geom: version 3.6-0
    • spatstat.random: version 3.4-2
    • TDA: version 1.9.4
    • tibble: version 3.3.0
    • tidyr: version 1.3.2

Getting Started:
----------------------------------
1. Clone or download this repository.
2. Open the main R Markdown file in RStudio.
3. Ensure that you have an active Internet connection; the code utilizes `httr` to download the shapefile components directly from the GitHub raw directory to a temporary folder.
4. Run the R script chunks sequentially to reproduce the analysis and generate all figures and tables.

Manuscript Summary:
----------------------------------
Chiefdom societies achieved regional integration through diverse organizational pathways that produced distinctive spatial signatures across prehispanic landscapes. This study compares settlement pattern trajectories in two Colombian chiefdom traditions spanning approximately 1800 years of occupation to evaluate how nucleation intensity, generative mechanisms, topological complexity, and network centralization varied independently across parallel chronological sequences. 

The Tairona tradition in the Sierra Nevada de Santa Marta concentrated populations in nucleated centers occupying defensive positions, while the Quimbaya tradition in the Middle Cauca region maintained dispersed farmstead distributions throughout comparable demographic growth. Despite these contrasting configurations, both traditions exhibited consistently low network centralization, challenging assumptions that population intensification necessarily produces hierarchical settlement structures. Machine learning classification confirmed that spatial signatures distinguish these alternative integration pathways at the individual site level. The results demonstrate that nucleation and network structure represent independent dimensions of regional organization.

For questions or further information, please contact: lms313@pitt.edu
