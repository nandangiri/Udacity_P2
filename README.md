# Disaster Response Pipeline Project

## Project Overview: 

With this project, I am building a machine learning model to classify the text messages during a disasterous event (Data provided by Appen) into various categories, so that the messages can be taken care of by responsible entities properly. The result of the model shall be visually presented on a web app.   

## File Description:
#### app: the folder contains the package for running the web app. It primaraly contains run.py. 
#### data: the folder contains the data input (disaster_categories.csv, disaster_messages.csv), the SQL database created (DisasterResponse.db), and the code that loads the and the process the csv input files, and created the database (process_data.py). 

#### models: the folder contains the machine learning model (train_classifier.py). The result generated (classifier.pkl) is too large for github upload, please refer to the file in workspace.

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Go to `app` directory: `cd app`

3. Run your web app: `python run.py`

4. Click the `PREVIEW` button to open the homepage
