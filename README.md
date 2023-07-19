# MONU_project1
Repository for Monash University Bootcamp Project 1 (Group 1)

## Quick Start
1. Run all the Jupyter notebooks starting with 'Cleaning_' first to generate the cleaned datasets. The files can be run in any order.
2. Run all the Jupyter notebooks starting with 'Analysis_' once the cleaned datasets have been generated. The files can be run in any order.

Note that Analysis_AirQuality_and_Hospitalisations_in_US.ipynb requires a valid API key for GeoApify. Once you have obtained your key, please follow the steps below:
1. Create a file called api_keys.py'
2. In the file, include the line: api_key_geoapify = "..."'
3. Replace ... with your geoapify API key'
4. Restart your Kernel before running the notebook.'

Please go through the dependencies in each notebook to make sure you have installed all the required modules.

## Folder structure and files
This section provides a high-level description of the directories. The content of each directory is provided in the next subsections.
- The raw datasets are included in the Data_Sources directory
- The cleaned datasets are included in the Cleaned_Datasets directory
- The Jupyter notebooks used to clean the data are included in the root directory and their names start with 'Cleaning_'
- The Jupyter notebooks used to analyse the cleaned data are included in the root directory and their names start with 'Analysis_'
- The images generated from the analysis notebooks are saved in the Images directory

### Data_Sources directory
The Data_Sources directory includes the datasets gathered from various sources on the Internet. The following files and directories are included:
- AirQuality directory, including CSV files from https://waqi.info/ containing historical air quality data
- Annual Asthma Hospitalizations (per year and state in USA. 2015-2021).csv from https://ephtracking.cdc.gov/ 
- Asthma Prevalence By Country.csv from https://ourworldindata.org/grapher/asthma-prevalence 
- cleaned_life_expectancy_data.csv
- Happiness 2015.csv
- Happiness 2016.csv
- Happiness 2017.csv
- Happiness 2018.csv
- Happiness 2019.csv
- Life Expectancy By Country.xls
- transposed_life_expectancy_data.csv
- USA_County_Hospital_Admissions.csv from https://ephtracking.cdc.gov/
- USA_States_Hospital_Admissions.csv from https://ephtracking.cdc.gov/
- World Life Expectancy.csv

### 

# Research
## Main Research Question
The overarching question this project aims at answering is: **What is the impact of air quality on quality of life?**

To approach this question, we break it down in its three main parts:
- "impact" is defined as a significant correlation between the air quality metric and different quality of life metrics (see below)
- "air quality" is defined as the concentration of Particule Matter smaller than 2.5 micrometers, an important pollutant
- "quality of life" is defined by three main metrics defined below

## PM2.5 as a Measure of Air Quality
In this research, we only focus on one type of pollutant: PM2.5. These are defined by the Government of Canada as "_particles in the air that measure less than 2.5 micrometers (μm) in diameter, and typically consists of a mix of things like smoke, soot, liquid or solid particles in aerosol, or biological matter like mould, bacteria, pollen and animal dander._"

PM2.5 come from various sources such as vehicle emissions, industry, woodworking and wood burning, gas stoves, and tobacco smoke.

PM2.5 was selected in this study as a representation of air quality for the following reasons:
- according to the UN, while PM2.5 is not as problematic as carbon-dioxide or methane when it comes to climate change, it has more direct effect on health, especially in terms of respiratory disease. It will therefore have a more immediate effect on quality of life.
- PM2.5 data were more easily available and more complete than for other pollutants. Given the quick turnaround of this project, only a couple of hours where dedicated to finding reliable data sources and the selected dataset was the most promising. Future studies could look at other pollutants such as CO or PM10.

Sources:
- https://www.canada.ca/en/health-canada/services/publications/healthy-living/infographic-fine-particulate-matter.html
- https://unece.org/unece-and-sdgs/improving-air-quality-while-fighting-climate-change

## Quality of Life, First Metric: Asthma Cases
We firstly defined quality of life in terms of physical health and in particular respiratory health as it is the most likley to be affected by poor air quality. While many respiratory diseases exist, asthma is very common across the world and several datasets could be found about it. We considered asthma prevalence (percent of people affected in a given population) as a way to measure repiratory health. We had access for worldwide data for asthma prevalence, as well as data for the United States related to hospital admissions due to asthma complications.

## Quality of Life, Second Metric: Life Expectancy
As a second metric for quality of life, we considered life expectancy as older people may be more affected by poor air quality and respiratory diseases.

## Quality of Life, Third Metric: Happiness Index
Finally, we looked at quality of life in terms of mental health, more globally represented in the Happiness Index. We assume that countries with higher quality of life will rank higher on the index.

# Conclusions
## Air Quality & Asthma Prevalence (World)
- Based on the data gathered and analysis conducted with this metric - we would gather that there is a **negative correlation** between air quality having an impact on the prevalence of asthma in countries. Meaning as air quality worsens - the asthma prevalence improves. We can conclude that there may be other varying factors and variables outside of this metric that may have affected the results. Some of which can include the varying air quality regulations in different countries, the differences in healthcare and reporting, socio-economic factors, etc. 

- If we look at Bangladesh and Nepal for example, both placing in the bottom tier of air quality, and high (better) tier for Asthma prevalence. We can interpret this data and assume that these countries' socio-economic factors, and as well as health care reporting and air quality regulations can have all have an implication on the results. Doing this analysis was very interesting, as we expected the data to demonstrate differently, as it shows to be out of line of our expectation, but given external factors, it's reported a **moderately negative correlation**.

## Air Quality & Hospitalisations caused by asthma (United States)
- We observe a positive correlation between the concentration of PM2.5 in the air and the number of hospitalisations
- This result is in line with the expectation that poorer air quality will increase astmatic reactions to a point that hospital admissions are required.
- Differences are highlighted between different states: states with larger cities (New York, California and Florida) have worse air quality (because of these cities) and higher number of hospitalisation (simply caused by the larger number of people.) Smaller states show the exact opposite results (smaller cities or more rural states have better air quality and fewer hospital admissions.) 

## Air Quality & Life Expectancy
To Be Written by Akbar

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

## Overall Conclusions
To answer the main research question related to the relationship between air quality and quality of life, we looked at three main parameters: the prevalence of asthma, the life expectancy of the population and the happiness index. The following conclusions were drawn from the data analysis:
1. Air quality and asthma prevalence do not present the expected correlation as countries with a better air quality seem to have a greater asthma prevalence number. The reason for this correlation is not covered in this project but one reason could be that more developed countries, with better air quality, may have better monitoring of asthma prevalence and the number of cases may be higher simply because of the greater fraction of the population being monitored.
2. To further understand the results related to asthma, we looked at data from the United States to understand how air pollution relates to hospitalisations related to asthma cases. We found that poorer air quality correlates with a greater number of hospitalisations. We believe that while asthma itself can be caused and affected by other factors than air quality, the poorer air quality seems to go hand in hand with a higher number of crtical cases needing hospitalisation.
3. We found that better air quality correlates with longer life expectancy.
4. Likewise, we concluded that lower pollution correlates with a higher level of happiness. In general, the happiest countries presents significantly better air quality compared to the countries at the other end of the happiness scale.

Overall, across all the parameters considered in this study, we conclude that air quality and quality of life go hand in hand. We are however cautious not to claim any causality between the two as both of these aspects are complex and many other parameters are undoubtedly at play. We leave the reader with a few ideas to consider next to this research and that could be used as the basis of future work:
- Happiness levels are driven by lower crime rates, higher gender equality, more respect of human rights, better healthcare, etc. Countries tackling these aspects effectively are likely to also better regulate their impact on the environment and therefore pollution. The link between air quality and happiness is then probably hidden within a much more complex politico-economic system than the simplified study we performed within this short-duration project.
- While we can more easily imply that better air quality improves physical (and probably mental) health and therefore life expectancy, the problem is here as well more complex and would necessitate more investigation on how very different countries manage healthcare and regulate the release of many different polluant (not only PM2.5) into the atmosphere.
- Looking at a single country, like the US, allows to eliminate some of the country-to-country variations and the study of the hospitalisation numbers per US state still revealed an important correlation with air quality. However, there are still differences between the different US states and looking at more metrics could allow to refine the study even more. Looking at daily data (higher time frequency) for a single city (smaller area) over a year could help control more of the variables. At the time of writing, this data was unfortunately not easily available. 











   
