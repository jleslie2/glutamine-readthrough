# glutamine-readthrough

**CYC8_RRTS_and_RPtraces.ipynb**, **SNF5_RRTS_and_RPtraces.ipynb** and **ade1Y244X_RRTS_and_RPtraces.ipynb**:
Code for normalizing CYC8, SNF5 and ADE1 ribosome profiling A-site corrected ribosome profiling densities to their respective RPKMs. Gene specific .bed files were created by extracting A-site corrected ribosome density coordinates by transcript ID from A-site corrected .wig files (canonical stop codon coordinates were excluded). For SNF5 and CYC8, frame distribution was calculated before and after the stop codon by taking the proportion of reads within each frame. To calculate RRTS for each transcript, ribosome density reads were summed, adjusted to transcript length and converted to reads per kilobase (RPK), then RPK signal after the premature stop codon was divided by RPK signal before and including the premature stop codon. These analyses correspond to data presented in Figure 4B-F, as well as Supplementary Figure 4G-I.

**Metageneplot.ipynb**:
Code for calculating genome-wide ribosome profiling densities from .bigwig files for 50 nucleotides before and 50 nucleotides after the stop. This analysis corresponds to Figure 6A.

**SortingAndScoringCTerminalAAEndings.ipynb**:
Code for filtering the yeast proteome for glutamine ending proteins (single, double and triple Qs) and all C-terminal yeast proteins that end in duplicate amino acids ('ZZ ending proteins'). For all ZZ ending proteins, this code extracts sequence information +/-9 nucleotides of the stop codon and assigns a stop strength score based on yeast ribosome profiling data in https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1009538. This analysis corresponds to data presented in Figures 6E-G.



