# :computer:  Appathon project for the course "Internet and Applications" 

# Requirements
pip install mysql.connector
For manipulation of the XML file we used a python script. This script also creates a database and inserts the data in it, hence the library needed above.

# Project Description
CTGOV-03: Countries in which Clinical Studies have taken place for a particular disease

# :book: Contents
Our aim is to create a web application that will present all the countries in which clinical studies for a particular disease have taken place. The name of the disease will be defined by the user through the web page or a suitable endpoint (e.g. localhost:8080/appathon_project/index.html?search={Disease_Name}&format={map or json}) and output will be the countries sorted according to the number of clinical studies that have taken place which will be presented either as json or with markers on a map.

For the needs of this application we downloaded all available clinical trials (XML files) from the https://clinicaltrials.gov/ to filter the clinical trials based on the disease and then identify the countries. We will add these studies to a database after proper processing in order to keep the following fields: official_title, brief_title, acronym, nct_id, country. In order to parsing the data, a suitable python script was created.

# 🧰 Tools
  - Eclipse IDE
  - MySQL,
  - html , css , javascript 
  - Java servlet , for database communication and post request service
  - google maps api
  - google geocoding (api to convert country name to coordinates to be placed as markers on the map)

# Formats
2 formats are supported:
  - json format
   [
     { "country_name": "...",
        "cnt" : ...,
        "lat" : ...,
        "lng" : ...
      }
      ...,
      {"status" : 200 ή "Zero_Results"}
   ]
  - Data with markers on a map

# :pencil: Authors
The author of this project is: Roussis Dimitrios

# :book: Documentation
The presentation powerpoint can be found in Greek in the [Documentation folder](https://github.com/jirou97/Appathon_project/tree/master/documentation)

An example using the markers format can be seen in the following image.
![image](https://user-images.githubusercontent.com/83036199/133442648-63feee4f-d0df-47e4-86e9-bb320f84f155.png)
