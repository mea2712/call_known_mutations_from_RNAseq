# call_known_mutations_from_RNAseq
Some snippet of code to call mutations in single cells. The mutations are NOT called di novo, you need to have previously defined the variants in a VCF file. In the case of cancer, a good starting point is the COSMIC database https://cancer.sanger.ac.uk/cosmic

The scripts here will:   
1) Format SmartSeq2 scRNAseq bam files to fit the 10x format: need to add CB tag - Uses JVARKIT
2) Index the formatted bams
3) Run VarTrix to call mutations given a predefined VCF file

The scripts are written to run in a HPC with SLURM.  
You execute 07.0_bamsCB.sh from the command line. This will call and execute 07.0_bamsCB.run. When all bams are formatted, you execute 08.0_vartrix.sh that will call and execute 08.0_vartrix.run to identified known somatic mutations    



 
