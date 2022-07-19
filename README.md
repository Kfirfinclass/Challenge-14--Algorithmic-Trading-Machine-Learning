# Challenge 14 -Algorithmic Trading + Machine Learning

In this Challenge, you’ll assume the role of a financial advisor at one of the top five financial advisory firms in the world. Your firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment. In recent years, your firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.

The speed of these transactions gave your firm a competitive advantage early on. But, people still need to specifically program these systems, which limits their ability to adapt to new data. You’re thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market. To do so, you’ll enhance the existing trading signals with machine learning algorithms that can adapt to new data.

# Technologies

Please run the following commands in your terminal once you have cloned the repository to your local machine.
run pip install -r requirements.txt

---

## Installation Guide

Clone Repo
Run pip install -r requirements.txt


---

# Analysis

## Baseline Performance
Actual vs Strategy Returns:
<img width="673" alt="baseline" src="https://user-images.githubusercontent.com/98926901/179636709-e8ef0b25-0ef8-485a-9e50-3aa3514d4164.png">


The baseline strategy currently outperforms actual returns so it is a strong baseline. 
Can we produce a better return?

## Tuning the Baseline


What impact resulted from increasing or decreasing the training window?
- The strategy returns performed better than the baseline when the training window increased to 6 months.
<img width="673" alt="baseline6" src="https://user-images.githubusercontent.com/98926901/179636725-9bc93769-e5dd-45f3-9543-c8782830f1c0.png">


What impact resulted from increasing or decreasing either or both of the SMA windows?
- By adjusting the windows up to 16 and 120, the strategy returns underperformed against the baseline. 
<img width="600" alt="sma" src="https://user-images.githubusercontent.com/98926901/179636738-c2b48b25-e9f8-4723-af87-c7db069377f5.png">

As per the above photos, increasing the trading window appears to allow better predictions and a more accurate model, which retults in better strategy returns. 

## New Machine Learning Classifier
<img width="743" alt="baseml" src="https://user-images.githubusercontent.com/98926901/179636774-b9df6ae1-89cb-499d-9d2f-4fc7d4a65175.png">


Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?

-The AdaBoost Classifier does a better job than the baseline model once volatility occured after the big downturn in march, but my Ada tuned ML algorithm does get beat by the regular algo.
--- 

## Contributors

Kfir Bar
kfirfinclass@gmail.com

---

## License

This code is exclusive to those who are provided a direct access. A user-key feature can be added later.
