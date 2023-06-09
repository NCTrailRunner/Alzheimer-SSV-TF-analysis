# Alzheimer-SSV-TF-analysis
Data sets and codes for analysis of short structural variant impact on transcription factor binding sites in Alzheimer's Disease Genome-wide Association loci


These files contain the computer code and data used to generate the Tables and Results for the paper: Lutz MW, Chiba-Falek O. Bioinformatics pipeline to guide post-GWAS studies in Alzheimer's: A new catalogue of disease candidate short structural variants. Alzheimers Dement. 2023 May 30. doi: 10.1002/alz.13168. Epub ahead of print. PMID: 37253165.

The file "region mapping for Table of epigenetic evidence" contains VBA macro code to map from genomic regions to specific candidate cis-regulatory elements.  The decision to use visual basic for applications was based on the availability of tabular data from the UCSC Table Browser.  These data were imported into EXCEL and the overlap calculations performed using the VBA code.  For calculations for <100 regions, this code is a simple approach to implement.  For larger, genome-scale calculations, R-based code would be a possible choice using the VBA code as examples and using R table data structures instead of the worksheets.  The worksheet regions contains a list of the genomic regions, the worksheet ccre conditains a list of the candidate cis regulatory elements.  The worksheet output contains the mapping.  

Example computer code for running MotifbreakR is contained in the file Example motifbreakR script.docx, which includes detailed comments on the code and input/output tables.

All data loaded from the UCSC Genome browser (GRCh38/hg38) was current as of 6/2022.

Several output datasets are included as excel files for downstream analysis:

All loci for analysis.txt contains a listing of all of the input AD GWAS loci for analysis by the pipeline

All cCRE.txt contains a list of all cis candidate response elements for further analysis

Epigenetic evidence (Supplemental S1) contains Epigenetic evidence for each candidate cis-regulatory element (cCRE).  Tissues: hippocampus, temporal lobe and mid frontal

Summary of sigle cell data analysis (Supplemental S2) contains the analysis of single cell RNA-seq data for differential gene expression for genes and transcription factors in study.

MotifbreakR analysis for all loci (Supplemental S3)  contains the MotifbreakR analysis for all LOAD GWAS loci.
