
<img width="840" alt="Screenshot 2023-11-30 092618" src="https://github.com/MW200410/adf_sg_project/assets/72687468/8499742b-7a54-4cb0-a5b7-d25021487ef1">

***
### Crew

MW200410

andyc2901

spartakill

c038644

LaurenG123

# Project Brief:

The aim of this project was to develop an Extract, Transform, Load (ETL) pipeline to process publicly available data regarding past and present potential alien contacts. The goal was to structure and analyse the data for further scientific and research purposes.

# Project Summary:

### EDA:

Our group which we named Life On Mars, decided with the agreement of the project stakeholder to instead look at exoplanets and attempt to estimate the probability that life could exist on some of these planets. The team found a suitable data source at the <a href="https://exoplanetarchive.ipac.caltech.edu/docs/data.html"> NASA Exoplanet Archive </a> and setup a TAP request to extract relevant features for our study. 

<img width="840" alt="EDA" src="https://github.com/MW200410/adf_sg_project/blob/main/readme_data/Missing_Values.JPG">

The dataset showed 25% missing values for two columns of interest, these were dropped leaving the dataset with still over 3700 confirmed exoplanets. We had data on the observatories that originally discovered the respective exoplanets, using feature engineering we generated the country and continent of discovery. 

### ETL Pipeline:

We decided that we wanted to use cloud services to create an automated ETL pipeline after some debate about the pros and cons of each respective provider we decided that we would use Microsoft Azure to host our pipeline. The major reason for this selection was that it would be more simple to connect the pipeline up to Power BI which we were planning on using for the dashboard component of the project.  

Via an initial TAP request the dataset was saved to cloud storage and transferred to a SQL database. An API connection was also setup to the Life On Mars GitHub repository so that pipeline insures the most recent data is available for access by all team members. 

### Dashboard Creation:

We created Power BI dashboards to visualise the data in a more intuitive way. Unfortunately due to licencing issues we were not in a position to directly embed our Power BI visualisations directly to a webpage. We were also aware of the need to create something long-lasting of our work on this project. As this stage in the project a possible closure of our Azure account would result in the loss of interactivity of the dataset. Therefore we decided to create a new independent <a href="https://c038644.github.io/Life_On_Mars/"> Life On Mars website </a> which was hosted on <a href="https://github.com/c038644/Life_On_Mars/tree/main"> GitHub </a>. 
