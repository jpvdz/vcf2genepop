# vcf2genepop
Convert bi-allelic SNPs stored in VCF format to GENEPOP format. Requires a VCF file with bi-allelic SNPs and a population map, which is a CSV file containing sample IDs (first column) and population labels (second column). The columns need to be named `sample_id` and `population`.   

## Dependencies
Requires the `scikit-allel`, `numpy` and `pandas` packages. 

## How to run
The following example reads in a VCF file called `example.vcf` and a population map `example_popmap.csv`, converts the VCF into a GENEPOP file called `example.genepop`:

`./vcf2genepop.py example.vcf example_popmap.csv example.genepop`