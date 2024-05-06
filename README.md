This README file was generated on 02.05.24 by Celina Alexandria Kostich-Nilsen. 
Under construction! Last edited: 06.05.24

--------------------
GENERAL INFORMATION
--------------------
// Title of Datasets: Final_OTU_table_Celina_no_unidentified.xlsx
                      Phenolics EcoForest Celina.xlsx 
                      Variables_Celina 
// Contact Information 
	// Name: Celina Alexandria Kostich-Nilsen 
	// Email: celinaak@student.ibv.uio.no 
// Kind of data: Curated OTU table, environmental, physical, chemical 

%%
-------------------------------------------------------------
INFORMATION FOR: Final_OTU_table_Celina_no_unidentified.xlsx
-------------------------------------------------------------
// Description of dataset: 
Raw curated OTU table from DNA sequences obtained from Norway spruce needles. 
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

%%
--------------------------------------------------
INFORMATION FOR: Phenolics EcoForest Celina.xlsx 
--------------------------------------------------
Description of dataset: Plant chemical analysis of spruce needle samples. 
3 sheets:
- Sheet 1: Low molecular weight phenolics
- Sheet 2: MeOH soluble condensed tannins
- Sheet 3: MeOH insoluble condensed tannins
 
-----------------------------
METHODOLOGICAL INFORMATION
-----------------------------
Low molecular weight phenolic concentrations acquired from high performance liquid chromatography. 
Condensed tannins concentrations acquired from acid butanol assay for proanthocyanidins. 
These chemical analyses were conducted by Line Nybakken at Norwegian University of Life Sciences. 

-----------------------------
DATA SPECIFIC INFORMATION
-----------------------------
// Column List: 

// Sheet 1 - Low molecular weight phenolics 
Column 1: concentration values given (mg g-1) and sample ID numbers 
gallocatechin: concentrations of gallocatechin 
B3: concentration of B3 
(+) catechin: concentration of (+) catechin 
piceatannol glucoside: concentration of piceatannol glucoside
resveratrol: concentration of reseratrol 
Piceatannol aglycon: concentration of Piceatannol aglycon
Isorhapontin: concentration of Isorhapontin
quercetin3glucuronide: concentration of quercetin3glucuronide
quercetin3glucoside: concentration of quercetin3glucoside
kaempferol3glucuronide: concentration of kaempferol3glucuronide 
apigenin7glucoside: concnetration of apigenin7glucoside '
flavonoid: concentration of flavonoid 
Kaempferol3glucoside: concentration of Kaempferol3glucoside 
isorhamnetin: concentrations of isorhamnetin 
Sum, flavonoids: concentration sum of all flavonoids in sample (flavonoids represented by yellow color in header) 
Sum, stilbenes: concentration sum of all stilbenes in sample (stilbenes represented by blue color) 
flavonols = quercetins + kaempferols: sum of concentrations of flavonols 
flavan-3-ols = gallocatechin + B3 + (+) catechin: sum of concentrations of flavan-3-ols 
flavanones: sum of concentrations of flavanones 

// Sheet 2 - MeOH soluble condensed tannins 
Sample ID: sample ID of spruce needles samples  
Concentration mg g-1_ concentration of MeOH soluble condensed tannins 

// Sheet 3 - MeOH insoluble condensed tannins 
Sample ID: sample ID of spruce needle samples 
Concentrations, mg g-1: concentration of MeOH insoluble condensed tannins 

%% 
-----------------------------









