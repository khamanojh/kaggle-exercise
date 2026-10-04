# kaggle-exercise

Kaggle の Titanic コンペを題材にした Python 演習リポジトリ。Google Colab で実行し、コードは GitHub、データと出力は Google Drive で管理する。

## 管理方針

| 置き場所 | 入れるもの |
|---|---|
| GitHub | コード、ノートブック、README |
| Google Drive | 生データ、前処理済みデータ、提出ファイル |
| どちらにも置かない | Kaggle の API キー（Colab の「シークレット」で管理） |

## 構成

```
kaggle-exercise/
├── README.md
├── .gitignore
└── notebooks/
    └── 01_titanic_baseline.ipynb
```

Drive 側は次の構成を想定している。

```
MyDrive/kaggle-exercise/
├── data/titanic/        # train.csv, test.csv など
└── outputs/titanic/     # submission.csv など
```

## 使い方

1. Kaggle で Titanic コンペのページを開き、ルールに同意（Join）する。
2. Kaggle の API 認証情報を取得し、Colab の「シークレット」に `KAGGLE_USERNAME` と `KAGGLE_KEY` として登録する（ノートブックからのアクセスを許可）。
3. `notebooks/01_titanic_baseline.ipynb` を Colab で開き、上から順に実行する。
4. 作業後、Colab の「ファイル → GitHub にコピーを保存」でこのリポジトリに保存する。

## 演習メモ

- [ ] 01: データ取得・EDA・ベースラインモデル
- [ ] 02: 特徴量エンジニアリング（敬称、家族人数、キャビン階など）
- [ ] 03: モデル比較とハイパーパラメータ調整
