![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Project-Active-brightgreen)

# Metagenomic Profiling of Antibiotic Resistance Genes

This project explores antibiotic resistance genes (ARGs) in human gut microbiomes using publicly available shotgun metagenomic sequencing data. It applies tools like **Kraken2**, **Bracken**, and **DeepARG** for resistome and taxonomic profiling.

---

## 📑 Table of Contents

- [Objectives](#objectives)
- [Directory Structure](#directory-structure)
- [Tools Used](#tools-used)
- [Usage](#usage)
- [Results](#results)
- [How to Cite](#how-to-cite)
- [License](#license)

---

## 🎯 Objectives

- Taxonomic profiling of human gut microbiota
- Annotation of antibiotic resistance genes
- Visualization of ARG class distribution and species composition

---

## 🗂️ Directory Structure

├── data/

│├── raw/    
│└── processed/   

├── notebooks/

│  ├── 01_qc_trimming.ipynb
│  ├── 02_taxonomy.ipynb
│   ├── 03_ARG_annotation.ipynb
│   └── 04_visualization.ipynb

├── env/

│   └── environment.yml

├── results/

│   └── figures/

├── run_pipeline.py

├── README.md

└── LICENSE


---

## 🛠️ Tools Used

- `fastp`, `sra-tools`, `Kraken2`, `Bracken`, `DeepARG`
- `Bowtie2` for alignment
- `Python`, `JupyterLab`, `Seaborn`, `Matplotlib`

---

## 🚀 Usage

```bash
# Create conda environment
conda env create -f env/environment.yml
conda activate metagenomics-arg

# Run the pipeline
python run_pipeline.py
```

## 📊 Results
Output files include:

Taxonomic composition per sample

ARG annotations with class and identity

Visual plots in results/figures/


## 📖 How to Cite

If you use this pipeline in your work, please cite:
Subhadip Jana (2025).
Metagenomic Profiling of Antibiotic Resistance Genes.
GitHub Repository: https://github.com/SubhadipJana1409/metagenomics-arg


## 🪪 License

This project is licensed under the MIT License. See LICENSE for details.

Copyright (c) 2025 Subhadip Jana

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
"""
