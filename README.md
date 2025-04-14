# Tesla Risk Metrics Estimation

## Project Overview
This project estimates financial risk for a single asset (Tesla Inc.) by calculating **Value at Risk (VaR)** and **Expected Shortfall (ES)** using both historical simulation and parametric methods. It also evaluates the stability of these estimates using bootstrapped standard errors and confidence intervals.

---

## Tools & Techniques

**Python Libraries:**
- `pandas`, `numpy`, `yfinance`
- `scipy.stats`, `matplotlib`, `seaborn`

**Risk Metrics Calculated:**
- Historical VaR & ES (log and simple returns)
- Parametric VaR & ES using:
  - Normal distribution (simple returns)
  - Log-normal distribution (log returns, simulated ES)

**Statistical Evaluation:**
- Bootstrapping (1,000 resamples)
- Standard Error estimation
- 95% Confidence Intervals using percentile method

---

## Key Insights

- Historical methods better captured extreme losses but had greater variability, especially for ES.
- Parametric (normal) methods were efficient but slightly underestimated tail risk.
- Log-normal VaR reflected compounded losses more realistically; log-return ES required simulation.
- Bootstrap analysis showed:
  - ES is inherently more volatile than VaR
  - Estimates at 99% confidence levels had wider intervals, indicating more uncertainty

---

## Skills Demonstrated

- Financial risk modeling
- Statistical inference with bootstrapping
- Data visualization and interpretation
- Clean, modular Python scripting for risk analysis


