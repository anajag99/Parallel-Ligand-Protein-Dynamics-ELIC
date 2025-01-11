# Parallelized Protein Dynamics Analysis of ELIC

## Overview
This repository focuses on the parallelized computational analysis of ligand-protein dynamics in the pentameric ligand-gated ion channel ELIC (Erythrina variegata lectin). By using bioinformatics tools, molecular dynamics simulations, and parallel processing techniques, this project demonstrates significant improvements in speed and efficiency for ligand extraction and protein structure analysis.

## Key Features
- **Sequential vs Parallel Execution**: Comparison of sequential and parallel execution for ligand-protein analysis, achieving a speedup of 6.95x.
- **Bioinformatics Tools**: Utilization of Python libraries such as Biopython and pandas for ligand extraction, binding site identification, and protein structure modification.
- **Molecular Dynamics**: Integration of molecular dynamics simulations for detailed analysis of ligand-protein interactions.
- **Parallel Processing**: Implementation of OpenMP and Python multiprocessing for concurrent task execution.

## Methodology
1. **Dataset Integration**:  
   - X-ray structures of ELIC in complex with memantine and bromoform were used.
   - Data processing and integration were performed using Python and pandas.

2. **Ligand Extraction**:  
   - Ligands were identified as non-protein residues and extracted using Biopython's PDBParser.  
   - Each ligand was saved as a distinct PDB file for further analysis.

3. **Protein Structure Modification**:  
   - Protein structures were processed to exclude ligands, focusing solely on the protein framework.

4. **Binding Site Analysis**:  
   - Binding sites were identified by analyzing amino acid residues such as ARG and LYS.  
   - Residue IDs and details were extracted for further insights.

5. **Parallelization**:  
   - Parallel processing was implemented to reduce computational time significantly, demonstrating the effectiveness of concurrent operations.

## Results
- **Sequential Execution Time**: 1.5317 seconds  
- **Parallel Execution Time**: 0.2204 seconds  
- **Speedup**: 6.95x  
- **Efficiency**: 3.47 (optimized resource utilization)

These results highlight the transformative potential of parallel computing in structural bioinformatics, enabling faster and more efficient protein-ligand analyses.

## Technologies Used
- **Programming Language**: Python  
- **Libraries**: Biopython, pandas, multiprocessing  
- **Parallelization Techniques**: OpenMP, Python multiprocessing  
- **Tools**: Molecular dynamics simulation software, X-ray crystallography data
