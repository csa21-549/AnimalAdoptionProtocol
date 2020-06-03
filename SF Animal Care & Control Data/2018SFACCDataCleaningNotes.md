# **Notes for cleaning dataset for 2018 SF Animal Care & Control Data**

- Extracted data from PDF to CSV file using Tabula.
- Separated merged columns (ACC and SF SPCA data were merged into one column during extraction).
- Removed footnote numbers.
- Removed “Total 2017” column. 
  - Note: In theory, this data would already be in the repository as a separate dataset, and if an end-user wants to compare the two datasets, they can request both and integrate. In any event, Calendar Year 2017 data should not be in this dataset, which is specific to the Calendar Year 2018 statistics.
- Combined data from “Incoming/Outgoing Transfers between ACC & SF SPCA,” “All Other Intakes/Outgoing Transfers from Organizations Within Coalition,” and “Intakes/Outgoing Transfers from Organizations Outside Coalition” as the Intake Type “Transfer” because, for the purposes of this repository, these do not need to be separated out. 
- Removed “Total Agency ______” data because this can be easily computed from the dataset, and the dataset is tidier without this redundant data. 
- The original data set combined data for animals that had either died or were lost while in the shelter. The data dictionary separated these two Outcome Type values, so in the cleaned dataset, they are listed as “Death in Facility.” This is not ideal, and is why the dataset should be submitted in compliance with the data dictionary and other protocols.
- I created a separate sheet for euthanasia data so that including the euthanasia reason would not make the other data messy. 
