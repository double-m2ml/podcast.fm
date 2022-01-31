# Episode
- 第27回（2022/01/24）: 第3回 - 気になる技術記事の紹介
  - リンク: https://anchor.fm/double-m2/episodes/27-3---e1db61e

# Agenda
- 第3回 - 気になる技術記事の紹介
    - How These 8 Companies Implement MLOps: In-Depth Guide
    - Swin Transformer: Hierarchical Vision Transformer using Shifted Windows

# Contents
## How These 8 Companies Implement MLOps: In-Depth Guide
- **asteriam**
    - Neptune.ai
    - MLOpsへのアプローチ方法の紹介
    - プロダクション環境への適用方法
    - プラットフォームの選択肢
        - **Cloud-based/Serverless Implementation**
            - GCP, AWSなどのマネージドサービス
        - **End-to-End Implementation with a Managed Platform**
            - DataRobotなど，もしくは他のAutoMLツール
        - **In-House ML Platform Implementation**
            - 自社で開発している独自のプラットフォーム
    - トレーサビリティ
        - データ・モデル・機械学習パイプライン
            - バージョン管理・実験管理・ログを追跡できる仕組み・監視
    - 事例紹介
        - **Holiday Extras: GCP**
        - データドリフトの監視
        - Google BigQueryでのイベント記録
        - パフォーマンスの可視化
            - Data Studio・Looker
        - Grafana（kibanaのようなログの可視化ツール）
            - スコアリング指標・アラートとエラー・システム指標・エンドポイントにヒットしたリクエストの数
        - **DoorDash:**
            - フードデリバリーサービス
                - 需要予測，飲食店とユーザーのマッチング，ダイナミックプライシングなど
            - LightGBM・PyTorch
            - 学習ジョブのスケジュール
                - Apache Airflow
            - ファイルとメタデータの保存
                - 使用したトレーニングデータ
                - トレーニング時間
                - 使用したハイパーパラメータ
                - Amazon S3
            - 監査とデバッグ
                - メタデータ
                    - 予測時間
                    - 予測に使用されたモデルのID
                - ログ記録
                    - Snowflakeデータストア
            - 特徴量
                - Feature Store
                - 特徴量の標準化（aggregate features, embeddings, など）
    - [MLOps - Practices](https://masatakashiwagi.github.io/mlops-practices/)
        - [ApplyingML](https://applyingml.com/)
        - 日本での各社の取り組みを整理
        - 自分用のメモ

## Swin Transformer: Hierarchical Vision Transformer using Shifted Windows
- **navi**
    - PetFinder2コンペ
    - 物体検出
    - セマンティックセグメンテーション
    - VisionTransformerの課題
        - トークンのスケールが固定
        - 高解像度画像だと入力が長大
    - 解決策
        - 小さいサイズのパッチ
        - 隣接するパッチを結合
        - 階層的な構造（FPNやU-Net）
        - ウィンドウのシフト
        - 局所的なAttension計算
        - 計算効率の簡略化
    - 性能
        - ImageNetでの結果はEfficientNetに近い性能

# Reference
## asteriam紹介記事
- [How These 8 Companies Implement MLOps: In-Depth Guide](https://neptune.ai/blog/how-these-8-companies-implement-mlops)
- [MLOps - Practices](https://masatakashiwagi.github.io/mlops-practices/)
- [ApplyingML](https://applyingml.com/)

## navi紹介記事
- [Swin Transformer: Hierarchical Vision Transformer using Shifted Windows](https://arxiv.org/pdf/2103.14030.pdf)
- [物体検出モデルの進展 Part3 ~ FPNとRetinaNet ~](https://qiita.com/TaigaHasegawa/items/653abc81ac4ee1f0d7b8)
- [論文紹介『Swin Transformer: Hierarchical Vision Transformer using Shifted Windows』](https://kyla.co.jp/blog/2021/05/10/%E8%AB%96%E6%96%87%E7%B4%B9%E4%BB%8B%E3%80%8Eswin-transformer-hierarchical-vision-transformer-using-shifted-windows%E3%80%8F/)
