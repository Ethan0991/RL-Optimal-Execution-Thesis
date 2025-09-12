<h1 align="center">Reinforcement Learning for Optimal Execution Algorithms</h1>

<p align="center">
  <em>A Master's Thesis on developing an autonomous trading agent to generate consistent execution alpha.</em>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ethanchemla/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="Masters_Thesis.pdf"><img src="data:image/png;base64,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" alt="PDF"/></a>
</p>

---

<table>
  <tr>
    <td width="25%"><strong>Author</strong></td>
    <td>Ethan Chemla</td>
  </tr>
  <tr>
    <td><strong>University</strong></td>
    <td><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Universit%C3%A9_PSL_logo.svg/1280px-Universit%C3%A9_PSL_logo.svg.png" alt="PSL Logo" width="100"> <br> University Paris Dauphine - PSL</td>
  </tr>
  <tr>
    <td><strong>In collaboration with</strong></td>
    <td><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Natixis_logo.svg/1280px-Natixis_logo.svg.png" alt="Natixis Logo" width="120"> <br> Execution Algo Team at Natixis CIB</td>
  </tr>
  <tr>
    <td><strong>Degree</strong></td>
    <td>M2 Artificial Intelligence, Systems and Data (IASD)</td>
  </tr>
  <tr>
    <td><strong>Status</strong></td>
    <td>Defended September 17, 2025</td>
  </tr>
</table>

---

## Thesis Overview

This project moves beyond simple market prediction to develop a complete, autonomous trading agent capable of generating consistent execution alpha in complex financial markets. The core contribution is a fully integrated Reinforcement Learning (RL) pipeline that bridges the critical gap between forecasting and optimal action.

### Phase 1: Building a Predictive Foundation

The first phase focused on engineering a robust predictive signal from high-frequency data.

* **Novel Feature Engineering**: Two original, theory-driven features were developed to capture market dynamics:
    * **Noise Range Percentage (NRP)**: An adaptive oscillator designed to identify temporary, mean-reverting price deviations from a dynamic local trend.
    * **Adaptive Trend Finder (ATF)**: A mechanism that dynamically identifies the most statistically significant trend timescale.
* **Supervised Model Training**: Advanced models (XGBoost, ResNet) were trained on these features to generate high-level probabilistic forecasts. These predictions are not the final output, but rather a key input for the RL agent.

### Phase 2: The Autonomous Execution Agent

The second phase implemented the end-to-end reinforcement learning framework to transform predictive signals into an optimal execution policy.

* **RL Framework**:
    * **Algorithm**: An agent based on **Proximal Policy Optimization (PPO)** was trained to intelligently liquidate a significant position over a finite horizon.
    * **Custom Environment**: The agent learns within a custom-built optimal liquidation environment.
    * **Reward Function**: The agent's learning is guided by a sophisticated reward function designed to maximize financial outperformance against a **Time-Weighted Average Price (TWAP)** benchmark, including penalties for market impact and incomplete liquidation.
    * **Policy Network**: The agent leverages a hybrid **CNN-LSTM architecture** to effectively process the temporal nature of the market state.

### Validation & Results

The final out-of-sample evaluation on an unseen dataset confirms the successful training of a profitable and adaptive execution strategy. The agent demonstrated the ability to translate high-frequency signals into a superior execution policy, achieving:
* **Average Alpha**: +$42.19 per episode against the TWAP benchmark.
* **Win Rate**: 55.57% over 3000 test episodes.
* **Order Completion**: A 99.5% order completion rate.

---

## 🏆 Key Results & Achievements

-   **Generated Positive Alpha**: Achieved an average alpha of **+$42.19 per episode** against the industry-standard TWAP benchmark on an out-of-sample dataset.
-   **Consistent Win Rate**: Outperformed the TWAP benchmark in **55.57%** of the 3000 test episodes, demonstrating a significant predictive edge.
-   **High Reliability**: Successfully liquidated **99.5%** of the initial position across all episodes, confirming the effectiveness of the penalty-driven reward function.
-   **Novel Feature Engineering**: Developed two original, theory-driven features: the **Noise Range Percentage (NRP)** for mean-reversion and the **Adaptive Trend Finder (ATF)** for dynamic trend identification.

---

## 🛠️ Methodology & Keywords

-   **Core Algorithm**: Proximal Policy Optimization (PPO)
-   **Policy Network**: Hybrid CNN-LSTM Architecture
-   **Core Problem**: Optimal Liquidation / Algorithmic Execution
-   **Predictive Models**: XGBoost, ResNet
-   **Key Concepts**: Markov Decision Process (MDP), TWAP Benchmark, Mean Reversion, Momentum, Kalman Filtering, Isotonic Regression

---

## 📊 Visualizations

*Example of the agent's adaptive liquidation strategy compared to the static TWAP benchmark. Green areas show an aggressive (faster) liquidation pace, while red shows a passive (slower) pace.*
![Agent Liquidation Trajectory](example_liquidation.png)

*Evolution of the agent's performance (PnL difference vs. TWAP) over the training period, smoothed with a 5000-episode moving average, demonstrating a clear and robust learning curve.*
![Smoothed Learning Curve](example_learning_curve.png)

---

## 📜 Read the Full Thesis

For a complete breakdown of the methodology, mathematical formulations, and detailed results, you can access the full PDF here:

**[➡️ Download Memoire.pdf](Memoire.pdf)**
