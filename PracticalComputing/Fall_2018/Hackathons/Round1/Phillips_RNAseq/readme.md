# RNA-Seq Resistome profiling of Acinetobacter baumannii
- For this project, you will:
    - organize RNA data.
    - discover transcipts responsible for antibiotic resistances in Acinetobacter baumannii. 

## Recomended modules 
Matplotlib 
Pandas
Numpy

### Input Files
1. "khead\_table.csv" is a comma-separated file containing transcript nomenclature(target\_id), sample names of the bioreplicates (sample), normalized read counts for each transcript (est\_count), tpm, eff\_len, len, strain profile information (resistance_profile), and treatment.

2. "s\_table.csv" is a csv file containing the output of a statistical analysis comparing levels of transcript expression from different isolates/conditions. Columns of interest include: the name of the differentially expressed transcript (target_id), the p-value (pval) and the adjusted p-vaule (qval) . 

3. There is also one "abundance.tsv" file for each bioreplicate organized within a set of directories starting with the 'indiv\_replicates' directory and including one subdirectory for each bioreplicate. These tab-delimited files contain the raw output from kallisto (an RNA-seq analysis algorithm). Info from these files were combined to form "khead\table.csv".


### Expected Output

Your aim is to read in the data from "khead\_table.csv" and "s\_table.csv", and generate a new tab-delimited output file containing a subset of the columns from these two input files, as well as a few new columns with summary statistics. final table containing columns, meanEstCount, sigma, pval, qval, and Difference. Some columns will simply be replicated into a truncated easier to read file. Other columns will require calculation and data structuring.  

2. Calculate mean(est_count) over triplicates from Khead_table for each transcript and add to Output.csv.

3. Calculate standard deviatation(est_count) over triplicates from khead_table for each transcript and add to Output.csv.

4. Extract P-value and Q-value from s_table and add to Output.csv.

5. Write Output.csv

6. Generate boxplot of the transcript with the biggest difference in abundance. 

	Alternatively, collect and calculate from raw data in form of abundance.tsv files (1 per bioreplicate).



