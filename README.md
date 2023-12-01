
<img width="840" alt="Screenshot 2023-11-30 092618" src="https://github.com/MW200410/adf_sg_project/assets/72687468/8499742b-7a54-4cb0-a5b7-d25021487ef1">

***
### Crew

<a href= "https://github.com/MW200410">MW200410</a>

<a href= "https://github.com/andyc2901">andyc2901</a>

<a href= "https://github.com/spartakill">spartakill</a>

<a href= "https://github.com/c038644">c038644</a>

<a href= "https://github.com/LaurenG123">LaurenG123</a>



# Project Brief:

The aim of this project was to develop an Extract, Transform, Load (ETL) pipeline to process publicly available data regarding past and present potential alien contacts. The goal was to structure and analyse the data for further scientific and research purposes.

# Project Summary:

## EDA:

Our group which we named Life On Mars, decided with the agreement of the project stakeholder to instead look at exoplanets and attempt to estimate the probability that life could exist on some of these planets. The team found a suitable data source at the <a href="https://exoplanetarchive.ipac.caltech.edu/docs/data.html"> NASA Exoplanet Archive </a> and setup a TAP request to extract relevant features for our study. 

<img width="600" alt="EDA" src="https://github.com/MW200410/adf_sg_project/blob/main/readme_data/Missing_Values.JPG">

### Table 1: EDA Analysis of missing values in the dataset

The dataset showed 25% missing values for two columns of interest, these were dropped leaving the dataset with still over 3700 confirmed exoplanets. We had data on the observatories that originally discovered the respective exoplanets, using feature engineering we generated the country and continent of discovery. 

## ETL Pipeline:

We decided that we wanted to use cloud services to create an automated ETL pipeline after some debate about the pros and cons of each respective provider we decided that we would use Microsoft Azure to host our pipeline. The major reason for this selection was that it would be more simple to connect the pipeline up to Power BI which we were planning on using for the dashboard component of the project.  

Via an initial TAP request the dataset was saved to cloud storage and transferred to a SQL database. An API connection was also setup to the Life On Mars GitHub repository so that pipeline insures the most recent data is available for access by all team members. 

## Dashboard Creation:

We created Power BI dashboards to visualise the data in a more intuitive way. Unfortunately due to licencing issues we were not in a position to directly embed our Power BI visualisations directly to a webpage. We were also aware of the need to create something long-lasting of our work on this project. As this stage in the project a possible closure of our Azure account would result in the loss of interactivity of the dataset. Therefore we decided to create a new independent <a href="https://c038644.github.io/Life_On_Mars/"> Life On Mars website </a> which was hosted on <a href="https://github.com/c038644/Life_On_Mars/tree/main"> GitHub </a>. 

<img width="1200" alt="EDA" src="https://github.com/MW200410/adf_sg_project/blob/main/Dashboard%20PDFs/Main.jpg">

### Table 2: Life On Mars Power BI Dashboard

<img width="1200" alt="EDA" src="https://github.com/MW200410/adf_sg_project/blob/main/Dashboard%20PDFs/FacilityMap.jpg">

### Table 3: Location of Earth based observatories that have discovered exoplanets

## Key Findings:

Several planets look to have suitable conditions to potentially harbour life: 

<img width="1200" alt="EDA" src="https://github.com/MW200410/adf_sg_project/blob/main/readme_data/Optimal_Planets.JPG">

### Table 4: Dataframe showing the most promising exoplanets for the existence of life 

The first exoplanet was discovered in only 1992 and as of 2023 there are only 5,550 confirmed discoveries. Given that the Milky Way contains 100 billion stars the number of exoplanets discovered is much less than a fraction of 1%. Despite this our basic analysis shows 9 plausible candidates for life on exoplanets. To put this another way 0.16% of the planets in our dataset could potentially support life. Calculating for the Milky Way, this gives 160 million planets that could possibly support life. Therefore, it seems highly likely that sophisticated life exists on many exoplanets. Most likely they will be asking themselves the same question we ask ourselves here on Earth: “Are we alone?” 

## Project Presentation Overview

<a href="https://testingcircle-my.sharepoint.com/:p:/r/personal/acarver_spartaglobal_com/Documents/Exoplanet%20Sparta%20Presentation.pptx?d=wee291f5d499e4813ab24aa39e06053a8&csf=1&web=1&e=RiApen"> View Powerpoint Presentation </a>

# Demo Video

<a href="https://drive.google.com/file/d/1DTb7xIacqo4IfKa3nQAUic8lP2gSiOiJ/view"> Watch Video </a>

<div><br class="Apple-interchange-newline"><iframe src="<a href="https://drive.google.com/file/d/1DTb7xIacqo4IfKa3nQAUic8lP2gSiOiJ/preview%22" title="https://drive.google.com/file/d/1dtb7xiacqo4ifka3nqauic8lp2gsioij/preview%22" target="_blank" rel="noreferrer noopener">https://drive.google.com/file/d/1DTb7xIacqo4IfKa3nQAUic8lP2gSiOiJ/preview"</a> width="640" height="480" allow="autoplay"></iframe></div>

