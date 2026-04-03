# Quantum Alpha

**Reinforcement Learning Strategy for Dynamic Portfolio Optimization During Market Volatility on NIFTY 50**

A Deep Q-Network (DQN) agent that learns to dynamically adjust long/short/flat exposure in the Indian equity market, with strong emphasis on regime adaptation and risk control during volatility shocks.

## Key Highlights
- Custom Gym-style RL environment for NIFTY trading
- 7-dimensional state vector (momentum, volatility, trend, drawdown, VIX, breadth + position)
- Superior risk management vs traditional momentum rule-based strategy
- Rigorous evaluation: walk-forward validation, multi-regime stress testing, and robustness analysis
- Full research paper (18 pages) included

## Results (2023–2025 Out-of-Sample)

| Metric                | RL Agent     | Rule-Based   | NIFTY Benchmark |
|-----------------------|--------------|--------------|-----------------|
| CAGR (%)              | -3.43        | -8.59        | +13.37          |
| Volatility (%)        | 6.12         | 10.25        | 12.01           |
| Sharpe Ratio          | -1.60        | -1.46        | +0.56           |
| Max Drawdown (%)      | -15.07       | -31.80       | -15.67          |

The agent shows significantly better downside protection while maintaining regime-adaptive behaviour.

## Repository Structure
See folder layout above.

## How to Run
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Explore notebooks in the `/notebooks` folder

## Research Paper
Full 18-page research report available in `/docs/Quantum_Alpha_Research_Paper.pdf`

## Tech Stack
- Python, PyTorch
- Gym-style custom environment
- Pandas, NumPy, Matplotlib, Plotly

## Author
**Ayush Rawat**  
BBA (Finance), Tecnia Institute of Advanced Studies  
Guru Gobind Singh Indraprastha University, Delhi

---

Built as a high-level quant finance project aiming for CFA / financial engineering standards.