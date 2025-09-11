<h1 align="center">Reinforcement Learning for Optimal Execution Algorithms</h1>

<p align="center">
  <em>A Master's Thesis on developing an autonomous trading agent to generate consistent execution alpha.</em>
</p>

<p align="center">
  <a href="[VOTRE_URL_LINKEDIN]"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="Memoire.pdf"><img src="https://img.shields.io/badge/Read_Full_Thesis_(PDF)-FF0000?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="PDF"/></a>
</p>

---

<table>
  <tr>
    <td width="25%"><strong>Author</strong></td>
    [cite_start]<td>Ethan Chemla [cite: 6]</td>
  </tr>
  <tr>
    <td><strong>University</strong></td>
    [cite_start]<td><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Universit%C3%A9_PSL_logo.svg/1280px-Universit%C3%A9_PSL_logo.svg.png" alt="PSL Logo" width="100"> <br> University Paris Dauphine - PSL [cite: 1, 10]</td>
  </tr>
  <tr>
    <td><strong>In collaboration with</strong></td>
    [cite_start]<td><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Natixis_logo.svg/1280px-Natixis_logo.svg.png" alt="Natixis Logo" width="120"> <br> Execution Algo Team at Natixis CIB [cite: 2, 11]</td>
  </tr>
  <tr>
    <td><strong>Degree</strong></td>
    [cite_start]<td>M2 Artificial Intelligence, Systems and Data (IASD) [cite: 9]</td>
  </tr>
  <tr>
    <td><strong>Status</strong></td>
    [cite_start]<td>Defended September 17, 2025 [cite: 14]</td>
  </tr>
</table>

---

## Thesis Overview

[cite_start]This project moves beyond simple market prediction to develop a complete, autonomous trading agent capable of generating consistent execution alpha in complex financial markets[cite: 17]. [cite_start]The core contribution is a fully integrated Reinforcement Learning (RL) pipeline that bridges the critical gap between forecasting and optimal action[cite: 18].

### Phase 1: Building a Predictive Foundation

[cite_start]The first phase focused on engineering a robust predictive signal from high-frequency data[cite: 19].

* [cite_start]**Novel Feature Engineering**: Two original, theory-driven features were developed to capture market dynamics[cite: 20]:
    * [cite_start]**Noise Range Percentage (NRP)**: An adaptive oscillator designed to identify temporary, mean-reverting price deviations from a dynamic local trend[cite: 20].
    * [cite_start]**Adaptive Trend Finder (ATF)**: A mechanism that dynamically identifies the most statistically significant trend timescale[cite: 20].
* [cite_start]**Supervised Model Training**: Advanced models (XGBoost, ResNet) were trained on these features to generate high-level probabilistic forecasts[cite: 21]. [cite_start]These predictions are not the final output, but rather a key input for the RL agent[cite: 21, 22].

### Phase 2: The Autonomous Execution Agent

[cite_start]The second phase implemented the end-to-end reinforcement learning framework to transform predictive signals into an optimal execution policy[cite: 23].

* **RL Framework**:
    * [cite_start]**Algorithm**: An agent based on **Proximal Policy Optimization (PPO)** was trained to intelligently liquidate a significant position over a finite horizon[cite: 23, 24].
    * [cite_start]**Custom Environment**: The agent learns within a custom-built optimal liquidation environment[cite: 23].
    * [cite_start]**Reward Function**: The agent's learning is guided by a sophisticated reward function designed to maximize financial outperformance against a **Time-Weighted Average Price (TWAP)** benchmark, including penalties for market impact and incomplete liquidation[cite: 25].
    * [cite_start]**Policy Network**: The agent leverages a hybrid **CNN-LSTM architecture** to effectively process the temporal nature of the market state[cite: 26, 27].

### Validation & Results

[cite_start]The final out-of-sample evaluation on an unseen dataset confirms the successful training of a profitable and adaptive execution strategy[cite: 29]. [cite_start]The agent demonstrated the ability to translate high-frequency signals into a superior execution policy[cite: 31], achieving:
* [cite_start]**Average Alpha**: +$42.19 per episode against the TWAP benchmark[cite: 30].
* [cite_start]**Win Rate**: 55.57% over 3000 test episodes[cite: 30].
* [cite_start]**Order Completion**: A 99.5% order completion rate[cite: 30].

---

## 🏆 Key Results & Achievements

-   [cite_start]**Generated Positive Alpha**: Achieved an average alpha of **+$42.19 per episode** against the industry-standard TWAP benchmark on an out-of-sample dataset[cite: 30].
-   [cite_start]**Consistent Win Rate**: Outperformed the TWAP benchmark in **55.57%** of the 3000 test episodes, demonstrating a significant predictive edge[cite: 30].
-   [cite_start]**High Reliability**: Successfully liquidated **99.5%** of the initial position across all episodes, confirming the effectiveness of the penalty-driven reward function[cite: 30].
-   [cite_start]**Novel Feature Engineering**: Developed two original, theory-driven features: the **Noise Range Percentage (NRP)** for mean-reversion and the **Adaptive Trend Finder (ATF)** for dynamic trend identification[cite: 20].

---

## 🛠️ Methodology & Keywords

-   [cite_start]**Core Algorithm**: Proximal Policy Optimization (PPO) [cite: 23]
-   [cite_start]**Policy Network**: Hybrid CNN-LSTM Architecture [cite: 26]
-   [cite_start]**Core Problem**: Optimal Liquidation / Algorithmic Execution [cite: 16, 23]
-   [cite_start]**Predictive Models**: XGBoost, ResNet [cite: 21]
-   [cite_start]**Key Concepts**: Markov Decision Process (MDP) [cite: 81][cite_start], TWAP Benchmark [cite: 25][cite_start], Mean Reversion [cite: 32][cite_start], Momentum [cite: 34][cite_start], Kalman Filtering [cite: 36][cite_start], Isotonic Regression [cite: 37]

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
