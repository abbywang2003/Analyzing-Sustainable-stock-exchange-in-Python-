# 📈 Shanghai Stock Exchange (SSE) Risk Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Latest-blue)
![SciPy](https://img.shields.io/badge/SciPy-Latest-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 🎯 Project Overview

This project performs an advanced statistical analysis of the Shanghai Stock Exchange (SSE) Composite Index to assess financial risk through Value at Risk (VaR) and Expected Shortfall (ES) calculations. Using Bayesian inference and Gibbs sampling, we create a robust framework for market risk assessment.

![Project Structure](https://via.placeholder.com/800x400.png?text=SSE+Analysis+Pipeline)

## 🔑 Key Features

- 📊 Log returns calculation and distribution analysis
- 🔄 Bayesian parameter estimation using Gibbs sampling
- 📉 VaR and ES risk metrics computation
- 📋 Distribution validation using autocorrelation
- 📈 Linear correlation analysis between risk metrics

## 🛠️ Technical Implementation

### Data Processing Pipeline

```mermaid
graph LR
    A[Raw SSE Data] --> B[Log Returns]
    B --> C[Parameter Estimation]
    C --> D[Distribution Validation]
    D --> E[Risk Metrics]
    E --> F[Correlation Analysis]
```

### Key Formulas

#### 1. Logarithmic Returns
```python
LogarithmicReturn = ln(PresentValue/PastValue)
```

#### 2. Risk Metrics
```python
VaRα = μ + zα·σ
ESα = μ + φ(zα)·σ
```

## 📊 Results

### Distribution Validation
![ACF Plot](https://via.placeholder.com/600x300.png?text=ACF+Plot)

### Risk Metrics Correlation
- Correlation Coefficient: 0.946
- Strong linear relationship between VaR and ES
- Higher density in middle values

## 🚀 Getting Started

### Prerequisites
```python
pip install pandas numpy scipy matplotlib seaborn
```

### Running the Analysis
```python
# Clone repository
git clone https://github.com/yourusername/sse-analysis.git

# Navigate to project directory
cd sse-analysis

# Run main analysis
python main.py
```

## 📁 Project Structure

```
sse-analysis/
│
├── data/
│   └── sse_data.csv
│
├── src/
│   ├── data_processing.py
│   ├── parameter_estimation.py
│   ├── risk_metrics.py
│   └── visualization.py
│
├── notebooks/
│   └── analysis.ipynb
│
└── results/
    ├── figures/
    └── statistics/
```

## 🔍 Methodology

### Bayesian Framework
- **Prior Distributions**
  - Normal Distribution (μ_prior): `(0, 10000)`
  - Gamma Distribution (τ_prior): `(1, 1000)`

### Computational Efficiency
- Time Complexity: `O(n * m)`
  - n: iterations
  - m: data length

## 📊 Visualizations

### Distribution Analysis
![Distribution](https://via.placeholder.com/600x300.png?text=Distribution+Analysis)

### Risk Metrics Correlation
![Correlation](https://via.placeholder.com/600x300.png?text=Risk+Metrics+Correlation)

## 🎓 Research Background

This project implements concepts from:
- Bayesian inference
- Financial risk assessment
- Time series analysis
- Statistical modeling

## 📝 Citation

```bibtex
@article{YourName2024,
  title={Risk Assessment of Shanghai Stock Exchange Using Bayesian Methods},
  author={Your Name},
  year={2024}
}
```

## 📫 Contact

- **Author**: [Abby Wang]
- **Email**: [sw546@duke.edu]
- **LinkedIn**: [https://www.linkedin.com/in/siyuan-wang-abby/]


---
⭐ If you find this project useful, please consider giving it a star!
