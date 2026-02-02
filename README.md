# Inventory Optimization Model

## Business Context
Inventory decisions directly impact profitability—ordering too much ties up capital and increases holding costs, while ordering too little leads to stockouts and lost revenue. This project implements mathematical optimization models to determine optimal inventory levels under demand uncertainty.

## Project Highlights

### Problem Addressed
Developed an **inventory optimization system** using the Newsvendor framework to maximize expected profit while accounting for:
- Uncertain customer demand
- Rush order premiums for emergency restocking
- Disposal costs for excess inventory
- Price-demand elasticity

### Key Outcomes
- **Profit Maximization**: Built LP/QP models to find optimal order quantities
- **Dynamic Pricing**: Extended model to jointly optimize price and quantity decisions
- **Risk Quantification**: Used bootstrap analysis to generate confidence intervals for recommendations
- **Demand Modeling**: Implemented regression to predict demand based on pricing decisions

## Methodology
1. **Demand Forecasting**: Linear regression modeling of price-demand relationship
2. **Optimization**: Gurobi-based Linear and Quadratic Programming formulations
3. **Uncertainty Analysis**: Bootstrap resampling (1,000+ iterations) for robust decision-making

## Technologies
| Category | Tools |
|----------|-------|
| Optimization | Gurobi (LP/QP Solver) |
| Analytics | Python, Pandas, NumPy, Scikit-learn |
| Visualization | Matplotlib, Seaborn |

## How to Run
```bash
pip install numpy pandas matplotlib seaborn scikit-learn gurobipy
jupyter notebook Analysis.ipynb
```
*Note: Requires Gurobi license (free academic licenses available)*

## Skills Demonstrated
- **Inventory Management** - Newsvendor model, safety stock, service level optimization
- **Mathematical Optimization** - Linear Programming, Quadratic Programming, constraint modeling
- **Demand Forecasting** - Regression analysis, price elasticity modeling
- **Risk Analysis** - Bootstrap methods, confidence intervals, uncertainty quantification
- **Python Programming** - Data manipulation, optimization modeling, visualization

