# CUH_2019_SMT
This repository contains the Jupyter Notebook and other input files relevant to the following paper:

## Pre-requisites
- Machine: Ubuntu 18.04. 48 core, 500GB Memory, +1TB Space
- Software & Plugins
  - [QIIME 2](https://qiime2.org/) installed under the Conda environment
  - [PICRUSt2](https://github.com/picrust/picrust2) installed under the separate Conda environment
- 16s rRNA sequences
  - 16s rRNA sequences were submitted to the NCBI BioProject [PRJNA814893](http://www.ncbi.nlm.nih.gov/bioproject/814893)

## Workflow
1. Please install the QIIME 2 under your conda environment and locate the ``main_analysis.ipynb``, ``metadata.txt``, and ``manifest.txt`` files. 
2. Follow the scripts as described in the ``main_analysis.ipynb``.
3. Some of the PICRUSt2 features are not yet available as a q2-picrust2 plugin. picrust2_pipeline.py was used with the following commands as described in the ``main_analysis.ipynb``.

        picrust2_pipeline.py -s dna-sequences.fasta -i feature-table.biom -o picrust2_out_pipeline -p 12
