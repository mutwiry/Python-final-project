# Python-final-project

# COVID-19 Global Data Tracker

This project involves the analysis of the "Our World in Data" COVID-19 dataset to track and visualize global trends in cases, deaths, and vaccinations. The primary focus is on a comparative analysis of Kenya, the United States, and India, culminating in key insights derived from the data. The analysis is performed using Python within a Jupyter Notebook environment.

## Objectives

The main objectives of this project are:

1.  **Data Loading & Exploration:** Load the dataset and perform initial checks (shape, data types, missing values).
2.  **Data Cleaning:** Handle missing data, convert data types, and filter the dataset for relevant countries and columns.
3.  **Exploratory Data Analysis (EDA):**
    *   Visualize total cases and total deaths over time for selected countries.
    *   Compare new daily cases across these countries.
    *   Calculate and plot the death rate (total deaths / total cases).
4.  **Vaccination Analysis:**
    *   Plot cumulative vaccinations over time.
    *   Visualize the percentage of the population vaccinated per country.
5.  **Derive Insights:** Summarize key findings and observations from the analysis.


## Tools and Libraries Used

*   **Python 3.x**
*   **Jupyter Notebook** (as part of Anaconda distribution)
*   **Pandas:** For data manipulation and analysis.
*   **Matplotlib:** For creating static, animated, and interactive visualizations.
*   **Seaborn:** For making statistical graphics more attractive and informative.


## Data Source

The dataset used is `owid-covid-data.csv` from [Our World in Data](https://github.com/owid/covid-19-data/tree/master/public/data).
Please download the latest version of this file and place it in the root directory of the project for the notebook to run correctly.

## How to Run/View the Project

### Prerequisites

*   [Anaconda](https://www.anaconda.com/products/distribution) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html) installed. This will provide Python, Jupyter Notebook, and manage packages.
*   The dataset `owid-covid-data.csv` in the project's root directory.

### Setup and Execution

1.  **Clone the repository (or download the files):**
    ```bash
    git clone <>
    cd <>
    ```

2.  **Create and activate a Conda environment (recommended):**
    ```bash
    conda create -n covid_tracker python=3.9 pandas matplotlib seaborn plotly -y
    conda activate covid_tracker
    ```
    If you prefer not to create an environment, ensure the necessary libraries are installed in your base environment:
    ```bash
    pip install pandas matplotlib seaborn plotly jupyterlab
    ```

3.  **Place the dataset:**
    Ensure `owid-covid-data.csv` is in the same directory as the `.ipynb` notebook file.

4.  **Launch Jupyter Notebook or JupyterLab:**
    ```bash
    jupyter notebook
    ```
    or
    ```bash
    jupyter lab
    ```
    This will open a new tab in your web browser.

5.  **Open and run the notebook:**
    Navigate to and open the `COVID-19_Global_Data_Tracker.ipynb` (or whatever you named your notebook file). You can then run the cells sequentially to execute the code and see the outputs.

### Viewing on GitHub

The Jupyter Notebook (`.ipynb` file) can also be viewed directly on GitHub. GitHub renders the notebook, including the code, markdown explanations, and static versions of the plots.

## Insights and Reflections

Based on the analysis of COVID-19 data for Kenya, the United States, and India:

1.  **Varying Scale of Impact:** The absolute number of cases and deaths significantly differed across the three nations, with the US and India experiencing much larger outbreaks compared to Kenya, partly attributable to population size and other epidemiological factors.
2.  **Distinct Wave Patterns:** Each country showcased unique pandemic wave patterns, influenced by variants, public health interventions, and societal behavior. For example, India's Delta wave in mid-2021 was particularly severe.
3.  **Vaccination Disparities:** Vaccination rollout and coverage varied considerably. The US initiated its campaign earlier and achieved higher per capita vaccination rates more quickly than India and Kenya. India, despite a later start, managed a massive scale-up. Kenya's progress reflected challenges common in lower-income countries regarding vaccine access and distribution.
4.  **Dynamic Death Rates:** The death rate (total deaths / total cases) was not static, fluctuating over time due to factors like testing capacity (more testing can lower the apparent death rate by identifying milder cases), healthcare system strain, emergence of new variants, and improved treatments.
5.  **Data Completeness and Quality:** The analysis underscored the importance of data quality. Missing values and the need for data smoothing (e.g., 7-day rolling averages for new cases) are common challenges in real-world epidemiological datasets, highlighting the need for robust data collection and reporting.

**Reflections:**
This project serves as a practical application of data analysis techniques to a real-world global health crisis. The Our World in Data dataset is an invaluable resource, though its comprehensiveness also brings challenges in terms of data cleaning and interpretation. Visualizations proved crucial in understanding complex trends and making comparisons across countries. Further analysis could delve into correlations with policy measures, demographic factors, or economic impacts.

---

*This README provides a guide to understanding, running, and interpreting the "COVID-19 Global Data Tracker" project.*
