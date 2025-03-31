# call_known_mutations_from_RNAseq
Some snippet of code to call mutations in single cells. The mutations are NOT called di novo, you need to have previously defined the variants in a VCF file. In the case of cancer, a good starting point is the COSMIC database https://cancer.sanger.ac.uk/cosmic

The scripts here will:   
1) Format SmartSeq2 scRNAseq bam files to fit the 10x format: need to add CB tag
2) Index the formatted bams
3) Run VarTrix to call mutations given a predefined VCF file

 
