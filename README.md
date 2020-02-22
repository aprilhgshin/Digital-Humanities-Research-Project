# Air-Pollution-Research-Project

### Introduction:
I have been highly interested in the changes in the environment and its impacts on life as well as how the human population contributed to the change. For this project, I decided to do a study on air quality, as it has been a prevalent issue since the beginning of rise of the industry. 

### Research Focus:
- What is the relationship between the human population and Ozone levels in California counties?
    - Does human population density have an effect on ozone levels? (Given that human activity - driving vehicles, for instance - directly contribute to higher ozone levels on the ground level - EPA)
    - Is there an association between asthma and ozone levels?
    
### Data Sources
Geographical regions of the following data cover each county in California, United States:
- Population Density: 2010 US Census. Additional data derived from Open Data Network
- Number of days when ozone levels are above regulatory standards: California Environmental Protection Agency, Air Resource Board: (iADAM) Air Quality Data Statistics
- Average Particulate Matter Concentration: California Environmental Protection Agency, Air Resource Board: (iADAM) Air Quality Data Statistics
- Number of Emergency Room visits due to Asthma: California’s Office of Statewide Health Planning and Development (OSHPD)¶

### Methods
- Process datasets.
    - Import and read csv, xls, xlsx files. Webscrape. Apply pandas methods to process (filter, merge, transpose, sort, etc.) all imported data and create visualizations. Organize into appropriate data structures.
    - Standardize all data.
- Apply A/B testing to test for association. Test for linear relationship.
    - Traditional steps for A/B testing followed: 
        - Create Null/Alternative Hypotheses 
        - Set Test Statistic (used absolute difference between means of the absolute value of standardized data)
        - Set Observed Test Statistic
        - Create 1000 simulations by creating samples through shuffling with replacement from original dataset and computing test statistic
        - Compute p-value 
        - Using p-value, determine if null hypothesis is supported or rejected (setting 1% as the cut-off)
    - Linear Relationship:
        - Calculate Correlation Coefficient
