# Reef_fish-
Spatial and temporal trends of reef fish 

The purpose of this project is to examine changes in reef fish distribution through time, and to determine what environmental factors are driving their distributions.  This project is part of my master's thesis.  Data is from the Southeast Reef fish survey (SERFS) data base.  
All data is located in the data folder.  The following files are in this folder: 
  1. Raw Chevron Trap Data.csv- This is the raw data file that I started all of the analyses with.  
  2. RawChevron.csv - Data file I created after selecting the columns I needed from the original raw data file. 
  3. RawBSB.csv- raw black sea bass file I created by selecting only the variables of interest and creating a presence absence column. 
  4. NewBSB.csv- limiting data to 2011-2015 and running na.exclude
  5. RawWG.csv and NewWG.csv same as black sea bass but for white grunt
  6. SpatialBSB.csv- adding habitat data to black sea bass data file
  7. SpatialWG.csv- adding habitat data to white grunt data file
  8. Video Data- used to create habitat data for my data

The scripts folder contains the working scripts for my project.  
  1.  SpatialDataExploration.rmd - This is the first markdown associated with the project.  This markdown contains a lot of subsetting and data selection.  I am creating new data files and subsetting data frames to be used later one.  Also, I am using code created by Joseph Ballenger to create habitat data for my data that is currently lacking habitat data. 
  2.  SpatialModeling.rmd - This markdown contains automated model selection for black sea bass and white grunt.  Best models are then chosen based on BIC values (and AIC).  Visreg is then used to visualize the effects of individual variables on presence/absence. 
  3.  SLOO bsb.rmd - This markdown contains a test run to see if there was spatial dependence at the trap level.  Since there wasn't we went forward with traditional cross validation instead of spatial cross validation.
  4.  CrossValidation.rmd- This markdown completes kfold cross validation for the best models for white grunt and black sea bass. 

