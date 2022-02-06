# Episode
- 第29回（2022/02/07）: Data-Centric AIの紹介
    - リンク: https://anchor.fm/double-m2/episodes/29-Data-Centric-AI-e1e0cqr

# Agenda
- Data-Centric AIの紹介
- Data-Centricを実現するサービスやツールの紹介

# Contents
- Data-Centric AIとは
    - Andrew Ng先生が提唱する
    - モデルではなくデータの品質を高める・改良していく思想
        - モデルは固定
    - ユースケース：外観検査
        - モデルを改善したケースとデータを改善したケースで精度比較
        - データを改善したケースが大幅に改善した
    - システマティクにアノテーションできる仕組みが必要
    - データが少ない場合はより品質が大事になる
- Data-Centric AI Competition
    - 手書きのローマ字データセットの分類
    - モデルは固定でデータセットを改良するコンペ
        - 工夫するポイント
            - 前処理やノイズ処理，データの水増しなど
            - バリデーション方法
    - ベースラインと比較して20%くらい改善した
- Data-Centric AIを実現するプラットフォーム
    - Akridata
    - トヨタなどとパートナー組んでいる
- SnorkelというPythonライブラリ
    - ラベル付けや前処理を便利にしてくれるライブラリ
    - Data-Centricの思想に基づいて，データを正しく整形することに主眼を置いている
    - ラベリングでは各種統計データや以下の項目の指標が自動で計算できる
        - Polarity
        - Coverage
        - Overlaps
        - Conflicts
        - Correct
        - Incorrect
        - Empirical Accuracy
    - データスライシング
        - データセット全体から特定の範囲を切り取り，モデルの精度を確認できる
        - 特定のデータだけ精度が落ちていないかなど
- Snorkel Flow
    - ダッシュボードが用意されていてUIで分析やモニタリングできる

# Reference
- [Data-Centric AIの紹介](https://www.slideshare.net/KazuyukiMiyazawa/datacentric-ai)
- [Data-centricなML開発](https://www.slideshare.net/TakeshiSuzuki21/data-centricml-248354451)
- [Akridata](https://www.akridata.com/)
- [Snorkel](https://snorkel.ai/)
- [Snorkel Flow](https://snorkel.ai/platform/)
- [snorkel-team/snorkel](https://github.com/snorkel-team/snorkel)