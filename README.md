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
