# Machine-Learning-Model-for-Car-Park-Where
This repository serves the machine learning portion for the app *Car Park Where*.
There are 4 Python Notebooks in this directory namely:
- Load Model
- Prediction of Carpark Availability (Data from API)
- Prediction of Carpark Availability (Data from Directory)
- Visualisation of Carpark Availability and Carpark Details

These notebooks highlight the processes taken by the *Car Park Where* team with regards to the machine learning aspects.
### Data Collection
Firstly, we obtain the live data from the Data.gov.sg and URA websites, thereafter collect the data on a daily basis. The live data is collected at intervals of seconds. The data is then stored in our server accessible by a URL.

## Data Extraction
Next, data is extracted with Python notebook using the *urllib* module. After the extraction, we use the pandas module to process into a structured data frame. More details are elaborated in the notebooks below.

## Cleaning and Pre-processing


## About Car Park Where
This is an app that provides live carpark availability in Singapore, and also makes prediction of carpark availability so that users can make informed decisions on parking options.
The output of the carpark lot prediction is made from the machine learning model trained with the scripts in this directory. You may refer to this link for more details of Car Park Where.

## Machine Learning 

## Load Model
This notebook is a template to load the trained machine learning model that was saved previously, and then use to make predictions.

## Prediction of Carpark Availability (Data from API)
This notebook draws the data from API URLs, and then process the data into a structured data frame. However, as the data accumulates day by day, 

## Prediction of Carpark Availability (Data from Directory)

## Visualisation of Carpark Availability and Carpark Details

usedCarparks.csv
DT_model.sav
allCarparksData.csv
hdb-carpark-information.csv
carparkDetails.json