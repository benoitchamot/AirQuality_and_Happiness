# MONU_project1
Repository for Monash University Bootcamp Project 1 (Group 1)

## Folder structure and files
This section provides a high-level description of the directories. The content of each directory is provided in the next subsections.
- The raw datasets are included in the Data_Sources directory
- The cleaned datasets are included in the Cleaned_Datasets directory
- The Jupyter notebooks used to clean the data are included in the Cleaning_Process directory
- The Jupyter notebooks used to analyse the cleaned data are included in the main directory
- The images generated from the analysis notebooks are saved in the Images directory

### Data_Sources directory
The Data_Sources directory includes the datasets gathered from various sources on the Internet. The following files and directories are included:
- AirQuality directory, including CSV files from https://waqi.info/ containing historical air quality data
- Annual Asthma Hospitalizations (per year and state in USA. 2015-2021).csv from https://ephtracking.cdc.gov/ 
- Asthma Prevalence By Country.csv from https://ourworldindata.org/grapher/asthma-prevalence 
- cleaned_life_expectancy_data.csv
- ED Visits for Asthma (per year and state in USA.(2015-2021).csv from https://ephtracking.cdc.gov/ 
- Happiness 2015.csv
- Happiness 2016.csv
- Happiness 2017.csv
- Happiness 2018.csv
- Happiness 2019.csv
- Life Expectancy By Country.xls
- Life Expectancy US data-table.csv
- transposed_life_expectancy_data.csv
- USA_County_Hospital_Admissions.csv from https://ephtracking.cdc.gov/
- USA_States_Hospital_Admissions.csv from https://ephtracking.cdc.gov/
- World Life Expectancy.csv

# Conclusions
## Air Quality & Happiness Index
- By examining the Happiness Index Rankings and relevant Air Quality data, we observe a positive correlation of moderate strength as indicated by an R-Value of 0.62. 
  As the concentration of PM2.5 particles rises (corresponding to an increase in pollution levels), we observe a downward trend in a country's Happiness Ranking. Higher pollution
  generally equates to a lower happiness ranking. 
  Although air quality does not directly dictate a country's position in the Happiness Index Ranking system, we can observe a meaningful connection of moderate significance between these
  two factors. This finding emphasises the importance of addressing air pollution as a potential contributor to overall well-being.
  
- Looking specifically at the mean PM2.5 value of top-ranked and bottom-ranked countries, we conclude a relationship beween average air quality being better for top-ranked
  countries, and lower (worse) in the bottom-ranked countries.
  Top-ranked countries mean PM2.5 value (26) falls into the 'Moderate' air quality category.
  Bottom-ranked countries mean PM2.5 value (106) falls into the 'Unhealthy' air quality category.

  It's important to note that air quality is not the sole determinant of a country's ranking or a significantly impactful factor based on this single air quality metric, but we can infer a
  relationship between air quality and the happiness index based on the analysis.

 - **Limitations**:
   It's important to consider the limitations when comparing just these two sets of data. The Happiness Ranking Index is compiled using multiple data sources, including
   GDP, Social Support, Life Expectancy, Freedom to Make life Choices, Generosity, Perceptions of Corruption, and self-reported Life Satisfaction. These are the key drivers of the
   Happiness Score and Ranking system, and it is not solely dependent on a single metric.

 - **Next Steps & Further Research**:
   To further explore the impact of air quality on a country's happiness index, it is important to consider additional variables and conduct more comprehensive analyses. Future research
   could involve examining the interactions between air quality, socioeconomic factors, and specific policy interventions to gain deeper insights into the relationship. Additionally,
   investigating the long-term effects of air quality improvements on happiness rankings and exploring regional variations could provide a more nuanced understanding of the subject.











   
