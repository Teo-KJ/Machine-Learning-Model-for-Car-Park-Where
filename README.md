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

### Data Extraction
Next, data is extracted with Python notebook using the *urllib* module. After the extraction, we use the *pandas* module to process into a structured data frame. More details are elaborated in the notebooks below.

### Cleaning and Pre-processing
After obtaining the data, it has to go through cleaning to remove unnecessary columns. In addition, we obtain some features from the original data. Laslty, attributes in string data type are encoded so that they can be accepted into the model for training.

### Training with Decision Tree Regressor
When the data is prepared, it is trained with Scikit-learn (sklearn) Decision Tree Regressor to generate the numerical output which is the predicted carpark lots. When the model is generated, it is saved for future prediction of the carpark availability.

## About Car Park Where
This is an app that provides live carpark availability in Singapore, and also makes prediction of carpark availability so that users can make informed decisions on parking options.
The output of the carpark lot prediction is made from the machine learning model trained with the scripts in this directory. You may refer to this [link](https://github.com/Teo-KJ/Car-Park-Where) for more details of Car Park Where.

## About the notebooks and data

### Data
The data was intially generated from the URL of our servers. However, as the data gets accumulated daily, the size increases until it becomes very large. Hence, data was downloaded from the website manually. The following are generated data.
* **usedCarparks.csv** stores data of the carparks that are used in the prediction and analysis.
* **hdb-carpark-information.csv** is a CSV file taken from the Data.gov.sg which stores details of carparks managed by the HDB.
* **carparkDetails.json** is a JSON file taken from the URA website which stores details of carparks managed by the URA.

### Load Model
This notebook is a template to load the trained machine learning model that was saved previously, and then use to make predictions.

### Prediction of Carpark Availability (Data from API)
This notebook draws the data from API URLs, and then process the data into a structured data frame. However, as the data accumulates day by day, this notebook was no longer continued to train the final model.

### Prediction of Carpark Availability (Data from Directory)
As the data gets increasingly large, we use this notebook to read the data from the local directory as the files are downloaded from the URL. In addition, we train the final models in this notebook. The final models are also splitted into 30 parts based on carpark number as one single model is very large in size. 

### Visualisation of Carpark Availability and Carpark Details
This notebook is an attempt to visualise the carpark details data taken from both HDB and URA. In addition, we visualised the average carpark availability for selected carparks based on a single week and on a single day. This objective of visualisation is to show how it can be visualised when implemented in the *Car Park Where* app.

DT_model.sav
