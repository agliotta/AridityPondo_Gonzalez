# AridityPondo_Gonzalez

Journal: Ecology

Title: Increased aridity is associated with stronger tradeoffs in ponderosa pine vital functions

Authors: Angela D. Gonzalez, Ian S. Pearse, Miranda D. Redmond

Year: 2023

----------------------------------------------------------------------------------------------------------

#### Description of the data and file structure #####

List of files in Gonzalez et al., 2023:

Files used for Analysis:

annual_data.csv - annual climate and ponderosa pine data. This data set also includes some site specific information that is not annual. Details below.

  site- site ID
	year - year corresponding to measurement
	tree - tree ID
	growth12 - radial annual xylem growth (mm) measurements taken for 12mm diameter core
	conematur - annual cone abundance at year of maturation
	resinarea2 - annual relative duct area (% annual ring)   
	totalresin - annual total resin area(mm2 year-1)
	meanductsize - annual mean duct size (mm2)
	wuecentered - 21 year individual average of Delta 13C stable carbon isotopes. 13C values were centered to the site mean and represent deviations of an individual tree from the average 13C of a site. 
	cwd - mean 30-year cumulative climatic water deficit at each site. 
	FDSI - annual Forest Drought Severity Index calculated using early vapor pressure deficit and prior year precipitation


averages_data.csv - average climate and ponderosa pine data used for among individual models
	tree - tree ID
	site - site ID
	growth12 - 21-year average radial annual xylem growth (mm) measurements taken for 12mm diameter core
	conematur - 21-year average annual cone abundance at year of maturation
	resinarea2 - 21-year average annual relative duct area (% annual ring) 
	BA5 - local neighborhood tree density around focal tree measured as ft2/acre
	dbh - individual tree diameter measured at breast height (cm)
	wuecentered - 21 year individual average of Delta 13C stable carbon isotopes. 13C values were centered to the site mean and represent deviations of an individual tree from the average 13C of a site. 
	cwd - mean 30-year cumulative climatic water deficit at each site.

Gonzalez_2022.Rmd - file containing R markdown script to run model diagnostics and analysis of the above manuscript. This RMD file is annotated for the ease of the user. 


Raw Data: 
The unprocessed raw data gathered prior to data analysis.

carbonisotopes.csv - file containing stable carbon isotope data given after processing from UC Davis's stable isotope facility. It is recommended to see UC Davis carbon isotope facility for details prior to use of this data: https://stableisotopefacility.ucdavis.edu/ 

	SampleID - the site ID, Tree ID, and year (in that order). All samples have 20 denoted as the year in which the sample was taken.  
	d13CVPD - 21-year average of the raw carbon discrimination value 
	TotalC - 21-year total carbon for each sample

ringwidths_5mm.csv - data of annual xylem ring widths (5 mm core). Ring width values were verified using chronologies. Cores were dated to latest year of certainty.
	Year - annual xylem ring width
	Subsequent columns are ring width values identified by site ID and tree ID of tree (site_tree)

ringwidths_12mm.csv - data of annual xylem ring widths (12 mm core). Ring width values were verified using chronologies and the computer program COFECHA. See manuscript Appendix S1 for details. Cores were dated from 2020-2000, or latest date of certainty.
	Year - annual xylem ring width
	Subsequent columns are ring width values identified by site ID and tree ID of tree (site_tree)

master_ducts.csv - 
	site- site ID
	tree - tree ID	
	Year - year corresponding to measurement
	Area - resin duct area (mm2) of each vertical oleoresin duct found in the assigned year. Measurements were taken between 2000-2020. See Appendix S1 for details. 

master_lengths.csv - 
	site- site ID
	tree - tree ID	
	Year - year corresponding to measurement
	Length - the length of each annual xylem ring (mm)
	Scar - the area (mm2) of scarring found in each annual xylem ring
