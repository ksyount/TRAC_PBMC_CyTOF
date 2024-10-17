# TRAC_PBMC_CyTOF

Data and code from the research article entitled "Unique T cell signatures associated with reduced Chlamydia trachomatis reinfection in a highly exposed cohort"

Data files referenced here can be accessed at ImmPort.org at accession \#SDY2772

#### 1. tSNE & automated gating (Figure 3A-B,D-E)

Download the following data files from ImmPort:

-   post_combat_gated_CD4.csv (downsampled and batch-corrected CyTOF expression data, manually gated on CD4+ T cells for further analysis)

-   post_combat_gated_CD8.csv (downsampled and batch-corrected CyTOF expression data, manually gated on CD8+ T cells for further analysis)

Code used to perform automated gating by k-means clustering:

-   PBMC_CYTOF_AutomatedGating.ipynb 

#### 2. Feature engineering and random forest training matrix generation

Download the following data files from ImmPort:

-   Classifiers.xlsx (PTIDs and Visits with Infection, Ascension, and Follow-Up observation outcomes defined)

-   Freqs.csv (Manually gated frequencies exported from FlowJo workspace)

-   Upperqs.csv (Upper quartile expression of each marker of interest among each manually gated T cell subset exported from FlowJo workspace)

Code used to generate upper quartile features and create matrices for random forest model training:

-   RandomForestMatrixPrep.Rmd

#### 3. Random forest model & Gini feature importance analysis (Fig 4A,H; Fig 6A,B; Fig S2E,F; Table S6-8)

Matrices were generated previously (see above).

Code used to run random forest models and Gini feature importance analysis:

-   RandomForest_GiniAnalysis.Rmd

#### 4. Upper quartile expression plots (Fig 4B-G,I-M; Fig 6C-F)

Download the following data files from ImmPort:

-   allupperqdata.csv

-   expressiondata.csv

Code used to generate figures:

-   UpperQuartileExpressionPlots.Rmd
