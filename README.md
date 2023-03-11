# police-killings

# fatal_encounters_renamed_cols.csv underwent the following limited cleaning in R (code below):
fatal_encounters_clean <- 

  fatal_encounters %>% 
  
  select(
  
    # select columns to keep and rename
    
    c(`unique_id` = `Unique ID`,
    
      `age` = `Age`,
      
      `gender` = `Gender`,
      
      `race` = `Race`,
      `race_w_imputations` = `Race with imputations`,
      `imputation_probability` = `Imputation probability`,
      `date` = `Date of injury resulting in death (month/day/year)`,
      `city` = `Location of death (city)`,
      `state` = `State`,
      `zip` = `Location of death (zip code)`,
      `county` = `Location of death (county)`,
      `latitude` = `Latitude`,
      `longitude` = `Longitude`,
      `agencies` = `Agency or agencies involved`,
      `highest_force` = `Highest level of force`,
      `armed` = `Armed/Unarmed`,
      `weapon` = `Alleged weapon`,
      `aggressive` = `Aggressive physical movement`,
      `fleeing` = `Fleeing/Not fleeing`,
      `dispositions_exclusions` = `Dispositions/Exclusions INTERNAL USE, NOT FOR ANALYSIS`,
      `intended_use_of_force` = `Intended use of force (Developing)`,
      `mental_illness` = `Foreknowledge of mental illness? INTERNAL USE, NOT FOR ANALYSIS`
       )
    )

The original columns were:

 [1] "Unique ID"                                                      
 [2] "Name"                                                           
 [3] "Age"                                                            
 [4] "Gender"                                                         
 [5] "Race"                                                           
 [6] "Race with imputations"                                          
 [7] "Imputation probability"                                         
 [8] "URL of image (PLS NO HOTLINKS)"                                 
 [9] "Date of injury resulting in death (month/day/year)"             
[10] "Location of injury (address)"                                   
[11] "Location of death (city)"                                       
[12] "State"                                                          
[13] "Location of death (zip code)"                                   
[14] "Location of death (county)"                                     
[15] "Full Address"                                                   
[16] "Latitude"                                                       
[17] "Longitude"                                                      
[18] "Agency or agencies involved"                                    
[19] "Highest level of force"                                         
[20] "UID Temporary"                                                  
[21] "Name Temporary"                                                 
[22] "Armed/Unarmed"                                                  
[23] "Alleged weapon"                                                 
[24] "Aggressive physical movement"                                   
[25] "Fleeing/Not fleeing"                                            
[26] "Description Temp"                                               
[27] "URL Temp"                                                       
[28] "Brief description"                                              
[29] "Dispositions/Exclusions INTERNAL USE, NOT FOR ANALYSIS"         
[30] "Intended use of force (Developing)"                             
[31] "Supporting document link"                                       
[32] "Foreknowledge of mental illness? INTERNAL USE, NOT FOR ANALYSIS"
[33] "V33"                                                            
[34] "V34"                                                            
[35] "Unique ID formula"                                              
[36] "Unique identifier (redundant)"                                  
