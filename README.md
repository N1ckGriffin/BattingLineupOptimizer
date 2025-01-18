# Baseball Batting Order Optimization

This project implements a machine learning approach to optimize baseball batting orders using XGBoost classifiers. The system analyzes player statistics and predicts optimal batting positions based on historical MLB data, with separate models for facing right-handed and left-handed pitchers.

## Features

- Three distinct XGBoost models:
  - General batting order optimization
  - Specific optimization for facing left-handed pitchers
  - Specific optimization for facing right-handed pitchers
- Hyperparameter optimization using RandomizedSearchCV
- Hungarian Algorithm implementation for optimal player assignment
- Feature importance analysis for model interpretability
- Comprehensive player statistics processing
- Support for both standard and combinatorial optimization approaches

## Installation

```bash
pip install -r requirements.txt
```

## Usage

1. Prepare your player statistics in CSV format
2. Run the models to generate optimized batting orders:
   ```python
   python batting_order_optimizer.py
   ```

## Data Requirements

Input CSV files should include the following statistics:
- Basic batting statistics (AVG, OBP, SLG)
- Advanced metrics (wOBA, wRC+)
- Physical attributes (height, weight)
- Handedness information
- Split statistics (vs LHP/RHP)

## Contributors

- Nicholas Griffin
- Drew Kearney
- Nicholas Kim