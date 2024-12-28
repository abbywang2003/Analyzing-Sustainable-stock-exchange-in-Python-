# Analyzing-Sustainable-stock-exchange-in-Python-

## Project Overview
This project analyzes the Shanghai Stock Exchange (SSE) Composite Index data to assess financial risk through Value at Risk (VaR) and Expected Shortfall (ES) calculations. The analysis employs Bayesian inference, statistical validation, and correlation analysis using Python.

## Key Features
- Log returns calculation and distribution analysis
- Bayesian inference implementation using Gibbs sampling
- Distribution validation through autocorrelation analysis
- VaR and ES calculations with correlation analysis
- Advanced visualization of financial risk metrics

## Prerequisites
- Python 3.8+
- Required Python packages:
  ```
  numpy
  pandas
  matplotlib
  scipy
  seaborn
  ```

## Installation
1. Clone this repository:
   ```bash
   git clone [your-repository-url]
   cd sse-analysis
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the SSE dataset:
   - Visit: [SSE Dataset on Kaggle](https://www.kaggle.com/datasets/jmselina/sse-shanghai-stock-exchange)
   - Download and place the CSV file in the project directory

## Project Structure
```
sse-analysis/
├── data/
│   └── sse_data.csv
├── notebooks/
│   └── sse_analysis.ipynb
├── requirements.txt
└── README.md
```

## Usage
1. Open the Jupyter notebook:
   ```bash
   jupyter notebook notebooks/sse_analysis.ipynb
   ```

2. Follow the step-by-step analysis:
   - Data preparation and log returns calculation
   - Gibbs sampling implementation
   - Distribution validation
   - VaR and ES analysis
   - Correlation visualization

## Methodology

### 1. Distribution Setup
- Uses the last 1000 records of closing prices
- Calculates logarithmic returns
- Implements Bayesian inference using Gibbs sampling
- Parameters: μ_prior (Normal distribution) and τ_prior (Gamma distribution)

### 2. Distribution Validation
- Employs autocorrelation function (ACF) analysis
- Validates convergence of parameters
- Excludes first 100 samples for better accuracy

### 3. VaR and ES Analysis
- Calculates VaR using: VaRα = μ + zα·σ
- Calculates ES using: ESα = μ + φ(zα)·σ
- Analyzes linear correlation between VaR and ES
- Includes density visualization and residual analysis

## Results
The analysis reveals:
- Strong linear correlation between VaR and ES (correlation coefficient: ~0.946)
- Reliable distribution validation through ACF analysis
- Robust parameter convergence in Gibbs sampling

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Create a new Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- Data source: Shanghai Stock Exchange (SSE)
- References:
  - Saturn Cloud: Logarithmic returns calculation
  - Advanced Statistical Computing: Gibbs Sampler implementation

## Contact
[Abby] - [sw546@duke.edu]

Project Link: [https://github.com/abbywang2003/Analyzing-Sustainable-stock-exchange-in-Python-]
