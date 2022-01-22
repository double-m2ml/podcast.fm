# Episode
- 第27回（2022/01/24）: 第3回 - 気になる技術記事の紹介
  - リンク:

# Contents
- 第3回 - 気になる技術記事の紹介
    - How These 8 Companies Implement MLOps: In-Depth Guide
    - Swin Transformer: Hierarchical Vision Transformer using Shifted Windows

## 内容

### How These 8 Companies Implement MLOps: In-Depth Guide
- ここで紹介されている8社が，どのようにしてプロダクション環境にモデルを管理してデプロイして改善しているのか，MLOpsに対して，どうアプローチしているのかを紹介
- MLOpsを実践していくためのプラットフォームとして何を選択しているか
    - **Cloud-based/Serverless Implementation**
        - GCP, AWSなどのマネージドサービス
    - **End-to-End Implementation with a Managed Platform**
        - DataRobotなど，もしくは他のAutoMLツール
    - **In-House ML Platform Implementation**
        - 自社で開発している独自のプラットフォーム
- MLOpsを成功させるためには，ワークフローに関連するすべてのコンポーネントのアクティビティを追跡するということ
    - データ・モデル・機械学習パイプライン
        - バージョン管理・実験管理・ログを追跡できる仕組み・監視
- **Holiday Extras: GCP**
    - **Monitoring model performance in production**
        - データのドリフトを監視するために，Google BigQueryを使って予測イベントを記録し，Data StudioやLookerなどのツールでパフォーマンスとドリフトを可視化できるようにしている．
        - Grafana（kibanaのようなログの可視化ツール）を使用して，AI Platformからログに記録されたイベントをスコアリング指標・アラートとエラー・システム指標・エンドポイントにヒットしたリクエストの数などの観点から可視化している
- **DoorDash:**
    - フードデリバリーサービス
        - 需要予測，飲食店とユーザーのマッチング，ダイナミックプライシングなど
    - LightGBM, PyTorchなどのライブラリを使用している
    - 学習ジョブのスケジュールと実行には，Apache Airflowを使用
    - ファイル（モデルのネイティブフォーマットとモデル設定）とメタデータ（使用したトレーニングデータ、トレーニング時間、使用したハイパーパラメータ）はモデルストア（Amazon S3に格納）に保存
    - 監査とデバッグのために，予測時間や予測に使用されたモデルのIDなどのメタデータとともにSnowflakeデータストアにログ記録
    - 特徴量はFeature Storeで管理して使用する特徴量を標準化している（aggregate features, embeddings, など）
- MLOps Practices
    - [ApplyingML](https://applyingml.com/)
    - 上記サイトに触発されて，日本での各社の取り組みを整理したやつ欲しいなと思って，自分のメモという確認用に作ったやつを更新して行きたいなーという思いで始めました

### Swin Transformer: Hierarchical Vision Transformer using Shifted Windows
- PetFinder2コンペでみんな使っていたVisionTransformerの進化版
- VisionTransformerの適用範囲を拡大する（物体検出やセマセグ）ために以下2つの課題を解消するための新しいBackbone
    - トークンのスケールが固定（画像を特定サイズのパッチに切り分けて入力していたが，大きさが固定になってしまう）
    - 高解像度画像だと入力が長大（TransformerのAttensionが画像サイズの2乗になる）
- 解決策として
    - 小さいサイズのパッチから計算を開始し，徐々に隣接するパッチを結合していく階層的な構造（FPNやU-Net）
    - ウィンドウをシフトし局所的なAttension計算を実現（計算効率の簡略化）
- Patch Partition
    - 重複なしのパッチ分割（ViTと同じ）
    - FeatureはRGB値を連結し，4*4*3 = 48となる
- Patch Marge
    - 2*2の隣接したパッチの特徴を連結しダウンサンプリングする（プーリング層に近い考えかた）
- Swin Transformer Block
    - MSA: Multi Self-Attention
    - LN: LayerNorm
    - W-MSA: シフトなしのウィンドウベースのSelf-Attension
    - SW-MSA: シフトウィンドウに基づくSelf-Attension
    - MLP: Multi Layer Perceptron
- 性能
    - ImageNetでの結果はEfficientNetに近い性能
- 余談
    - Petfinderコンペの終盤に新しいBackboneが公開された -> その名も「ConvNeXt」

## Reference
- [How These 8 Companies Implement MLOps: In-Depth Guide](https://neptune.ai/blog/how-these-8-companies-implement-mlops)
- [Swin Transformer: Hierarchical Vision Transformer using Shifted Windows](https://arxiv.org/pdf/2103.14030.pdf)
    - [物体検出モデルの進展 Part3 ~FPNとRetinaNet~](https://qiita.com/TaigaHasegawa/items/653abc81ac4ee1f0d7b8)
    - [論文紹介『Swin Transformer: Hierarchical Vision Transformer using Shifted Windows』](https://kyla.co.jp/blog/2021/05/10/%E8%AB%96%E6%96%87%E7%B4%B9%E4%BB%8B%E3%80%8Eswin-transformer-hierarchical-vision-transformer-using-shifted-windows%E3%80%8F/)
    - [Transformer(ViT)系より良いConvだけのネットワーク出たよ（画像認識向け）](https://qiita.com/TeamN/items/edee1b3803a1d77fc252)
