This README file was generated on 02.05.24 by Celina Alexandria Kostich-Nilsen. 
Under construction! Last edited: 06.05.24

--------------------
GENERAL INFORMATION
--------------------
// Title of Datasets: Final_OTU_table_Celina_no_unidentified.xlsx
                      Phenolics EcoForest Celina.xlsx 
                      Variables_CAKN 
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
--------------------------------------
INFORMATION FOR: Variables_CAKN.xlsx 
--------------------------------------
// Description of dataset: Environmental variables at plot level and needle associated variables. 
Environmental variables collected during needle collection or acquired from other datasets (Horvath et al., 2019; Asplund et al., 2024). Plots are 15 m x 15 m pairs, two plots per location/site. 

----------------------------
DATA SPECIFIC INFORMATION 
----------------------------
// Sheet 1 - Forest level 

Plot ID: Plot abbreviation and forestry type combined 
Location: Location of plot 
Site_ID: Abbreviation of location 
Forest_type: Type of forestry of plot (NN = near natural, CC = previously clear cut) 
Coordinates X0Y0 Lat: Latitude coordinates of plot 
Coordinates X0Y0 Lon: Longitude coordinates of plot 

Basal_area m2 ha-1: Basal area of living and dead trees in plot, measured as m2 ha-1 
Number of trees (living and dead): Number of living and dead trees in each plot 
Tree species (Diversity (shannon index): Tree species diversity measured using Shannon index diversity measure 
Connectivity: Connectivity of living spruce volume within a 25 km radius from the EcoForest plots. Connectivity was calculated using SR16 (Norway) and kNN 2010 (Sweden) data from 16 x 16 m and 25 x 25 m pixels, respectively. For Norwegian data, connectivity was calculated as the sum of: [living tree volume (with bark) from spruce-dominated pixels] * exp (- [distance from plot to pixel] * alpha). For Swedish data, connectivity was calculated the same except tree volume which was [living spruce volume (with bark) from all pixels].  Connectivity was calculated for forests with a stand age  80 years. Seven alpha values were used [0.05, 0.1, 0.2, 1, 1.34, 2, 4] corresponding to mean dispersal distances of 20, 10, 5, 1, 0.75, 0.5 and 0.25 km, respectively. This dataset using the alpha value 2 (0.5km). Collected and calculated by Lisa Fagerli Lunde. 
Crown length: Mean relative crown length. Height of lowest green branch subtracted from total height, expressed relative to total height. Collected by NORSKOG, calculated by Johan Asplund. 
Vegetation cover (vascular): Determined visually in 1 m x 1 m pllots, the average value of 6 subplots in each plot. Calculated by Damina Karlsen. 
Plant diversity (vascular; shannon divversity index): Shannon diversity index of vascular plants at each plot. Calulated by Damina Karlsen.
Mean temp warmest quarter: Modelled mean temperature of warmest quarter, 100 m x 100 m resolution. (Horvath et al., 2019)
Mean precipitation warmest quarter: Modelled mean precipitation, with 100 m x 100 m resolution. (Horvath et al., 2019)
Diffuse light index (average): The data was generated using hemispherical photos taken over the centre of each sub-plot. iPhone SE 2nd generation using the application Street View (Google LLC). DLI_yearly    Diffuse light index (DLI): average transmission of diffuse (indirect) radiation. Unit: W/m^2. Period: 1st of January to 31st of December. SAR = slope aspect Nov 2023. Collected and calculated by Rieke Lo Madsen. 
Insolation: Modeled data of Potential Incoming Solar Radiation; Geodatat - GEM; Saga; Potential incoming solar radiation (Horvath et al., 2019). 


// Sheet 2 - Needle data 

Location: Location of plots 
Site_ID: Abbreviation of location 
Forest_type: Type of forestry of plot (NN = near natural, CC = previously clear cut) 
Tree_ID: Sample number of tree that needles were collected from 
BioInfo_Sample: Sample number given during metabarcoding and bioinformatics 
Tree_number: number of tree collected from plot, numbers 1-8 possible. Eight trees sampled at each plot. 
Tree Diameter (BHD) in cm: Tree diameter of the tree the needles were collected from, taken at breast height (approx. 1.3 m), diameter recorded in centimeters. 
Date collected: the date the needles were collected 
Avrg needle length: the vaerage needle length of randomly sampled needles from the tree, between 47-53 needles. 
Needle weight after drying (g): total weight of randomly collected needles (47-53) from each tree after being freezedried for 72 hours, given in grams. 
% Nitrogen: percent nitrogen from aliqouted amount from pulverized needles. Measured with flash elemental analyzer. 
% Carbon: percent carbon from aliqouted amount from pulverized needles. Measured with flash elemental analyzer. 



--------------
REFERENCES 
--------------
Asplund, J., Nordén, J., Kjønaas, O. J., Madsen, R. L., Lunde, L. F., Birkemoe, T., Ronold, E. K., Norkute, Milda., Jansson, K. U., Karlsen, D., Sverdrup-Thygeson, A., Skrede, I., Methlie., I. S. H., Maurice, S., Kauserud, H., & Nybakken, L. (2024). Long term effects of forest management on forest structure and dead wood in mature boreal forests. [Preprint] https://doi.org/10.2139/ssrn.4772055 

Horvath, P., Halvorsen, R., Stordal, F., Tallksen, L. M., Tang, H., Bryn, A., Feilhauer, H. (2019). Distribution modelling of vegetation types based on area frame survey data. Vegetation Science 22(4), 547-560. http://doi.org/10.1111/avsc.12451 





















