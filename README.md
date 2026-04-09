# DPSCA
De novo Plant Single-Cell Annotator (DPSCA) is a workflow designed for genome-reference-independent cell-type annotation in non-model plants scRNA analysis. It is fully integrated and ready to run natively on PantheonOS (https://doi.org/10.64898/2026.02.26.707870).

# How to use
1. Install the PantheonOS (https://pantheonos.stanford.edu/) and setup LLM API;
2. Download "DPSCA.tar" file, copy to your path of PantheonOS-0.4.8/.pantheon/skills/omics/ and unzip it;
3. Download and copy Ref_data.gz and unzip it at your workdir
4. Copy the content of SKILL_Guide.md to your path of PantheonOS-0.4.8/.pantheon/skills/omics/SKILL.md;
5. Use natural language to inform PantheonOS that you want to process single-cell analysis for plants, providing the data type and location, as well as the analysis you want to perform.

# Example Conversational Prompt

"PantheonOS, please execute a plant single-cell transcriptome analysis task for me. The specific details are as follows:

1. Subject: Arabidopsis (or replace with rice, maize, etc.) single-cell data.
2. Data Type: Gene expression matrix in .h5ad format (or replace with FASTQ, .mtx, etc.).
3. Data Location: Cloud storage path /bio-data/plant_scRNA/.


# Attention
1. A transcript function profile (e.g., NR,Swissport,GO,KEGG) must be provided when leveraging LLMs for automated cell-type identification.
2. Providing step-by-step prompts might yield better results when executing the analysis. 
3. The choice of large language model may affect the results.
