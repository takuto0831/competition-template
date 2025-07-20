# Overview

- [目指せメダリスト！Kaggle実験管理術 着実にコンペで成果を出すためのノウハウ](https://www.shoeisha.co.jp/book/detail/9784798187457) を参考にレポジトリを組む

# Flow

1. preprocessX のフォルダーでデータの前処理をする
2. source/fixed/preprocessX 以下に 前処理済みのデータを配置する
3. expXXX.ipynb で source/fixed/preprocessX 以下のデータを参照してmodelを実行する
4. results/expXXX に expXXX.ipynbでの実験結果を保存する
5. results/total_results.csv に結果をまとめておく


```
├── experiments
│   ├── exp001.ipynb
│   └── exp002.ipynb
├── preprocess
│   ├── preprocess1
│   └── preprocess2
├── README.md
├── results
│   ├── exp001
│   │   ├── model.pkl
│   │   └── results.csv
│   └── exp002
└── source
    ├── fixed
    │   ├── preprocess1
    │   └── preprocess2
    └── raw
```
