# Who-Carries-Harder-Giannis-vs.-Jokic-Team-Impact-Exploration
Who Carries Harder? is a data science mini-project from the 2025 NBA season Which team would suffer more without its superstar — the Milwaukee Bucks without Giannis Antetokounmpo, or the Denver Nuggets without Nikola Jokić?


> Which team would be worse without its star, the **Milwaukee Bucks** (Giannis) or the **Denver Nuggets** (Jokić)?

[![Open in Colab]([https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/15yZasq2c1zyus3Vn-SJT4jffHBSdoBpo?usp=sharing)](#) <!-- Replace # with your Colab link if you want -->

## Overview
I estimate each team’s wins **with vs. without** their star using on/off efficiency and a pace adjustment, then map point differential to win% with a common analytics heuristic.

## Method (brief)
- Inputs: offensive/defensive points per 100 poss. (on), on/off differentials, average pace  
- Steps: convert on→off via on/off, adjust to pace, transform differential → win%  
- Output: estimated wins over an 82-game season

## Result
- **Bucks without Giannis:** ~28 wins  
- **Nuggets without Jokić:** ~14 wins

Interpretation: within this framework, Jokić appears to have the larger single-player impact on team performance.


## How to Run
**Colab:** click the badge at top.  
**Local:**
```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
# open the notebook in VS Code / Jupyter and run all cells
