# Football Match Predictor Using Poisson Distribution

## Introduction
This project is a football match predictor that utilises the Poisson distribution to estimate the outcomes of matches based on historical data. The main goal is to provide a statistical approach to predict the number of goals each team might score in a matchup, thereby determining possible match outcomes (win, loss, draw).

## Features
- **Data Analysis**: Perform exploratory data analysis on historical match data.
- **Poisson Model**: Utilise the Poisson distribution to predict the outcome of football matches based on the average number of goals scored by each team in previous encounters.
- **Simulation**: Simulate match scores multiple times to predict the most probable outcome.
- **Visualisation**: Generate various visualisations to display predicted results and statistical insights.

## Libraries Used
- Pandas for data manipulation
- Matplotlib and Seaborn for data visualisation
- SciPy for statistical functions

## Project Structure
```
PoissonMatchPredictor/
│
├── PoissonMatchPredictor.ipynb    # Main Jupyter notebook containing all the analyses and predictions
├── historical_data.csv            # Historical match data 
└── README.md                      # Project overview and setup instructions
```

## Setup and Installation
To get this project up and running on your local machine, follow these steps:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Amar0302/FootballMatchPredictionPoisson
   cd FootballMatchPredictionPoisson
   ```

2. **Install Required Python Packages**
   ```bash
   pip install pandas matplotlib seaborn scipy
   ```

3. **Run the Jupyter Notebook**
   - Ensure you have Jupyter installed. If not, you can install it using `pip install jupyter`.
   - Launch Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Open the `PoissonMatchPredictor.ipynb` notebook and run the cells.

## Usage
To use this project to predict the outcome of a football match:

1. Update the `historical_data.csv` with the latest match data.
2. Run the Jupyter notebook from start to finish to perform data analysis, prediction, and visualisation.

## Methodology
The core of the prediction model is based on the Poisson distribution, a discrete probability distribution that expresses the probability of a given number of events happening in a fixed interval of time or space if these events happen with a known constant mean rate and independently of the time since the last event.

### Predictive Model
- **Data Preparation**: Extract historical goal data and calculate average goals per match.
- **Poisson Distribution**: Use `scipy.stats.poisson` to model and simulate the scoring of each team.
- **Simulation**: Simulate multiple match outcomes to find the most probable result.

## Contributing
Feel free to fork this repository and submit pull requests to contribute to improvements, new features, or bug fixes.

## Licence
This project is licensed under the MIT Licence - see the [LICENCE.md](LICENCE.md) file for details.

## Acknowledgements
- Thanks to https://www.football-data.co.uk/ for providing the data set.
