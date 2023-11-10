# TARGET

目标是预测第二天的收盘价，close_price_shifted 作为预测的目标变量。

# TASKS

## T1: 验证社交媒体情绪对股票收盘价的影响

based on 3 different dataset: Y(基线)，Y + finbert，Y + Vader

## T2: model comparation

Target: choose a fit model

based on dev_set

## T3: stock price prediction & trading strategy

based on test_set

# Dataset

数据时间范围：2015.1.1-2019-12-31

Source：

- https://www.kaggle.com/datasets/omermetinn/tweets-about-the-top-companies-from-2015-to-2020
- yahoo finance

# Project Structure

FINAL/
├── data/
│ ├── original/
│ ├── finbert/
│ └── output/
├── models/
│ ├── finbert_GRU_model.pkl
│ ├── finbert_LSTM_model.pkl
│ ├── finbert_MLP_model.pkl
| └── finbert_RNN_model.pkl
├── notebooks/
│ ├── SA-VADER.ipynb
│ ├── SA-Finbert.ipynb
| ├── DataPreprocession.ipynb
│ ├── Experiment1.ipynb
| ├── Experiment2.ipynb
| └── Experiment3.ipynb
└── README.md
