# Sentence Predict
* Goal: using the fact of judgement predict sentence
---
## Dataset 3/15 Update
* Remove duplicate judgements
* Remove judgments with excessively long "facts"

## Method 1: BM25
* 直接用事實預測刑期
* 套件: Pyserini
* 流程: 建立反向索引，使用LuceneSearcher搜尋
* Reslut

| Metric | Value |
|--------|-------|
| MSE    | 22868.76 |
| RMSE   | 151.22 |
| MAE    | 108.20 |
---
## Method 2: Summary
* 把事實先壓縮到3k以下，看情節摘要做得如何
* 模型: Breeze