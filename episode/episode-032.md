# Episode
- 第32回（2022/04/18）: MLモニタリング - ドリフトの話
    - リンク: 

# Agenda
- スピーカーそれぞれがモニタリングに関する記事の紹介をしました
    - ML Monitors (asteriam)
    - Machine Learning Monitoring, Part 5: Why You Should Care About Data and Concept Drift (navi)

リンクは`Reference`を参照してください

# Contents
## asteriam
- 機械学習の一般的なモニタリング指標の紹介
    - **Data quality monitors（データの質）**
        - 欠損データ
        - 新しい特徴量
        - データレンジ
        - データタイプのミスマッチ
    - **Drift monitors（データドリフト&コンセプトドリフト）**
    - **Model activity monitors（モデルの活動）**
        - 予測件数
        - モデルの負荷状況
        - 将来的なトレンド
    - **Performance monitors（パフォーマンス）**
        - 各種メトリクス

## navi
- データドリフトとコンセプトドリフトの紹介
    - **モデルは必ず劣化する**
        - 状況の変化でモデルは劣化する
            - モデルをモニタリングし再学習する頻度を考える必要がある
        - 状況の変化というのは以下の2つ
            - データドリフト
            - コンセプトドリフト
    - **データドリフト**
        - 入力データにあたる特徴量の分布が変わること
        - 例：広告流入データからパーソナライズされたオファーを送信し、購入する可能性を予測
            - Facebookからの流入が増えてモデルがうまくいかなかった
    - **コンセプトドリフト**
        - モデルのターゲットの性質が変わる
            - →予測していることの意味が変わる
            - 徐々に変化するパターンと急に変化するパターンが存在する
        - 徐々に変化するパターン
            - 例：製造業における品質予測モデル
                - 機械の劣化による影響
        - 急に変化するパターン
            - 例：感染症予測モデル
                - COVID-19によるパンデミック
    - 対策
        - モデルの再学習（新しいデータを使う）

# Reference
- [ML Monitors](https://censius.ai/wiki/ml-monitors)
- [Machine Learning Monitoring, Part 5: Why You Should Care About Data and Concept Drift](https://evidentlyai.com/blog/machine-learning-monitoring-data-and-concept-drift)
- [機械学習デザインパターン / O'Reilly](https://www.oreilly.co.jp/books/9784873119564/)
