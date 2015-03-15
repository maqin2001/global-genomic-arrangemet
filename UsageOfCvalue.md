#Global Genomic Arrangement of Bacterial Genes is Closely Tied with the Total Transcriptional Efficiency

# Usage #
This software is used to calculate the Global Genomic Constrain function (C value) of bacterial genome in this paper:Genomic arrangement of bacterial operons is constrained by biological pathways encoded in the genome (PMID: 20308592).

# Installation #
Simply put "GlobalGenomicConstrain1.0.tar.gz" in any directory,
  * $ tar zxvf GlobalGenomicConstrain1.0.tar.gz
enter the folder "GlobalGenomicConstrain1.0" and type "make" then the compiled codes are within the same directory as the source.

# Inputs and outputs #
The major program in the provided package is `*Cvalue*`. See help and look at all available options.
  * $ ./Cvalue -h
To run an example:
  * $ ./Cvalue -j DATA/NC\_000913.ptt  -o DATA/NC\_000913.gi.operon -p DATA/pathway.example
To run with the known genomic partitions (supercoils):
  * $ ./Cvalue -j DATA/NC\_000913.ptt  -o DATA/NC\_000913.gi.operon -p DATA/pathway.example -s DATA/supercoils.fast
To run with the whole genome expression data, which can indicate the ultilization frequency of each pathway
  * $ ./Cvalue -i DATA/ecoli\_466\_4297 -j DATA/NC\_000913.ptt -o DATA/NC\_000913.gi.operon -p DATA/pathway.example


# Contact #
Any questions, problems, bugs are welcome and should be dumped to
Qin Ma <maqin2001@gmail.com>

Creation: April 3rd, 2012