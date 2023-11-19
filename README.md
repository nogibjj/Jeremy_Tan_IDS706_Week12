[![CI](https://github.com/nogibjj/Jeremy_Tan_IDS706_Week12/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/Jeremy_Tan_IDS706_Week12/actions/workflows/cicd.yml)

## Jeremy Tan IDS706 Week12
### File Structure
```
Jeremy_Tan_IDS706_Week12/
├── .devcontainer/
│   ├── devcontainer.json
│   └── Dockerfile
├── .github/
│   └── workflows/cicd.yml
├── .gitignore
├── MLFLOW ARTIFCATS
├── data/
│   ├── serve_times.csv
│   └── event_times.csv
├── Dockerfile
├── LICENSE
├── main.py
├── Makefile
├── README.md
├── requirements.txt
├── setup.sh
└── test_main.py
```

## Purpose of Project
Tennis Server Prediction using MLflow

1. Objective:
    Build a machine learning model to predict the server in a tennis match based on the seconds before the next point. Utilize MLflow for experiment tracking and model management.

2. Data:
    The dataset contains information about tennis matches, including the server, seconds before the next point, day, opponent, game score, set, and game.

3. Steps:

    1. Data Loading and Preprocessing:
    2. Load the dataset into a Pandas DataFrame.
    3. Extract relevant features (e.g., 'seconds_before_next_point', 'server').
    4. Model Training:
        -Split the data into training and testing sets.
        -Train the model on the training set.
    5. MLflow Integration:
        1. Use MLflow to log parameters, metrics, and the trained model.
        2. Log parameters such as the model type and data path.
        3. Log metrics like accuracy.

### Preparation: 
1. git clone the repo
2. install: `make install`
3. run: `python main.py`
4. run: `mlflow ui` to view mlflow interface 
5. view saved model and other artifacts in `mlruns/0`

### Check Format and Test Errors: 
1. Format code `make format`
2. Lint code `make lint`
3. Test coce `make test`

