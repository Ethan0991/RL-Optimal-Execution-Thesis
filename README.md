# Reinforcement Learning for Optimal Execution Algorithms

A Master's Thesis by **Ethan Chemla** in partial fulfillment of the requirements for the M2 in Artificial Intelligence, Systems and Data (IASD) at **University Paris Dauphine - PSL**, in collaboration with the **Execution Algo Team at Natixis CIB**.

[cite_start]Defended: September 17, 2025 [cite: 226]

<a href="[VOTRE_URL_LINKEDIN]"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="Memoire.pdf"><img src="https://img.shields.io/badge/Read_Full_Thesis_(PDF)-FF0000?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="PDF"/></a>

---

## Abstract

> [cite_start]In a context of increasingly complex and non-stationary financial markets, traditional algorithmic execution strategies struggle to maintain their performance[cite: 228]. [cite_start]This thesis, conducted within the quantitative trading team at Natixis, addresses the challenge of moving beyond simple execution optimization to develop an autonomous trading agent capable of generating a consistent execution alpha[cite: 229]. [cite_start]The core problem lies in the critical transition from prediction to action, a gap that this work aims to bridge through a complete and integrated Reinforcement Learning (RL) pipeline[cite: 230]. [cite_start]The methodology is structured in two distinct phases[cite: 231]. [cite_start]First, we focus on building a robust predictive foundation through the engineering of original, theory-driven features[cite: 231]. [cite_start]We introduce two novel concepts: the Noise Range Percentage (NRP), a normalized and adaptive oscillator designed to capture temporary price deviations from its dynamic local trend based on mean-reversion hypotheses, and the Adaptive Trend Finder (ATF), a mechanism that dynamically identifies the most statistically significant trend timescale[cite: 232]. [cite_start]These features, along with more traditional indicators, are used to train advanced supervised models (XGBoost, ResNet) whose probabilistic predictions serve as high-level inputs for the second phase[cite: 233, 234]. [cite_start]The second phase implements the end-to-end reinforcement learning framework[cite: 235]. [cite_start]An agent based on the Proximal Policy Optimization (PPO) algorithm is trained within a custom-built optimal liquidation environment[cite: 235]. [cite_start]Its objective is to intelligently liquidate a significant position over a finite horizon[cite: 236]. [cite_start]The agent's learning is guided by a sophisticated reward function engineered to maximize the financial outperformance against an industry-standard Time-Weighted Average Price (TWAP) benchmark, while incorporating dynamic penalties for adverse market impact and incomplete liquidation[cite: 237]. [cite_start]The agent's policy network leverages a hybrid CNN-LSTM architecture to effectively process the temporal nature of the market state[cite: 238, 239]. [cite_start]The results first validate the predictive edge of our engineered features, which form a solid foundation for the RL agent[cite: 240]. [cite_start]The final out-of-sample evaluation on an unseen dataset confirms the successful training of the PPO agent[cite: 241]. [cite_start]The agent demonstrates the ability to learn a profitable and adaptive execution strategy, generating an average alpha of +$42.19 per episode against the TWAP benchmark, achieving a win rate of 55.57% and a 99.5% order completion rate[cite: 242]. [cite_start]This thesis thus not only establishes a rigorous methodology for high-frequency signal extraction but also demonstrates its practical application by building a complete RL-based agent capable of translating these signals into a superior execution policy[cite: 243].

---

## 🏆 Key Results & Achievements

-   [cite_start]**Generated Positive Alpha**: Achieved an average alpha of **+$42.19 per episode** against the industry-standard TWAP benchmark on an out-of-sample dataset[cite: 242].
-   [cite_start]**Consistent Win Rate**: Outperformed the TWAP benchmark in **55.57%** of the 3000 test episodes, demonstrating a significant predictive edge[cite: 242].
-   [cite_start]**High Reliability**: Successfully liquidated **99.5%** of the initial position across all episodes, confirming the effectiveness of the penalty-driven reward function[cite: 242].
-   [cite_start]**Novel Feature Engineering**: Developed two original, theory-driven features: the **Noise Range Percentage (NRP)** for mean-reversion and the **Adaptive Trend Finder (ATF)** for dynamic trend identification[cite: 232].

---

## 🛠️ Methodology & Keywords

-   [cite_start]**Core Algorithm**: Proximal Policy Optimization (PPO) [cite: 235]
-   [cite_start]**Policy Network**: Hybrid CNN-LSTM Architecture [cite: 238]
-   [cite_start]**Core Problem**: Optimal Liquidation / Algorithmic Execution [cite: 235, 216]
-   [cite_start]**Predictive Models**: XGBoost, ResNet [cite: 233]
-   [cite_start]**Key Concepts**: Markov Decision Process (MDP), TWAP Benchmark, Mean Reversion, Momentum, Kalman Filtering, Isotonic Regression [cite: 245, 247, 248, 282, 237]

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
