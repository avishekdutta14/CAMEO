# CAMEO
A tool for control subtraction and data-mining in the field of microbial ecology

##Steps for using CAMEO

1) Download Python 3.3.3 from https://www.python.org/downloads/ and install it on your windows OS (Win 7 and above)

2) Download CAMEO from https://github.com/avishekdutta14/CAMEO.

3) Decompress CAMEO.zip

4) Place your file in offiline folder present in CAMEO

5) Input files will contain *example input files are provided in the example_input folder*

  (i)	Output from pick_otus.py  i.e. filename_otus.txt

  (ii)	Output from pick_rep_set.py i.e. filename_rep_set.fna

  (iii)	Output from assign_taxonomy.py i.e. filename_tax_assignments.txt

  (iv)	Index file present in the CAMEO package containing the exact name of the outputs of pick_otus.py, assigned_taxonomy.py, pick_rep_set.py should be present in row starting   with OTU, TAXA and FASTA parameters respectively. Sample ID of the contaminant sample or samples should be mentioned under CONTROL and separated by comma. Sample ID of the       samples to compare should be mentioned in COMPARE row and number of rarefaction steps should be mentioned in RARESTP row.

 **N.B.: First three input files should be compressed into zip format.**

6) Once everything is done click on the backend_processor.py to initiate the analysis

7) The script will take time as per the input and number of samples.

8) Once the script has finished processing, the output will be in a compressed folder named download_zip.zip

10) The folder download_zip.zip will have the results

## Description of the output files

(i)	OTU table in CSV format containing read details, taxonomic affiliation, GC percentage and abundance of each reads in different samples (File name :otu_table.csv). If control Sample ID is provided in the index, OTU table generated will not contain the OTUs harboring contaminated reads.

(ii)	Read abundance and taxonomic distribution at different levels (File name starts with D_).

(iii)	Unique OTUs are present in unique_otu_table.csv

(iv)	Rarefaction data is present in rarefaction_data.csv which might be plotted in any graph plotting software to generate rarefaction curve.

(v)	Krona chart on the basis of diversity of different samples can be observed in common_OTU.html

(vi)	Krona chart on the basis of unique diversity of different samples can be observed in single_OTU.html

N.B.: Krona chart generated in the form of HTML file can be viewed through any web-browser supporting HTML file.


For any CAMEO related query contact 

avishekdutta14@gmail.com
