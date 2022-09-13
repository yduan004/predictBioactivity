# Bioactivity Prediction


# Run on Heroku
The web service is alive on Heroku at . 

# Reproducing this web app
To recreate this web application on your own computer, clone this repository to your local computer by running
```sh
git clone https://github.com/yduan004/predictBioactivity.git
cd predictBioactivity
```

### Create virtual environment
Firstly, we will create and activate a virtual environment named *env*
```sh
virtualenv env --python=python3.10
source env/bin/activate 
```
### Install prerequisite libraries

```sh
pip install -r requirements.txt
```

### Generating the PKL file

The machine learning model used in this web app is stored as `cdk_model.pkl`. You could generate your own model on other target proteins of interest by running the included Jupyter notebook [bioactivity_prediction_app.ipynb](https://github.com/yduan004/predictBioactivity/blob/main/bioactivity_prediction_app.ipynb). Upon successfully running all code cells, a customized pickled model will be generated. 

###  Launch the app

```
streamlit run app.py
```
