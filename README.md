# DSA210 - Term Project Proposal

## Introduction

I have chosen to work on publicly available datasets. They are available on kaggle:

- E-commerce Data
  <https://www.kaggle.com/datasets/carrie1/ecommerce-data/code>

- World Development Indicators
  <https://www.kaggle.com/datasets/theworldbank/world-development-indicators/code>

## Motivation

I was reading about customer behaviours in the modern world in my daily life. Also I know e-commerce is one of most popular locations for custormers today. That is why I have decided to analyze the _E-commerce Data_ dataset. I use the country and product information from this dataset additionally, I use the _World Development Indicators_ dataset to join buying trends with certain economic and societal factors in countries to understand why marketing trends are specifically unique in some certain countries. I am hoping to find insights that are uncommon and has not been paid enough attention.

## Reproducing the Experiment

To reproduce the customer value prediction experiment, follow the steps below:

### Data

The experiment uses two publicly available datasets:

1.  **E-commerce Data**: UK Online Retail dataset from Kaggle (Dec 2010–Dec 2011). This dataset contains transactional data.

    - Download from: [E-commerce Data](https://www.kaggle.com/datasets/carrie1/ecommerce-data/code)
    - Place the `data.csv` file inside a `datasets/` directory in the root of your project.

2.  **World Development Indicators (WDI)**: This dataset provides various macroeconomic indicators.
    - Download from: [World Development Indicators](https://www.kaggle.com/datasets/theworldbank/world-development-indicators/code)
    - Extract the contents of `wdi-csv-zip-57-mb-.zip` and place the `WDIData.csv` file inside the `datasets/` directory.

our project structure should look like this:

.
├── main.ipynb
└── datasets/
├── data.csv
└── WDIData.csv

### Setup

1.  **Clone the repository (if applicable)**: If this project is hosted in a Git repository, clone it to your local machine.
2.  **Create a virtual environment (recommended)**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install dependencies**: The experiment relies on the following Python libraries.
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```

### Running the Notebook

1.  **Start Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```
2.  **Open `main.ipynb`**: In your browser, navigate to the Jupyter interface and open the `main.ipynb` file.
3.  **Run all cells**: Execute all cells in the notebook sequentially to perform data loading, preprocessing, model training, evaluation, and feature importance analysis.

The notebook will output the RMSE and R² metrics for the trained model, as well as the feature importances, demonstrating the model's performance and the key drivers of customer value.
