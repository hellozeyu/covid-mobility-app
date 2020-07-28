### Introduction
- This analysis is based on the [COVID-19 Community Mobility Reports](https://www.google.com/covid19/mobility/index.html?hl=en) created by Google. The reports aim to provide insights into what has changed in response to policies aimed at combating COVID-19. The reports chart movement trends over time by geography, across different categories of places such as retail and recreation, groceries and pharmacies, parks, transit stations, workplaces, and residential.
- In order to run the analysis, make sure you download the [original dataset](https://www.google.com/covid19/mobility/index.html?hl=en) from Google and run all the code chunks in the `data_cleaning.ipynb` to create the cleaned dataframe that only focuses on the trend in the U.S
- I also combined it with the [COVID-19 dataset](https://github.com/nytimes/covid-19-data) from New York Times, trying to find how people from different states are responding to the number of confirmed cases and deaths.
- The analysis can be found in the `data_analysis.ipynb` notebook. I also built a [Plotly Dash]([Dash](https://plot.ly/dash) App on top it.


### Project structure
    ├── app.py                  # where Dash instance is defined
    ├── index.py                # the entry point for running the app
    ├── layouts.py              # define the layout of each url/page
    ├── callbacks.py            # define how we handle the input/output
    ├── requirements.txt        # install project dependecies in a virtual environment
    ├── assets/                 # static files
    └── ...

### How to run the APP
**Step 1:**
You can either use the virtual env that used to build this app
 - On macOS and Linux:
 `source env/bin/activate`
 - On Windows:
`.\env\Scripts\activate`

or you can install all the dependencies manually by running `pip install -r requirements.txt` 

**Step 2:**
Start the Dash App by running `python index.py`

**Step 3:**
Check the app locally at `http://127.0.0.1:8050/`