# TRAC_PBMC_CyTOF

Data and code from the research article entitled "Unique T cell signatures associated with reduced Chlamydia trachomatis reinfection in a highly exposed cohort"

FCS and CSV data files referenced here can be accessed at ImmPort.org at accession \# \_\_\_\_

#### 1. tSNE & automated gating

Code used to perform automated gating by k-means clustering (Figure S3A-B,D-E):

-   "Automated gating & tSNE visualization" section in PBMC_CYTOF_RandomForest_Frequency.ipynb 

#### 2. Feature engineering and random forest training matrix generation

##### For manually gated frequency features and upper quartile expression features:

Download the following data files from ImmPort:

-   Classifiers.xlsx (PTIDs and Visits with Infection, Ascension, and Follow-Up observation outcomes defined)

-   Freqs.csv (Manually gated frequencies exported from FlowJo workspace)

-   Upperqs.csv (Upper quartile expression of each marker of interest among each manually gated T cell subset exported from FlowJo workspace)

Code used to generate upper quartile features and create matrices for random forest model training:

-   RandomForestMatrixPrep.Rmd

##### For automated gating frequency features:

-   "Frequency Features engineering" section in PBMC_CYTOF_RandomForest_Frequency.ipynb 

#### 3. Random forest model & Gini feature importance analysis

##### For manually gated frequency features and upper quartile expression features (Fig 3A,H; Fig 4E,F; Fig 6A,B; Fig S2):

Matrices were generated previously (see above).

Code used to run random forest models and Gini feature importance analysis:

-   RandomForest_GiniAnalysis.Rmd

##### For manually gated frequency features and upper quartile expression features (Fig S3G-H, Fig S4A-B):

-   "Random forest training & Gini feature importance analysis" section in PBMC_CYTOF_RandomForest_Frequency.ipynb 

#### 4. Upper quartile expression plots

Download the following data files from ImmPort:

-   allupperqdata.csv

-   expressiondata.csv

Code used to generate Figure 3B-G,I-M and Figure 6C-F:

-   UpperQuartileExpressionPlots.Rmd
