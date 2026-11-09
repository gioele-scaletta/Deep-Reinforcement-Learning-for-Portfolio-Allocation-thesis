# Deep Reinforcement Learning for Portfolio Optimization

MSc thesis — Politecnico di Torino, 2024
**Author:** Gioele Scaletta

## 📄 Links
- **Official thesis (PoliTo webthesis):** https://webthesis.biblio.polito.it/31091/
- **Presentation slides:** [Scaletta_Gioele_thesis_ppt_final.pdf](./Scaletta_Gioele_thesis_ppt_final.pdf)

## Overview
This thesis applies Deep Reinforcement Learning to automate equity portfolio management.
An agent observes past prices and technical indicators and outputs daily portfolio weights,
with the previous step's portfolio return as reward and 0.1% transaction costs.

Starting from a PPO baseline, three variants are explored:
1. **PPO + Gated Transformer-XL (GTrXL)** to better embed past prices and indicators
2. **PPO pre-trained on expert actions**, derived from optimal actions in hindsight
3. **TD3+BC (offline RL)**, i.e. Twin Delayed DDPG with behavioural cloning, trained on a set enlarged with S&P 500-sampled stocks

Models are tested on Dow Jones Industrial Average stocks. Variant 3 consistently outperformed
the baseline in backtesting, while stability across runs remained the main open issue.

## Repository contents
- `Scaletta_Gioele_thesis_ppt_final.pdf` — defence slides

## Contact
[LinkedIn](https://www.linkedin.com/in/gioele-scaletta-5b154b1a6) · gioelescaletta@gmail.com
