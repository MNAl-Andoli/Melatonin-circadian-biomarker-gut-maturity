
# Melatonin Circadian Biomarker of Gut Maturity in Infancy

This repository contains the code and data analysis used in the paper:

**"Fecal melatonin as a biomarker of emerging circadian gut microbiota maturity in infancy"**

All analyses were performed in **R**, using **Jupyter Notebooks** with the **R kernel**. The code is organized into six thematic modules that cover different aspects of the study.

---

## 🧪 Project Overview

This study explores how fecal melatonin levels relate to gut microbiota development and circadian system maturation in infants. While melatonin is known for its role in sleep and circadian rhythms, its influence on the gut microbiome during early life remains poorly understood.

We analyzed data from infants at 3, 6, and 12 months of age to examine relationships between fecal melatonin and:

- Gut microbial diversity and richness  
- Specific bacterial taxa (ZOTUs)  
- Actimetry-based sleep-wake patterns  
- Time-dependent variables (e.g., time since last stool, sleep, and feeding)

**Key findings:**

1. Fecal melatonin increases with age, but shows high inter-individual variability  
2. Stool timing and fasting time affect melatonin levels  
3. Higher melatonin levels are associated with lower gut microbial richness  
4. The number of melatonin-associated taxa decreases with age  
5. Melatonin correlates with sleep onset latency and circadian maturity  
6. Fecal melatonin is a promising biomarker linking gut microbial and behavioral circadian rhythms

---

## 📁 Repository Structure

The repository is divided into six folders, each covering a distinct aspect of the analysis:

1. `Time based variables - Melatonin - GMB/`  
   Time-resolved analysis of melatonin and gut microbiota interactions

2. `Melatonin - OTUs - Phylum/`  
   Analysis of melatonin associations at the **phylum** taxonomic level

3. `Melatonin - OTUs - Genera/`  
   Analysis at the **genera** level of bacterial classification

4. `Melatonin - Actimetry/`  
   Associations between melatonin and infant sleep-wake patterns from actimetry

5. `Melatonin - CFI/`  
   Correlations between melatonin and **Circadian Function Index (CFI)**

6. `Melatonin - Days/`  
   Day-to-day variation in fecal melatonin levels

> 📝 To explore any folder, open a terminal, `cd` into the folder, and type:  
> `jupyter notebook`

---

## ⚙️ Environment Setup

### Step 1: Install R

Download R from [https://cran.r-project.org/](https://cran.r-project.org/)

### Step 2: Install Jupyter Notebook

Using pip or Anaconda:

```bash
# Recommended via pip:
pip install notebook
```

### Step 3: Install R Kernel for Jupyter

In an R console:

```R
install.packages("IRkernel")
IRkernel::installspec(user = FALSE)
```

This makes R available in your Jupyter Notebook interface.

---

## 📦 Required R Libraries

You can install all required packages with the following:

```R
install.packages(c(
  "tidyverse", "ggplot2", "dplyr", "lubridate", "reshape2", "gridExtra",
  "vegan", "phyloseq", "pheatmap", "scales", "nlme", "lme4", "car",
  "ggpubr", "ggthemes", "RColorBrewer", "knitr", "zoo", "readxl", "stringr"
))
```

Some libraries require Bioconductor:

```R
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("phyloseq")
```

---

## 🚀 Running the Analysis

For each of the six modules:

```bash
cd "FOLDER_NAME"
jupyter notebook
```

Then open the `.ipynb` file and run the code cells sequentially.

---

