# Episode

- 第66回（2023/05/29）: 記事紹介 - MLOps Maturity Assessment（後編）
  - リンク: https://podcasters.spotify.com/pod/show/double-m2/episodes/66----MLOps-Maturity-Assessment-e24pob1

# Agenda

- 前回に引き続き、プロジェクトレベルでの MLOps の成熟度を測る上で参考になる MLOps Maturity Assessment に関するブログ記事を紹介しました！

# Contents

- Code Quality
  - MLOpsのすべてのステップでテストを含めること
    - データ処理、MLモデルの学習、APIデプロイなど
    - 複数のコンポーネントで構成されるパイプライン全体のE2Eのテストは難しい
  - APIの負荷テストやレイテンシーの確認をすること
    - サービスとしてどこまで許容できるか次第
  - コードのドキュメントやリリースノートの作成
- Monitoring & Support
  - MLプロジェクトにおけるコストの見積もり
    - 過不足をモニタリングし、適切なリソースを付与する
  - インフラリソースの健全性を監視する
    - 不要なインスタンスコストを削除する
  - KPIとモデルパフォーマンスのモニタリング
    - KPIとモデルの評価指標を見える化し、両者の関連性を見極める
  - データドリフトや外れ値の確認
    - ドリフト検知ツールは様々なものがある
      - 例
        - [great expectation](https://greatexpectations.io/)
        - [Evidentaly AI](https://docs.evidentlyai.com/)
- 紹介しきれなかったコンテンツ
  - データ変換のパイプライン設計と特徴量ストア
  - モデルの説明性（透明性） 
  - ABテストの実施とフィードバックループ


# Reference

- [MLOps Maturity Assessment](https://mlops.community/mlops-maturity-assessment/)
