# MLP-for-Optimal-Equity-Derivative-Hedging
## Award Recognition 🏆
**1st Place Certificate** – **Bay Area Data Science Summit 2025 (BADSS2025)** 

## Overview
This project presents a **Multi-Layer Perceptron (MLP)-based framework** for **optimal equity derivative hedging**, developed as part of our award-winning participation in the **Bay Area Data Science Summit 2025 (BADSS2025)**. 

Our model leverages:
- **Multi-Layer Perceptron** to optimize hedging strategies.
- **Real-time data processing** for dynamic risk management.
- **Exposure-PnL mapping** to balance profitability and risk.
- **A smart buy-sell greedy strategy** that adapts to market fluctuations.

Our experimental results demonstrate **substantial cost reduction and enhanced risk mitigation**, making our approach highly applicable for algorithmic trading in real-world financial markets.

## Methodology

### 1. Data Preprocessing
- **Handling missing data**: Filling in gaps while preserving data integrity.
- **Time series alignment**: Ensuring consistent tracking of options data.
- **PnL & Exposure calculations**: Computing key risk and profitability metrics.

### 2. Labeling and Network Training
- **Novel Labeling Mechanism**: A PnL-Exposure trade-off function for prioritizing options.
- **Multi-Layer Perceptron (MLP)**:
  - Architecture: **128 → 64 → 32 → 1**
  - **5-fold cross-validation** to prevent overfitting.
  - Optimized for **non-linear market relationships**.

### 3. Decision Logic
- **Dynamic exposure control**: Meeting daily exposure targets of **≥ $10M**.
- **Buy-sell execution strategy**:
  1. **Managing existing sell orders** via a structured dictionary.
  2. **Iterative purchase adjustment** based on ranked option labels.
  3. **Real-time exposure updates** ensuring risk-aware trading decisions.

## Key Results
|  | **Training Set** | **Testing Set** |
|-----------------|-----------------|-----------------|
| **Cost** | $11,097,348 | $11,299,563 |
| **Profit (Baseline)** | $5,552,290 | $22,560,857 |
| **Profit (Our Model)** | $2,779,349 | $4,008,805 |

- **Significant cost reduction** while maintaining exposure.
- **Robust tracking of non-linear option behavior**.
- **Scalable framework for future enhancements**.

## Important Notice
Due to competition regulations, **we are unable to publicly share our training and testing datasets**. The model implementation provided in this repository is **for reference purposes only** and may require adaptation for real-world deployment.

## Future Work
- **Feature importance evaluation**: Identifying the most critical market indicators.
- **Market adaptability**: Enhancing the model’s responsiveness to financial trends.
- **Explainability**: Improving interpretability for financial professionals.
