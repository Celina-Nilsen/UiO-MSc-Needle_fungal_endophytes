This README file was generated on 02.05.24 by Celina Alexandria Kostich-Nilsen. 
Under construction! Last edited: 02.05.24

--------------------
GENERAL INFORMATION
--------------------
// Title of Datasets: Final_OTU_table_Celina_no_unidentified.xlsx
                      Phenolics EcoForest Celina.xlsx 
                      Variables_Celina 
// Contact Information 
	// Name: Celina Alexandria Kostich-Nilsen 
	// Email: celinaaak@student.ibv.uio.no 
// Kind of data: Curated OTU table, environmental, physical, chemical 

// Description of dataset: 
Raw curated OTU table from DNA sequences obtained from Norway spruce needles. 

-------------------------------------------------------------
INFORMATION FOR: Final_OTU_table_Celina_no_unidentified.xlsx
-------------------------------------------------------------
---------------------------
METHODOLOGICAL INFORMATION 
---------------------------
Description for generation of data: 

DNA extraction performed on 50 needles per sample, PCR amplified and library prepared. 
Libraries were sent to Fasteris (Switzerland) for ITS2 region to be sequenced on Illumina MiSeq. 
Returned sequences were analayzed using 
CUTADAPT - demultiplex sequences, minimum 26 bp overlap, minimum length of 100 bp 
DADA2 - denoised and dereplicated sequences, two errors allowed in each direction and 
10 bp trimmed off tail end of sequences, ASV table constructed and chimeric sequences removed
ITSx - extract only ITS2 region 
SWARM - clustered ASVs to OTUs
mumu - final clustered OTU table, corrected oversplitting 
SINTAX - taxonomic annotation, sequences in database with "unidentified" in header were removed

---------------------------
DATA-SPECIFIC INFORMATION 
---------------------------

// Column List: 

amplicon: unique amplicon name 
S001-S192: sample name 
sequence: DNA sequence 
length: basepair length 
Phylum: taxonomic annotation of phylum from SINTAX  
Class: taxonomic annotation of class from SINTAX 
Order: taxonomic annotation of order from SINTAX 
Family: taxonomic annotation of family from SINTAX 
Genus: taxonomic annotation of genus from SINTAX 
Species: taxonomic annotation of species from SINTAX 
Kingdom_support: bootstrap support value of kingdom rank from SINTAX 
Phylum_support: bootstrap support value of phylum rank from SINTAX 
Class_support: bootstrap support value of class rank from SINTAX  
Order_support: bootstrap support value of order rank from SINTAX
Family_support: bootstrap support value of family rank from SINTAX
Genus_support: bootstrap support value of genus rank from SINTAX
Species_support: bootstrap support value of species rank from SINTAX
Strand: 
Tax_above_threshold: all classes taxonomy was able to be given to 
