# Customer Lifetime Value Prediction with PyMC-Marketing

## Project Overview
This project implements advanced Customer Lifetime Value (CLV) prediction using Bayesian statistical models via the PyMC-Marketing library. It focuses on "Buy Till You Die" (BTYD) modeling approaches, particularly the BG/NBD and Gamma-Gamma models, to evaluate and predict the future value of customers based on their transaction history.

## Features
- **Data Preparation**: Processes transaction data to be model-ready.
- **BG/NBD Model**: Estimates the probability that a customer is still "alive" and their purchasing frequency.
- **Gamma-Gamma Model**: Predicts the monetary value of customer transactions.
- **CLV Calculation**: Integrates both models to calculate the expected lifetime value of customers.

## Methodology

1. **Data Preparation**: This initial phase involves gathering and cleaning transactional data, ensuring it includes customer IDs, transaction dates, and transaction values. Any anomalies, such as returns or missing data, are addressed in this stage.

2. **Model Implementation**:
   - **BG/NBD Model**: This model is applied to predict how frequently a customer will make purchases and whether they are still active (i.e., not churned). It uses a probabilistic framework to model purchase frequency based on historical data.
   - **Gamma-Gamma Model**: Used for predicting the monetary value of transactions for each customer. It assumes that the monetary value of a customer's transactions varies randomly around their average transaction value, which is estimated from the data.

3. **Integration and CLV Calculation**: The outputs of the BG/NBD and Gamma-Gamma models are combined to estimate the CLV. This involves calculating the expected number of transactions and the expected average transaction value to derive the total expected revenue from a customer over their lifetime.

4. **Analysis and Actionable Insights**: The final step involves analyzing the CLV outputs to identify high-value customers and understand customer behavior. This analysis supports strategic decisions in marketing, such as resource allocation and personalized marketing campaigns.

Each step is supported by Python code and Jupyter notebooks that facilitate data manipulation, model fitting, and result visualization.

## Installation
To set up the project environment:
```bash
git clone https://github.com/drshaheed/CLV-Prediction.git
cd CLV-Prediction
pip install -r requirements.txt
```

## Usage
Run the Jupyter notebooks in the `notebooks` directory to go through the modeling process:
```bash
jupyter notebook
```
- **01_data_preparation.ipynb** - Data cleaning and preparation.
- **02_model_building.ipynb** - Building and training the models.
- **03_results_analysis.ipynb** - Analyzing and visualizing the results.

## Contributing
Contributions to enhance the model or improve the methodology are welcome. Please fork the repository, make your changes, and submit a pull request for review.

## License
This project is licensed under the MIT License - see [LICENSE](LICENSE) for details.

## Contact
Shaheed Shahul Hameed
- Email: drshaheedofficial@gmail.com
- LinkedIn: [drshaheed](https://linkedin.com/in/drshaheed)
- GitHub: [drshaheed](https://github.com/drshaheed)

## Acknowledgements
- [PyMC-Marketing Library](https://github.com/pymc-labs/pymc-marketing)
- Data sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail)
