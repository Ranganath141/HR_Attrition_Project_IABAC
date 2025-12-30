## PROJECT DIRECTORY STRUCTURE


├── Project Summary <- The top-level summary of the Project
│ ├── Requirement <- Data from third party sources.
│ ├── Analysis <- Interpreting Data and summary of various choices from selecting ML algorithm to data processing techniques
│ ├── Summary <- Project Summary with Analysis and recommendation.
├── data
│ ├── external <- Data from third party sources.
│ ├── processed <- The final, canonical data sets for modeling.
│ └── raw <- The original, immutable data dump.
│
├── src <- Source code for use in this project.
│ ├── Data Processing <- Data processing, data mugging, exploratory Analysis
│ │ ├── data_processing.ipynb
│ │ ├── data_exploratory_analysis.ipynb
│ ├── models <- Scripts to train models and predictions
│ │ ├── train_model.ipynb
│ │ └── predict_model.ipynb
│ └── visualization <- Scripts to create exploratory and results visualizations
│ └── visualize.ipynb
└── references <- Data dictionaries, manuals, and all explanatory materials.
