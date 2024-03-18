# Sentence Predict
* Goal: using the fact of judgement predict sentence
---
## Dataset 3/15 Update
* Remove duplicate judgements
* Remove judgments with excessively long "facts"
* Remove outliers

## Method 1: BM25
* 直接用事實預測刑期
* 套件: Pyserini
* 流程：建立反向索引，使用LuceneSearcher搜尋
* Reslut
| Metric | Value                |
|--------|----------------------|
| MSE    | 22868.76             |
| RMSE   | 151.22420441185994  |
| MAE    | 108.2                |

## Method 2: Summary
* 把事實做情節摘要，再預測刑期
* 套件: Breeze
* 流程: 超過5,000字，用sliding window做摘要